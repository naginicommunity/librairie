---
description: >-
  Traduction de la partie Introduction au Mimblewimble et Grin disponible dans
  la documentation du site officiel.
---

# Mimblewimble et Grin

## **Introduction**

Mimblewimble est une blockchain et un protocole qui offrent une excellente évolutivité, une confidentialité et une fongibilité en s'appuyant sur des primitives cryptographiques fortes. Il évoque les pièces manquantes/comble les lacunes existant dans presque toutes les implémentations actuelles de blockchain.

Grin est un projet de logiciel libre qui met en œuvre une blockchain Mimblewimble et comble les lacunes nécessaires au déploiement d'une blockchain et d'une crypto-monnaie.

L'objectif principal et les caractéristiques du projet Grin sont les suivantes :

* la confidentialité par défaut. Cela permet la totale fongibilité sans empêcher le fait de divulguer de manière sélective des informations selon les besoins.
* Mise à l'échelle principalement avec le nombre d'utilisateurs et minimalement avec le nombre de transactions (noyau <100 octets), ce qui permet un grand gain d'espace par rapport aux autres blockchains.
* Une cryptographie forte et montrée. Mimblewimble s'appuie uniquement sur la cryptographie elliptique à courbe, ce qui a été essayé et testé depuis des décennies
* Un simple design qui facilite l'audit et la maintenance au cours du temps.
* Dirigé par la communauté, il encourage la décentralisation de l'exploitation de la minorité.

Vous trouverez un article détaillé étape par étape sur le fonctionnement des transactions Grin, dans cet article Medium.

**Une difficulté pour tout le monde**

Ce document s’adresse aux lecteurs avec une bonne compréhension de la blockchain et la cryptographie basique. Avec ceci en tête, nous tentons d'expliquer la construction technique de Mimblewimble et comment elle est appliquée dans Grin. Nous espérons que ce document est compréhensible pour une partie des lecteurs à l'esprit technique. Notre objectif est de vous encourager à vous intéresser au Grin et à y contribuer de quelque manière que ce soit.

Pour atteindre cet objectif, nous allons introduire les principaux concepts exigés pour une bonne compréhension de Grin en tant qu’implémentation du Mimblewimble. Nous commencerons par une brève description de certaines propriétés clés du la Courbe Elliptique Cryptographique (CEC) pour poser les bases sur lesquelles Grin est fondé, puis nous décrirons tous les éléments clés d'une transaction et des blocs d'une blockchain Mimblewimble.

**Des petits bouts de courbes elliptiques**

Nous commençons par une brève introduction sur la Courbe Elliptique Cryptographique, en passant par les propriétés nécessaires pour comprendre le fonctionnement de Mimblewimble et sans trop nous plonger dans les subtilités de l'CEC. Pour les lecteurs qui souhaitent en connaître beaucoup plus sur ses hypothèses, il y a d’autres opportunités pour en savoir plus.

Dans les cadres de la cryptographie, une courbe elliptique est simplement un ensemble de points que nous appellerons “C”. Ces points peuvent être additionner ou soustraits et le résultat est un point sur la courbe. De plus, un point peut être successivement additionner à soi même, ceci étant représenter comme une multiplication par des entiers. Étant donné un tel point H, un nombre entier k et en utilisant l'opération de multiplication scalaire, nous pouvons calculer k\*H, qui est également un point sur la courbe C. Étant donné un autre nombre entier j, on peut également calculer (k+j) \*H , qui est égal à k\*H + j\*H. Les opérations d'addition et de multiplication scalaire sur une courbe elliptique conservent la propriété distributive de l'addition et de la multiplication : (k+j) \* H = k\*H + j\*H

En CEC, si nous choisissons un (très grand) nombre k en tant que clé privé, k\*H est considéré comme la clé publique correspondante. Même si un individu connaît la valeur de la clé publique k\*H, en déduire k est presque impossible (ou autrement dit , alors que la multiplication est triviale, la "divison" par les points de courbe est extrêmement difficile)

