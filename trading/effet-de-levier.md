# Effet de levier

## **Introduction**

Certains traders aimeraient avoir des positions avec une exposition supérieure que ce que leur capital ne leur permet. C’est pour cela que la plupart des courtiers proposent des CFD (contract for difference) permettant de prendre position avec un effet de levier. Cela signifie que la position du trader sera supérieure à celle permise par son capital. Dans cet article, nous allons explorer les différentes possibilités de l’effet de levier.

## **Le levier**

Le courtier prêtera au trader une valeur lors de l’ouverture d’une position. Lorsque le trader fermera la position, il rendra la valeur au courtier. Ainsi, les gains du trader seront multipliés, mais également ses pertes. On appelle levier le ratio utilisé entre le capital investit par le trader et le capital prêté.

Exemple :

Imaginons un Bitcoin à 10 000$. Un trader possédant 1 000$ veut ouvrir une position long (à la hausse) sur le Bitcoin. Si ce trader n’utilise pas d’effet de levier, il investit ses 1000$ et a en retour 0.1 Bitcoin. Maintenant si ce trader utilise un effet de levier disons 1 :10, il investit toujours 1 000 $ mais a en retour l’équivalent de 1 Bitcoin

Imaginons maintenant deux scénarios : dans le premier, le Bitcoin vaut maintenant 11 000 $

En vendant ses bitcoins, le trader recevra sans effet de levier 0.1 x 10 100 / 10 000 = 1 010 $ et avec effet de levier 1 x (10 100/10 000) – 9 000 =1 100 $

Dans le second cas, le bitcoin vaut maintenant 9 900 $

Sans effet de levier le trader a maintenant 990$ , avec effet de levier il a 900$

Vous l’aurez compris, l’effet de levier multiplie les profits comme les pertes.

Les positions à effet de levier peuvent etre prises en long ou en short et fonctionnent de la même manière dans les 2 situations.

On appelle marge le capital investit par le trader. Il y a une relation entre marge et effet de levier : en inversant le ratio on retrouve le pourcentage de marge.

Exemple :

Un levier de 10:1 donne une marge de 10% de la position totale

Un levier de 20 :1 donne une marge de 5%

Un levier de 2 :1 donne une marge de 50%

Il est important de correctement choisir son effet de levier en fonction de la liquidité du marché.

En effet, sur un marché peu volatile, ne pas avoir d’effet de levier demanderait une équité énorme. Au contraire, sur un marché très volatile, un fort effet de levier pourrait fermer la position même si cette dernière est viable sur le long terme.

## **Margin Call**

Imaginons maintenant que le prix du bitcoin tombe à 8 000 $

Dans le premier cas, le trader a 800$ , mais dans le second, il a – 1000$ C’est-à-dire que le trader n’est même plus capable de rembourser le courtier. La plupart des courtiers refusent de prendre ce risque, c’est pourquoi il y a souvent dans le contrat une clause stipulant que la position est fermée lorsque le trader n’est plus capable de rembourser le courtier. On appelle cela un margin call ou liquidation. Afin d’évité une fermeture brutale de la position, le courtier peut demander au trader de rajouter des fonds afin de couvrir les pertes. Dans le cas de forts mouvements, il se peut que le courtier ne soit pas capable de fermer la position à temps, dans ce cas, il sera en droit de demander au trader de rembourser les pertes supplémentaires. En pratique, les courtiers refusent même de s’exposer à une perte de 100% des traders. C’est pourquoi la position est liquidé automatiquement à un pourcentage de la marge. Le pourcentage minimal fixé par la FINRA (Financial Industry Regulatory Authority) est de 25%, mais il est possible que les échanges mettent un pourcentage supperieur. On appelle ce pourcentage Maintenance Margin.

Exemple :

Sur une position à effet de levier à 10 :1 avec une marge de 100$ et une Maintenance Margin à 25%, si l’ouverture de la position se fait à 100$, la position totale sera de 1 000 $, la Maintenance margin se fera au bout de 75$ de perte donc quand la position totale sera à 925$, c’est-à-dire que le prix sera à 92.5$

La maintenance margin dépend de la taille de la position. En effet, liquider une énorme position entrainera une variation du prix (slippage). Ainsi, le courtier est en droit d’exiger une marge plus grande

Bien évidemment, le prêt n’est pas gratuit, et une position à effet de levier entrainera des intérêts.

La plupart des détails dépendent de la plateforme et des courtiers. Nous allons par la suite étudier les conditions des effets de levier des plus grandes plateformes.

**Binance**

L’effet de levier max dépend de la crypto en question. Et la maintenance margin de la taille de la position. Les positions

[https://www.binance.com/au/support/articles/360033162192-Leverage-and-Margin-of-Perpetual-Futures-Contracts](https://www.binance.com/au/support/articles/360033162192-Leverage-and-Margin-of-Perpetual-Futures-Contracts)

[https://www.binance.com/fr/fee/marginFee](https://www.binance.com/fr/fee/marginFee)

les leviers se font en USDT

**Kraken**

https://support.kraken.com/hc/en-us/articles/227876608-Margin-trading-pairs-and-their-maximum-leverage

Kraken demande un Collatéral (une assurance) afin de pouvoir se rembourser en cas de forte variation d’un asset.

Fees : https://support.kraken.com/hc/en-us/articles/206161568