La formule précédente (k+j) \*H = k\*H + j\*H, avec k et j tout les deux des clés privés, démontre qu’une clé publique obtenue par l’addition de deux clés privés ((k+j) \*H) est identique que l’addition de deux clés publiques pour chacune des clés privés (k\*H + j\*H). Dans la blockchain Bitcoin, les portefeuilles déterministes hiérarchiques s'appuient fortement sur ce principe. Mimblewimble et le Grin le font également.

**Effectuer des transactions avec Mimblewimble**

La structure des transactions démontre une partie cruciale de Mimblewimble: forte assurance de la vie privée et confidentialité garantie. La validation des transactions Mimblewimble est basée sur deux propriétés de base:

* **La verification des sommes nulles**. La somme des sorties moins les entrées est toujours égale à zéro, prouvant que la transaction n’a pas crée de nouveaux fonds, sans révéler les montant réels.
* **La possession des clés privés**. Comme pour la plupart des autres crypto-monnaies, la propriété des résultats de la transaction est garantie par la possession des clés privés CEC. Cependant, la preuve qu’une entité possède sa clé privée n’est pas obtenue en signant directement la transaction.

Les sections suivantes sont sur l'équilibre, la propriété, le changement et les preuves détaillent comment ces deux propriétés fondamentales sont réalisées.

**L’équilibre**

En s'appuyant sur les propriétés de l'CEC que nous avons décrites ci-dessus, on peut masquer les valeurs dans une transaction.

Si v est la valeur d’entrée ou de sortie d’une transaction et H, un point sur la courbe elliptique C, nous pouvons simplement intégrer v\*H à la place de v dans une transaction. Ceci marche car, en utilisant les opérations CEC, on peut toujours valider que la somme des sorties d’une transaction est égale à la somme des entrées: v1+v2=v3 => v1\*H +v2\*H = v3\*H

En vérifiant cette propriété sur chaque transaction permet au protocole de vérifier qu’une transaction ne créer pas de monnaie à partir de rien, sans savoir quelles sont les valeurs réelles.

A noter que connaître v1 (d’une transaction précédente par exemple) et le résultat v1\*H révèle toutes les sorties avec la valeur v1 à travers la blockchain. Nous introduisons un deuxième point G sur la même courbe elliptique (pratiquement G est juste un autre point générateur sur le même groupe de courbes que H) et une clé privée r utilisée comme facteur d'aveuglement.

Une valeur d'entrée ou de sortie dans une transaction peut alors être exprimée comme r\*G + v\*H

où :

* r est une clé privée utilisée comme facteur aveuglant, G est un point sur la courbe elliptique C et le point r\*G est la clé publique pour r (en utilisant G comme point générateur).
* v est la valeur d'une entrée ou d'une sortie et H est un autre point sur la courbe elliptique C, produisant ensemble une autre clé publique v\*H (utilisant H comme point générateur)

Ni v ni r ne peuvent être déduits, grâce aux propriétés fondamentales de la cryptographie par courbes elliptiques. r\*G + v\*H est appelé un engagement de Pedersen.

A titre d'exemple, supposons que nous voulons construire une transaction avec deux entrées et une sortie, nous avons (en ignorant les frais) :

\-vi1 et vi2 comme valeurs d'entrée

* vo3 comme valeur de sortie

Tels que : vi1 + vi2 = vo3

Générer une clé privée comme facteur pour chaque valeur d'entrée et remplaçant chaque valeur par leurs engagements respectifs de Pedersen. Dans l’équation précédente, nous obtenons :

(ri1\*G) + vi1\*H) + (ri2\*G + vi2\*H) = ro3\*G + vo3\*H). Par conséquence ceci exige : (ri1 + ri2 = ro3). Ceci est le premier pilier de Mimblewimble : l'arithmétique nécessaire pour valider une transaction peut être effectuée sans connaître aucune des valeurs.

Pour finir, cette idée est en fait dérivée de « Confidential Transactions » de Greg Maxwell, qui est lui-même dérivé de la proposition d'Adam Back concernant l'application de valeurs homomorphique dans Bitcoin.

**Propriété**

Dans la section précédente, nous avons introduit une clé privée comme un facteur aveuglant pour obscurcir les valeurs de la transaction. La deuxième idée de Mimblewimble est que cette clé privée peut être utilisée pour prouver la propriété de la valeur. Par exemple, Alice vous envoie 3 pièces et pour masquer ce montant, vous choisissez 28 comme facteur aveuglant quelque part sur la blockchain, le résultat suivant apparaît et ne peut être dépensé que par vous :

X = 28\*G + 3\*H

X, le résultat de l'addition, est visible pour tous. La valeur 3 n'est connue que de vous et Alice, et 28 n'est connu que de vous pour transférer à nouveau ces trois pièces, le protocole exige qu'il soit connu d'une manière ou d'une autre. Pour démontrer comment cela fonctionne, disons que vous voulez transférer ces 3 mêmes pièces à Carol. Vous devez construire une transaction simple telle que: Xi => Y

Si Xi est une entrée qui dépense votre production X et Y est la sortie de Carol. Il est impossible de faire une telle transaction et de l'équilibrer sans connaître la clé privée de 28. En effet, si Carole doit équilibrer cette transaction, elle doit connaître à la fois la valeur envoyée et votre clé privée pour que: Y – Xi = (28\*G + 3\*H) – (28\*G + 3\*H) = 0\*G + 0\*H

En vérifiant que tout a été mis à zéro, nous pouvons à nouveau nous assurer qu'aucune nouvelle monnaie n'a été créée. Mais attendez ! Stop ! Maintenant vous connaissez les clés privées de la sortie de Carole (qui, dans ce cas, pour s’équilibrer doivent être les mêmes que les vôtres) et vous pouvez donc lui voler votre argent ! Pour résoudre ce problème, Carole utilise une clé privée de son choix. Elle choisit 113 par exemple et ce qui se retrouve sur la blockchain est :

Y – Xi = (113\*G + 3\*H) – (28\*G + 3\*H) = 85\*G + 0\*H. Maintenant, la somme de cette opération n'est plus égale à zéro et nous avons une valeur excédentaire (85), qui est le résultat de la somme ou de la soustraction de tous les facteurs aveuglants ; notez que 85\*G est une clé publique valide pour le point générateur G.

Par conséquent, le protocole doit vérifier que les parties contractantes peuvent collectivement produire la clé privé (85 dans l’exemple précédent) pour le point Y-Xi (ceci devrait être la clé publique correspondante, pour le point générateur G ; 85\*G dans l’exemple ci-dessus). Une simple façon de faire cela c’est en utilisant la clé publique Y-Xi (85\*G) pour vérifier une signature, ceci était signé en utilisant la valeur excessive (85). Cela assure que:

* Les parties contractantes peuvent collectivement produire la clé privé (la valeur en excès) pour la clé publique (Y-Xi)
* La somme des valeurs des sorties moins la somme des valeurs des entrées est zéro (sinon il n’y aurait pas de correspondance entre les clés publiques et privés, ce qui est exactement la raison pour laquelle il y a une signature)

Cette signature, attachée à chaque transaction, ainsi que certains frais supplémentaires d'exploration de données, est appelé « noyau de transaction » ou encore en anglais « transaction kernel » et est vérifiée par tous les validateurs.

**Quelques points plus précis**

Cette section du texte détaille sur la construction des transactions en discutant comment le changement est introduit et l'exigence de preuves d'étendue pour que toutes les valeurs soient prouvées comme étant non négatives. Aucun de ces éléments n'est absolument nécessaire pour comprendre Mimblewimble et Grim, donc si vous êtes pressé, n'hésitez pas à passer directement à l’onglet Mettre tout en place ou « Putting it all together »

**Change**

Disons que vous souhaitez envoyer 2 coins à Carol des 3 que vous avez reçu d’Alice. Pour faire cela, vous aller vous renvoyer le restant 1 coin à vous même en tant que monnaie restante. Vous générez une autre clé privée (disons 12 par exemple) en tant que facteur aveuglant pour protéger votre production de monnaie. Carol utilise sa même clé privée d’avant.

Sortie de monnaie : 12\*G + 1\*H

Sortie de Carol: 113\*G + 2\*H

Ce qui se retrouve sur la blockchain est très similaire à ce qui existait avant. Et la signature est encore une fois construite avec la valeur excédentaire, ici 97.

(12\*G + 1\*H) + (113\*G + 2\*H) - (28\*G + 3\*H) = 97\*G + 0\*H

**Preuves d’étendue**

Dans tous les calculs au-dessus, on s’appuie sur le fait que les valeurs de transactions soient positives. L’introduction de montant négatifs serait extrêmement problématique car on pourra créer des nouveaux fonds à chaque transaction.

Par exemple, une personne pourrait créer une transaction avec une entrée de 2 et des sorties de 5 et -3 et obtenir quand même une transaction bien équilibrée. Ceci ne peut pas être facilement détecté car même si x est négatif, le point correspondant x\*H sur la courbe ressemble à n'importe quel autre.

Pour résoudre ce problème, Mimblewimble s'appuie sur un autre concept cryptographique issu des transactions confidentielles, appelé preuve d'intervalle : la preuve qu'un nombre se situe dans un intervalle donné, sans révéler le nombre. Nous ne nous étendrons pas sur la preuve d'intervalle qui montre que « v » est non négatif et ne déborde pas.

Il est aussi important de noter que les preuves d’intervalle sont nécessaires pour le facteur aveuglant et les valeurs.

La raison en est qu'elle empêche une attaque de censure où une tierce partie serait capable de verrouiller les utxo sans connaître leurs clés privées en créant une transaction telle que la suivante :

* L'UTXO de Carole : 113\*G + 2\*H
* Sortie de l'attaquant : (113+99) \*G + 2\*H

qui peut être signé par l'attaquant car les facteurs d'aveuglement de Carole s'annulent dans l'équation Y-Xi: Y -Xi = ((113+99) \*G + 2\*H) – (113\*G +2\*H) = 99\*G.

Cette sortie ((113 + 99) \*G + 2\*H) exige que tous les deux nombres 113 et 99 sont connu pour être dépensé; l’attaquant aurait donc réussi à verrouiller l'UTXO de Carole. L'exigence d'une preuve de portée pour le facteur d'aveuglement empêche cela, car l'attaquant ne connaît pas le nombre 113 et donc pas non plus (113+99). Une description plus détaillée des preuves de portée est présentée dans le document de portée.

**Tout mettre en place**

Une transaction Mimblewimble comprend les éléments suivants:

* Une paire d’entrées, qui font référence et dépensent un ensemble de sorties précédentes.
* Un ensemble de nouvelles sorties qui comprennent :
* un facteur d'aveuglement r et une valeur v utilisée pour la multiplication scalaire pour les points de courbe G, H respectivement, et ensuite additionnés pour être r\*G + v\*H
* une preuve de portée qui montre, entre autres, que v est non négatif
* Des frais de transaction en texteclair
* Une signature signée avec la valeur en excès (la somme de toutes les valeurs de sorties et des frais moins les valeurs d’entrée) comme la clé privée.

**État des blocs et des chaînes**

Nous avons expliqué ci-dessus comment les transactions Mimblewimble peuvent fournir de fortes garanties d'anonymat tout en maintenant les propriétés requises pour une blockchain valide, c'est-à-dire qu'une transaction ne crée pas d'argent et que la preuve de la propriété est établie par des clés privées. Avec cet ajout, une chaîne Mimblewimble gagne :

* une très bonne évolutivité, puisque la grande majorité des données de transaction peuvent être éliminées au fil du temps, sans compromettre la sécurité.
* un anonymat supplémentaire grâce au mélange et à la suppression des données de transaction

**Regroupement des transactions**

Pour rappeler, une transaction consiste en:

* un ensemble d'entrées qui référencent et dépensent un ensemble de sorties аantérieures,
* un ensemble de nouvelles sorties,
* un noyau de transaction composé de: l’excès du noyau et de la signature de la transaction signée par la valeur excédentaire.

(La présentation ci-dessus n’a pas explicitement parler et inclut l’excédent du noyau dans la transaction, car elle peut être calculée à partir des entrées et des sorties. Ce paragraphe montre les avantages de celui-ci et pourquoi l’inclure, pour le regroupement dans la construction du block)

Nous pouvons dire que l’expression suivante est vraie pour toute transaction :

somme(sorties) – somme(entrées) = excès noyau

Il en va de même pour les blocs eux-mêmes, une fois que l'on a compris qu'un bloc n'est qu'un ensemble d'entrées, de sorties et de noyaux de transaction englobés. Nous pouvons additionner les sorties’ soustraire les entrées et en assimilant l'engagement de Pedersen résultant à la somme de l'excès de noyau : somme(sorties) - sommes(entrées) = somme (noyau\_excès)

En simplifiant un peu (en ignorant les frais de transaction), nous pouvons affirmer que les blocks de Mimblewimble peuvent être traités de la même manière que Mimblewimble.

**Offsets de noyau**

Il existe un léger problème avec les blocks et les transactions Mimblewimble énoncés plus haut. Il est possible (et dans certains cas trivial) de reconstruire la transaction constituant le block. Ceci a clairement un impact négatif sur le confidentiel. C’est est un « sous » problème: prenons un ensemble d’entrées, de sorties et de transactions noyau, un ensemble de ceux-ci va se combiner et restructurer une transaction valide.

Considérer les deux transactions suivantes:

(in1, in2) —> (out1), (kern1)

(in3) —> (out2), (kern2)

Nous pouvons les rassembler dans les blocks suivants:

(in1, in2, in3) —> (out1, out2), (kern1, kern2) //

(entrée1, entrée2, entrée3) —> (sortie1, sortie2), (noyau1, noyau2)

Il est très facile d’essayer toutes les permutations possibles pour récupérer une des transactions (ou à la somme égale à zéro).

(in1, in2) —> (out1), (kern1)

Nous savons aussi que tout reste peut être utilisé pour reconstruire les autres transactions valides (in3)—> (out2), (kern2)

Retenez que l’excès de noyau r\*G est tout simplement la clé publique de la valeur en excès r. Pour atténuer cela, nous pouvons réécrire l’excès de noyau de r\*G à (r-kernel\_offset)\*G et distribuer le kernel offsets \*\*\*\*a être inclus depuis cette étape dans chaque transaction noyau. La compensation du noyau est donc un facteur aveuglant qui doit être ajouté à la valeur excédentaire pour que la somme des engagements soit égale à zéro:

somme(sorties) - somme(entrées) = r\*G = (r-kernel\_offset)\*G + kernel\_offset\*G

ou alternativement

somme(sorties) – somme(entrées) = kernel\_excess + kernel\_offset\*G

Pour un engagement r\*G + 0\*H avec le décalage a, la transaction est signée avec (r-a) et a est publié pour que r\*G puisse être calculé afin de vérifier la validité de la transaction : étant donné l'excès du noyau (rappelons qu'il est donné comme une partie du noyau de la transaction) (r-a)\*G et le décalage a, on calcule a\*G et on obtient (r-a)\*G + a\*G = r\*G. Pendant la construction du bloc, tous les décalages de noyau sont additionnés pour générer un seul décalage de noyau agrégé couvrant l'ensemble du bloc. Le décalage du noyau pour toute transaction individuelle est alors irrécupérable et le problème du sous-ensemble est résolu.

**Couper à travers/selection**

Les blocs permettent aux mineurs d'assembler plusieurs transactions en un seul ensemble qui est ajouté à la chaîne. Dans les représentations des blocs suivants, contenant 3 transactions, nous ne montrons que les entrées et les sorties des transactions. Les entrées font référence aux sorties qu'elles dépensent. Et les sorties incluses dans un bloc précédent sont marquées d'un x minuscule.

I1(x1) --- O1

```
    \|- O2
```

I2(x2) --- O3

I3(O2) -|

I4(O3) --- O4

```
    \|- O5
```

Nous remarquons les deux propriétés suivantes :

* Dans ce bloc, certaines sorties sont directement dépensées par les entrées suivantes (I3 dépense O2 et I4 dépense O3).
* La structure de chaque transaction n'a pas vraiment d'importance. Puisque la somme de toutes les transactions est individuellement égale à zéro, la somme de toutes les entrées et sorties de la transaction doit être nulle.

Comme pour une transaction, tout ce qui doit être vérifié dans un bloc est que la propriété doit prouvée (ce qui provient des transactions noyaux) et que l'ensemble du bloc n'a pas créé de pièces (autres que ce qui est autorisé comme récompense pour le minage). Par conséquent, les entrées et sorties correspondantes peuvent être éliminées, car leur contribution à la somme globale s'annule. Ce qui conduit au bloc suivant, beaucoup plus compact :

I1(x1) | O1

I2(x2) | O4

```
   \| O5
```

Notez que toute la structure de transaction a été éliminée et que l'ordre des entrées et des sorties n'a plus d'importance. Cependant, la somme de toutes les entrées et sorties est toujours garantie comme étant égale à zéro.Un bloc est simplement construit à partir de :

* Un en-tête de bloc.
* La liste des entrées restantes après le découpage.
* La liste des sorties restantes après le découpage.
* Un seul décalage de noyau (somme de tous les décalages de noyau) pour couvrir le bloc complet.
* Les noyaux de transaction contenant, pour chaque transaction :

\-La clé publique (r-a)\*G, qui est l'excès de noyau (modifié).

\-Les signatures générées en utilisant la valeur de l'excès (modifié) (r-a) comme clé privée (de signature).

\-Les frais de minage.

Le contenu du bloc satisfait :

sum(outputs) - sum(inputs) = sum(kernel\_excess) + kernel\_offset\*G

Lorsqu'il est structuré de cette manière, un bloc Mimblewimble offre de très bonnes garanties de confidentialité :

* Les transactions intermédiaires (cut-through) ne seront représentées que par leurs noyaux de transaction.
* Toutes les sorties se ressemblent : de très grands nombres impossibles à différencier de manière significative les uns des autres. Si quelqu'un veut exclure une sortie spécifique, il devra tout exclure.
* Toute la structure des transactions a été supprimée, ce qui rend impossible de dire quelles entrées et sorties correspondent.

Et pourtant, tout est toujours valide !

**La transparence jusqu'au bout**

Pour en revenir à l'exemple de bloc précédent, les sorties x1 et x2, dépensées par I1 et I2, doivent être apparues précédemment dans la blockchain. Ainsi, après l'ajout de ce bloc, ces sorties ainsi que I1 et I2 peuvent également être retirées de la blockchain car elles sont maintenant des transactions intermédiaires.

Nous concluons que l'état de la chaîne (à l'exclusion des en-têtes) à tout moment peut être résumé par ces seuls éléments d'information :

1. La quantité totale de pièces créées par le minage dans la chaîne.
2. L'ensemble complet des sorties non dépensées.
3. Les noyaux de transaction pour chaque transaction.

Le premier élément d'information peut être déduit en utilisant simplement la hauteur du bloc.

Les UTXOs et les noyaux de transaction sont extrêmement compacts. Cela a deux conséquences importantes :

* La blockchain qu'un nœud doit maintenir est très petite (de l'ordre de quelques gigaoctets pour une blockchain de la taille d'un bitcoin, et potentiellement optimisable à quelques centaines de mégaoctets).
* Lorsqu'un nouveau nœud rejoint le réseau, la quantité d'informations qui doit être transférée est très faible.

En outre, l'ensemble UTXO ne peut pas être altéré. L'ajout ou la suppression d'une seule entrée ou sortie modifierait la somme des transactions pour qu'elle soit différente de zéro.

**Conclusion**

Dans ce document, nous avons couvert les principes de base qui soulignent/décrivent une blockchain de Mimblewimble. En utilisant l’addition des points de la courbe elliptique, nous sommes capables de construire des transactions qui sont complétement opaques mais qui peuvent quand meme être validé. Et en généralisant ces propriétés aux blocs, nous pouvons éliminer une grande quantité de données de la blockchain, ce qui permet une grande mise à l'échelle et une synchronisation rapide de nouveaux pairs.
