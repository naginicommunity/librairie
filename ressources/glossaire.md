# 📚 Glossaire

## 51% Attack

{% hint style="info" %}
Si plus de la moitié de la puissance informatique ou de la quantité de [minage](glossaire.md#minage) sur un réseau est géré par une seule personne ou un seul groupe de personnes, une attaque de 51% est en cours.

Cela signifie que cette entité a le plein contrôle du réseau et peut affecter négativement une [cryptomonnaie](glossaire.md#crypto-monnaie) en prenant le contrôle des opérations minières, en arrêtant ou en doublant les dépenses (réutilisation) des [coins](glossaire.md#coin-piece).
{% endhint %}

## Account Based (Basé sur le compte)

{% hint style="info" %}
Vous utilisez des [blockchains](glossaire.md#blockchain) qui disposent de mécaniques différentes pour suivre votre solde, sans forcément le savoir. Ces différences fondamentales font que certaines blockchains sont plus adaptées à un type d’usage : [Bitcoin](glossaire.md#bitcoin) pour des échanges d’argent et [Ethereum](glossaire.md#ethereum) pour l’exécution de [smart contract](glossaire.md#smart-contract).

Bitcoin utilise le schéma [UTXO](glossaire.md#utxo) (Unspent Transaction Output) tandis qu'[Ethereum ](glossaire.md#ethereum)utilise le modèle Account Based.

La gestion des soldes dans le modèle Account Based est le plus familier des deux modèles et fonctionne dans [Ethereum](glossaire.md#ethereum) de la même manière que dans le monde bancaire traditionnel. Essentiellement, chaque compte subit des transferts directs de valeur et d'informations avec des transitions d’état.

Dans [Ethereum](glossaire.md#ethereum), il existe deux types de comptes, les comptes d'utilisateurs contrôlés par [clé privée](glossaire.md#cle-privee) et les comptes contrôlés par code de contrat (contrats intelligents). Ceci est important car c'est une raison vitale pour laquelle Ethereum a choisi le modèle account based plutôt que le modèle UTXO. Étant donné qu'Ethereum utilise un langage de programmation complet Turing ([Solidity](glossaire.md#solidity) principalement) et que l'une de ses principales caractéristiques est les contrats intelligents, le modèle de compte offre une simplicité beaucoup plus grande que le modèle basé sur UTXO utilisé par Bitcoin. Ethereum possède une quantité substantielle [d'applications décentralisées](glossaire.md#dapps-applications-decentralisees) contenant un état et un code arbitraires, il n'est pas logique d'utiliser le modèle UTXO utilisé dans Bitcoin car cela limiterait intrinsèquement la capacité des contrats intelligents à s’exécuter.

Les avantages spécifiques offerts par le modèle de compte dans Ethereum sont un gain de place plus important, la simplicité, la familiarité et la fongibilité. Chaque transaction dans le modèle de compte n'a besoin que de faire une référence et une signature qui produisent une sortie, contrairement à la conception UTXO. Cela permet des économies d'espace substantielles, ce qui est vital pour une plate-forme aussi grande et complexe qu'Ethereum. De plus, outre la familiarité et la simplicité permises par le modèle basé sur le compte, le degré de fongibilité de la blockchain Ethereum est beaucoup plus élevé que celui du Bitcoin. Les utilisateurs d'Ethereum effectuent des transactions à l'aide d' appels de procédure à distance du client qui rendent le suivi des transactions internes dans le registre Ethereum beaucoup plus difficile que Bitcoin où toutes les transactions sont publiquement liées via le registre en suivant les signatures numériques du schéma UTXO. Ainsi, la fongibilité est augmentée car la liste noire des marchands de pièces utilisées pour des activités illicites est difficile à réaliser.

De l'autre côté, les inconvénients du modèle de compte tournent autour de celui-ci limitant l'évolutivité de la plateforme. Bien qu'une implémentation nécessaire en raison de la conception d'Ethereum, les problèmes d'évolutivité entourant le développement d'Ethereum sont bien établis et une préoccupation qui est venue au premier plan de l'industrie. La conception de la logique autour du modèle de compte n'est pas aussi simple qu'avec le modèle UTXO et peut avoir des implications potentielles sur d'autres concepts de conception au sein de la plate-forme à mesure qu'elle continue de croître.
{% endhint %}

## Adresse

{% hint style="info" %}
Une adresse permet de désigner la destination d'un paiement. En ce sens, elle peut être considérée comme l'équivalent d'un numéro de comptes Iban, ou l’identifiant de votre compte.
{% endhint %}

## Airdrop

{% hint style="danger" %}
Pour une entreprise un Airdrop consiste à offrir des [tokens](glossaire.md#token-jeton) ou des [coins](glossaire.md#coin-piece) de leurs cryptomonnaies en échanges de quelques contreparties comme partager une publication twitter, rejoindre un groupe Telegram, aimer leurs pages sur différents réseaux sociaux …..

Vous pouvez recevoir ces tokens sur votre [clé publique](glossaire.md#cle-publique) ethereum par exemple.

Il n’y a pas vraiment de règles pour savoir combien on peut gagner mais plus le projet semble prometteur, plus vous gagnerez de l’argent. Au pire, vous aurez perdu du temps.

Arnaques à éviter : ne jamais communiquer sa clé privée, ne télécharger aucun fichier, utiliser un nouveau mot de passe pour sa boite mail, ne jamais verser d’argent.
{% endhint %}

## Altcoin

{% hint style="info" %}
Un Altcoin fait référence à toute crypto-monnaie qui n’est pas Bitcoin et qui englobe les crypto-monnaies et les jetons dans le même terme.

Les altcoins sont des actifs numériques qui s’appuient sur la technologie blockchain mais intègrent d’autres fonctionnalités et d’autres protocoles de validation que le bitcoin.

Potentiellement le nombre d’altcoins est infini, tout le monde pouvant décider de lancer sa propre cryptomonnaie. Chaque altcoin dispose d’une valeur et d’un volume d’échanges qui lui est propre.

Des altcoins se trouvent aujourd’hui au coeur de véritables écosystèmes permettant notamment de passer des [**smart contacts**](glossaire.md#smart-contract) ou d’organiser des levées de fonds.
{% endhint %}

## Alt Season

{% hint style="info" %}
La définition de Alt Season est une période où uniquement les altcoins ou autres cryptomonnaies que Bitcoin sont en hausse de manière importante avec parfois un prix de Bitcoin qui baisse ainsi que le niveau de sa dominance sur le marché crypto.
{% endhint %}

## AML (Anti Money Laundering)

{% hint style="info" %}
Lutte contre le blanchiement d'argent
{% endhint %}

## AMM (Automated Market Maker)

{% hint style="info" %}
Les Automated Market Maker sont des programmes informatiques qui permettent de remplacer le travail des **market makers.**\
Les AMM sont basées sur des formules mathématiques permettant d’estimer le taux de change entre deux actifs, en prenant également en compte les liquidités présentes sur le protocole.
{% endhint %}

## Analyse fondamentale

{% hint style="info" %}
Méthode utilisée par les investisseurs et les traders pour tenter d'établir la valeur intrinsèque des actifs ou des entreprises. Pour les évaluer avec précision, ils vont étudier rigoureusement les facteurs internes et externes afin de déterminer si l'actif ou l'entreprise en question est surévalué ou sous-évalué. Leurs conclusions peuvent ensuite aider à mieux formuler une stratégie qui sera plus susceptible de produire de bons rendements.
{% endhint %}

## Analyse technique

{% hint style="info" %}
L'analyse technique consiste en l’étude des graphiques de cours de la bourse et de différents indicateurs déduits des cours dans le but de prévoir l'évolution des marchés. L'analyse technique est une discipline commerciale employée pour évaluer les investissements et identifier les opportunités commerciales en analysant les tendances statistiques recueillies à partir de l'activité commerciale, comme le mouvement des prix et le volume.
{% endhint %}

{% hint style="danger" %}
Attention à tous les vendeurs de rêve sur le net avec leur 3 droites et Bot ultra performant 😂
{% endhint %}

## API (Application Proggraming Interface)

{% hint style="info" %}
C’est essentiellement un ensemble de règles décrivant comment deux applications interagissent entre elles.

Une API vous permet de vous connecter à votre Exchange, vous donnant accès aux données du marché en temps réel, vous permet d’effectuer des transactions mais aussi de gérer votre compte.
{% endhint %}

## Arbitrage ou crypto-arbitrage

{% hint style="info" %}
Il s’agit d’une technique de trading qui consiste à profiter des différences ponctuelles de prix ou de cours pour un même actif, sur deux marchés différents.

Il existe d'autres types d'arbitrage
{% endhint %}

## ASIC (Application Specific Integrated Circuit)

{% hint style="info" %}
Un ASIC est un circuit qui intègre, sur une même puce, l’ensemble des éléments actifs indispensables à une seule fonction. Il faudra donc déterminer quelle(s) cryptomonnaie(s) vous souhaitez miner avant de choisir un ASIC car ils sont spécifiques à un seul algorithme de [**Preuve de travail (PoW**).](glossaire.md#pow-proof-of-work-preuve-de-travail)\
Les ASIC sont spécialement créés et achetés à des fins d’exploitation minière et offrent des améliorations d’efficacité et des économies d’énergie significatives du fait de son utilisation spécifique.
{% endhint %}

## ATH (All Time High)

{% hint style="info" %}
Ce sigle correspond à la valeur la plus haute atteinte par une cryptomonnaie.
{% endhint %}

## ATL (All Time Low)

{% hint style="info" %}
Correspond au prix le plus bas enregistré pour une cryptomonnaie.
{% endhint %}

## Atomic Swap (Echange Atomique)

{% hint style="info" %}
C’est une manière décentralisée et sûre d’échanger des cryptomonnaies fonctionnant sur des chaines de blocs différentes. L’adjectif « atomique » insiste sur la nature insécable de l’échange réalisé : soit les deux parties donnent ce qui est dû à l’autre, soit il ne se passe rien.

Si une des deux personnes ne respecte pas son engagement et n’envoie pas les tokens, alors la 1ère personne sera remboursée de son envoi grâce à une protection inscrite dans un [**smart contract**](glossaire.md#smart-contract).
{% endhint %}

## Bag

{% hint style="info" %}
Se rapporte à un sac de cryptomonnaies qu’un investisseur détient.
{% endhint %}

## Bear Market (Marché Baissier ou marché ours)

{% hint style="info" %}
Un bear market correspond à une période où les baisses des prix persistent. On parle également de Bear market si une baisse de 20% ou plus est enregistrée par rapport aux sommets le plus récent ou plus-haut historique.

Il est fortement lié à la psychologie du marché, donc aux comportements des investisseurs ou acteurs du marché.
{% endhint %}

## Bear Trap (Piège à ours)

{% hint style="info" %}
Une technique utilisée par un groupe de traders, visant à manipuler le prix d’une cryptomonnaie.

Le bear trap est mis en place en vendant une grande quantité de la même cryptomonnaie en même temps, induisant le marché en erreur en lui faisant penser à une baisse de prix imminente.

En réponse, d’autres investisseurs vendent leurs actifs, entraînant une baisse supplémentaire des prix.

Ceux qui placent le piège le relâchent alors, rachetant leurs actifs à un prix inférieur.

Le prix rebondit ensuite, leur permettant de réaliser un profit.
{% endhint %}

## BIP (Bitcoin Improvement Protocol)

{% hint style="info" %}
Un BIP est une proposition d’amélioration de Bitcoin. Il en existe trois types :

* Le **BIP de suivi de standard** (standards track BIP), qui concerne les changements qui affectent la plupart ou toutes les implémentations de Bitcoin, comme une modification du protocole de communication, des règles de validité des blocs ou des transactions, ou encore tout changement ou ajout qui impacte l’interopérabilité des applications utilisant Bitcoin. Il s'agit du type de BIP le plus courant.
* Le **BIP informationnel** (informational BIP), qui décrit un problème dans la conception de Bitcoin ou donne des directives générales ou des informations à la communauté de Bitcoin, mais **ne propose pas de nouvelle fonctionnalité**.
* Le **BIP de procédure** (process BIP), qui décrit une procédure ou un changement de procédure à adopter. Le BIP de procédure peut concerner le procédé des BIP lui-même (il s'agit alors d'un « méta-BIP »).
{% endhint %}

## Bitcoin

{% hint style="info" %}
Le bitcoin est une monnaie informatique dont la fonction est de réaliser des paiements en ligne, sans intermédiaire.

C'est aujourd'hui (avec les autres cryptos) le seul moyen de détenir de l'argent numériquement.
{% endhint %}

## **Bitcoin Halving**

{% hint style="info" %}
Tous les quatre ans environ, le Bitcoin est soumis à un évènement important appelé Bitcoin Halving ou Halvening qui peut se traduire par la division de moitié de la prime de [minage](glossaire.md#minage) Bitcoin.

Cela s’est produit pour la première fois en 2012 ensuite en 2016 et en 2020. Cela se reproduira en 2024 (c’est inscrit dans le [White Paper](glossaire.md#white-paper-libre-blanc) de Bitcoin).
{% endhint %}

## **Block**

{% hint style="info" %}
Les transactions effectuées entre les utilisateurs du réseau sont regroupées par blocs. Une fois le bloc validé, il est horodaté et ajouté à la chaîne de blocs (blockchain).
{% endhint %}

## **Blockchain**

{% hint style="info" %}
La blockchain est une technologie qui permet de garder la trace d'un ensemble de transactions, de manière décentralisée, sécurisée et transparente, sous forme d'une chaîne de blocs. Un principe de base de la blockchain est de distribuer (en fait de dupliquer) un registre (l'enregistrement des données) entre plusieurs acteurs ([noeuds](glossaire.md#node-noeud)). Le fait d'en avoir plusieurs exemplaires identiques et des mécanismes de contrôle, permet de se passer d'un organe central (le tiers de confiance). A la place, c'est la communauté qui valide de concert les transactions et qui se met d'accord (le consensus) sur une version de référence du registre.
{% endhint %}

## **Blockchain Publique**

{% hint style="info" %}
C’est un registre ouvert à tous. Tout le monde peut y accéder, sans censure, effectuer des transactions et participer au processus de consensus.

Cela ne veut pas dire que tout est visible et claire mais que, ayant un haut niveau de chiffrement, le registre est simplement lisible par les parties prenantes.

Avantages :

* L’objectif est d’éliminer les intermédiaires de toute forme, et plus important encore, de supprimer le besoin de confiance que les intervenants doivent placer en eux pour le bon déroulement de leurs opérations.
* Sécurisé : plus la décentralisation et la participation active sont importantes, plus une blockchain sera sécurisée. En effet, plus il y a de noeuds, plus il sera difficile pour un hacker d’attaquer le réseau. Inconvénients :
* Les blockchains publiques sont extrêmement lentes car il faut du temps à l’ensemble du réseau pour parvenir à un consensus sur l’état des transactions via des mécanismes tels que le PoW des bitcoins. Il y a également des limites au nombres de transactions pouvant entrer dans un bloc et au temps nécessaire pour le traitement des transactions au sein de ce bloc.
{% endhint %}

## **Blockchain Privée**

{% hint style="info" %}
La sécurité, le contrôle et l’organisation des pouvoirs de décision relèvent de l’organe central (une personne morale) investi de la gouvernance et qui engage sa responsabilité.

Certaines entreprise vont donc vouloir créer leur propre blockchain pour des raisons de sécurité ou de contrôle au sein de leur activité.

Avantages :

* rapidité : traitement des transactions plus rapide que celles des blockchain publiques car accès limité,
* Possibilité de passer simplement d’un algorithme de consensus [**Proof of Work (PoW)**](glossaire.md#pow-proof-of-work-preuve-de-travail) à un **Proof of Authority (PoA)**.

Inconvénients :

* l’intégralité du réseau dépend de la crédibilité des noeuds autorisés puisqu’il faut faire confiance à leurs détenteurs censés eux-mêmes vérifier et valider les transactions.
* Avec moins de [noeuds](glossaire.md#node-noeud), il est beaucoup plus facile pour un hacker de prendre le contrôle du réseau et manipuler les données inscrites.
{% endhint %}

## **Block time**

{% hint style="info" %}
Le temps entre la création de 2 blocks. Il est choisi par chaque protocole de manière arbitraire à sa création. Il est par exemple de 10 minutes pour le Bitcoin et de 15 secondes pour l'Ethereum.
{% endhint %}

## **Bots**

{% hint style="info" %}
Il s’agit d’un système reposant sur une technologie proche de l’intelligence artificielle. Un logiciel analyse automatiquement les donnes du marché et effectue des opérations de trading sur la base d’indicateurs construits avec ces mêmes données. Efficace et précis.

Il existe une infinité de manières permettant de développer des stratégies de trading mais elle doivent impérativement reposer sur des connaissances pointues du marché et de son comportement. Car même si certains fournisseurs de bots vous permettent d’accéder à des fonctions de base pour vous permettre de gagner du temps dans la mise en place de votre algorithme, il faut être en mesure de les comprendre et de savoir quand les mettre en pratique.
{% endhint %}

## **Bubble (Bulle)**

{% hint style="info" %}
Les bulles de cryptomonnaies ou bulle Bitcoin sont des bulles spéculatives qui affectent les cryptomonnaies.

L’absence de banque centrale régulatrice permet l’emballement des algorithmes ainsi que la médiation des envolées des cours.

99,99 % du grand public n’utilisant pas de cryptomonnaie pour faire ses achats, l’impact sur l’économie réelle reste de ce fait encore limité.\
Le Bitcoin présentant le comportement d’une bulle mais n’ayant pas complètement échoué, il est difficile de savoir si c’est le cas.
{% endhint %}

## **Bull Market (Marché du taureau)**

{% hint style="info" %}
Marché à tendance haussière. On utilise également l’adjectif « bullish » pour qualifier cette situation.

L’image utilisée est celle d’un taureau qui attaque son adversaire du bas vers le haut avec ses cornes, matérialisant ainsi le mouvement haussier. En opposition au [**Bear market**](glossaire.md#bear-market-marche-baissier-ou-marche-ours) qui désigne un marché baissier car l’ours attaque du haut vers le bas.
{% endhint %}

## **Bull Trap**

{% hint style="info" %}
C’est un faux signal du marché où la tendance à la baisse d’un actif semble être à la hausse, mais ne se matérialise pas, conduisant les taureaux à perdre de l’argent après avoir acheté une cryptomonnaie pensant qu’elle allait monter.

Un piège tendu par des traders comme le [Bear Trap](glossaire.md#bear-trap-piege-a-ours).

C’est la même technique mais on fait croire à une hausse de prix prochaine.
{% endhint %}

## **Buy the remor and sell the news (Acheter la rumeur, vendre la nouvelle)**

{% hint style="info" %}
Quand un évènement important est attendu, on parle de s’y préparer en achetant un jeton en amont de la nouvelle et en le vendant avant la diffusion de l’évènement tant attendu.
{% endhint %}

## **Buy Wall (Mur d'achat)**

{% hint style="info" %}
Un « wall » est la représentation d’un mur sur le carnet d’ordre de la plateforme d’échange d’une cryptomonnaie, sur laquelle sont effectués les ordres de vente et d’achat. On parle de « buy wall » dès lors qu’un volume important d’achats a été effectué au même prix par un utilisateur, ou lorsque plusieurs investisseurs effectuent simultanément des achats d’une devise au même prix.\
Un buy wall ou mur d’achat a tendance à faire grimper le cours d’une monnaie et affecte durablement la fixation de son prix. En effet, si un ou plusieurs gros ordres d’achat ont du mal à être absorbés par le marché, les ordres qui sont effectués à un prix inférieur le seront encore moins. Ce faisant, le buy wall va agir comme une sorte de « seuil plancher » empêchant le cours d’une devise de baisser, pendant une durée plus ou moins prolongée.

Les gros traders, surnommés les « baleines », peuvent manipuler le marché d’une devise en créant de manière artificielle un mur d’achat, pour attirer des investisseurs non aguerris.
{% endhint %}

## **Burned Coin ( brulage de pièce)**

{% hint style="info" %}
En français la « brulage de pièces » consiste à supprimer définitivement des [coins](glossaire.md#coin-piece) de circulation réduisant ainsi l’offre totale d’une crypto-monnaie d’après les étapes suivantes :

* Un détenteur du coin concerné lancera la fonction de brûlage en indiquant qu'il souhaite détruire un nombre de coin pré-désigné.
* Le contrat vérifiera ensuite que la personne a les coins en question dans son portefeuille et que le nombre de coin indiqué est valide. Seuls les nombres positifs fonctionnent.
* Si la personne ne dispose pas de suffisamment de coins ou si le nombre indiqué est invalide (par exemple, 0 ou -5), la fonction de destruction ne sera pas exécutée.
* Si l’intervenant a le solde requis, les coins seront enlevés de ce portefeuille. L'offre totale de ce coin sera alors mise à jour et le surplus de coins sera brûlé.

Les transactions de destruction sont publiques, irréversibles et enregistrées en permanence sur la blockchain.

Cette action vise à diminuer la quantité pour en faire augmenter le prix.
{% endhint %}

## **BFT (Bizantine Fault Tolerance)**

{% hint style="info" %}
En informatique, le **problème des généraux byzantins** est une métaphore qui traite de la remise en cause de la fiabilité des transmissions et de l'intégrité des interlocuteurs. La question est donc de savoir comment, et dans quelle mesure, il est possible de prendre en compte une information dont la source ou le canal de transmission est suspect. La solution implique l'établissement d'un algorithme (d'une stratégie) adapté.

Les algorithmes des Généraux Byzantins (BFT) sont très recherchés car ils garantissent le maintien des propriétés de sécurité sur un réseaux tant qu’un certain nombre de noeuds sont défaillants.

Cette approche du système de consensus implique que l’identité de chaque membre soit connue, ce qui nécessite l’existence d’une entité centralisée en charge de la gestion de ces données. De ce point de vue, les protocoles basés sur un algorithme BFT sont plus adaptes a un modèle de blockchain dite “privées” ou nécessitant une autorisation et offrent une résistance beaucoup plus importante aux attaques.

Ce type de protocole présente l’avantage de la finalité de son consensus c’est dire qu’un block ajouté à la blockchain ne peut être remis en cause, comme c’est notamment possible avec le mécanisme de la Preuve de Travail (Proof of Work). En effet avec BFT il n’est pas possible de créer un « fork »sur la blockchain, ce qui permet d’aligner exécution et confirmation des transactions et ainsi accélérer considérablement leur réalisation.
{% endhint %}

## **Bug Bounty**

{% hint style="info" %}
C\*\*'\*\*’est une campagne organisée pour trouver les derniers bugs ou erreurs encore présentes dans le code informatique en échange d’une récompense.

En générale, les informaticiens sont récompensés par des tokens.
{% endhint %}

## **Candle (Bougie)**

{% hint style="info" %}
Cela représente les bâtonnets rouges et verts sur les charts graphiques : chaque bâtonnet représente une durée (1 mn, 5 min, 1 heure, 1 jour, .)…

Un bâtonnet vert (green candle) indique qu’entre le début (prix d’ouverture) de cette durée et la fin (prix de fermeture) le prix a augmenté.

Un bâtonnet rouge (red candle) indique que le prix a baissé.
{% endhint %}

## **CBDC (Central Banking Digital Currency)**

{% hint style="info" %}
Témoins d’une économie de plus en plus numérique (exemple PayPal) et changeante ainsi que de l’essor de ces monnaies privées, les Banques Centrales des Etats du monde se lancent dans des recherches sur de potentielles monnaies numériques, mais publiques. Afin de répondre aux menaces de la montée en puissance des devises privées digitales, de nombreux gouvernements redoublent d’efforts pour créer une monnaie numérique dans sa version la plus centralisée et la plus souveraine.
{% endhint %}

## **CFD (Contrat sur la différence)**

{% hint style="info" %}
Un CFD, ou Contrat Sur La Différence, est un contrat financier que vous avez avec votre courtier pour échanger la différence de prix entre l’ouverture et la clôture d’une position CFD.

Lorsque vous utilisez les CFD sur crypto-monnaies, vous ne possédez pas le jeton sous-jacent. Vous profitez simplement de sa volatilité. Le grand avantage est que vous n’avez pas à passer par des plateformes d’échange et des procédures complexes pour acheter des jetons ni à les sécuriser dans des portefeuilles.

Avec le trading de CFD, vous utilisez également la marge et l’[effet de levier](glossaire.md#leverage-effet-de-levier), ce qui vous permet d’ouvrir des positions de trading plus importantes que ce que votre solde vous permettait initialement.

Vous pouvez donc trader des montants plus importants et potentiellement gagner (ou perdre) plus. Un autre grand avantage des CFD par rapport aux produits traditionnels est que vous pouvez profiter des marchés à la hausse comme à la baisse, ce qui signifie que vous pouvez profiter de toutes les conditions du marché.
{% endhint %}

## **Chart (graphique)**

{% hint style="info" %}
Chart fait référence aux graphiques et courbes des prix pendant la phase de trading.
{% endhint %}

## **Circulating supply**

{% hint style="info" %}
L'offre en circulation fait référence aux pièces (coin ou token) qui sont accessibles au public, c’est-à-dire le nombre de pièces qui ont déjà été émises moins les pièces hors circulation (par exemple, détenues par l’équipe de développement ou autre). Elle ne doit pas être confondue avec l'offre totale ou l'offre maximale. L'offre totale est utilisée pour quantifier le nombre de pièces existantes. L’offre maximale est le nombre maximum de pièces qui puisse exister pendant la durée de vie de la cryptomonnaie. Offre en circulation = Offre totale - pièces hors circulation (pertes codes, transactions invalides, …)
{% endhint %}

## Clé privée

{% hint style="info" %}
Avoir un compte, c’est posséder une clé privée à partir de laquelle sont générées une [clé publique](glossaire.md#cle-publique) et une [adresse](glossaire.md#adresse). Une clé privée est créée en convertissant une portion de texte générée automatiquement en un fichier clé à l’aide d’un algorithme mathématique, ce qui lui donne une valeur unique. Cette clé permet de générer une [signature](glossaire.md#digital-signature-signature-electronique) en cryptant un message. Une clé privée permet de dépenser de la cryptomonnaie à partir de votre adresse, quelque soit le portefeuille que vous utilisez. Avec la signature et la clé publique on peut s’assurer que c’est bien le détenteur de la clé privée qui est à l’origine de la transaction.
{% endhint %}

## Clé publique

{% hint style="info" %}
Une clé publique est générée à partir d’une clé privée à l’aide d’une méthode de multiplication par courbe elliptique. Cette méthode n’est pas réversible (il est impossible de retrouver une clé privée grâce à la clé publique). Une clé publique permet à d’autres portefeuilles d’effectuer des paiements à votre adresse.
{% endhint %}

## **Cloud Mining**

{% hint style="info" %}
Le cloud mining offre la possibilité de miner des cryptomonnaies sans devoir acheter de matériel ([ASIC](glossaire.md#asic-application-specific-integrated-circuit) par exemple) mais en louant la puissance de calcul aux entreprises qui possèdent l’équipement nécessaire.

Le locataire (le mineur) est rémunéré sur la base de cryptomonnaies créées par de

Avantages :

* pas d’investissement en matériel (tel qu’un ASIC) et économie d’électricité,
* Obtention de crypto-actifs produits par le minage.

Inconvénients :

* Beaucoup de plateformes sont frauduleuses en matière de cloud mining,
* Souvent des frais de fonctionnement sont facturés au client, réduisant la rentabilité de l’opération.
{% endhint %}

## Coin (Pièce)

{% hint style="info" %}
On entend souvent parler de coin et token, un coin fait référence à une crypto monnaie disposant de sa propre blockchain (Bitcoin, Ethereum, ...)
{% endhint %}

## **Coinbase**

{% hint style="info" %}
Coinbase est une plateforme sécurisée qui facilite l’achat, la vente et le stockage de cryptomonnaies telles que Bitcoin, Etherum, …
{% endhint %}

## **Cold Wallet**

{% hint style="info" %}
Un Cold Wallet, contrairement à un Hot Wallet, est un portefeuille crypto qui n’est pas connecté à internet et assure donc une sécurité optimale pour stocker et sécuriser vos bitcoins et cryptomonnaies. **L**es hackers n’ont pas accès, à distance, à votre Cold Wallet.
{% endhint %}

## Confirmation

{% hint style="info" %}
Quelles sont les étapes d’une confirmation :

la [signature](glossaire.md#digital-signature-signature-electronique) d’une transaction (via une [clé privée](glossaire.md#cle-privee)),

la diffusion de la transaction (envoi de la transaction signée sur le réseau)

l’arrivée de la transaction dans le mempool,

la vérification de la transaction et ajout à un bloc par le [mineur](glossaire.md#mineur) gagnant —> la transaction a obtenu 1 confirmation,

l’ajout d’un nouveau bloc après le bloc actuel → la transaction a deux confirmations, etc…
{% endhint %}

## Correction

{% hint style="info" %}
La Correction est un changement brutal de prix qui retrouve son cours antérieur (ou s’en rapproche) après une période de hausse ou de baisse relativement longue.
{% endhint %}

## Consensus

{% hint style="info" %}
Le consensus informatique dans le domaine de la cryptomonnaie est un moyen pour les participants ([noeuds](glossaire.md#node-noeud)) de se mettre d’accord sur la validité d’une transaction et de mettre à jour le grand livre avec un ensemble cohérent de faits confirmés.
{% endhint %}

## Crypto

{% hint style="info" %}
Abréviation pour désigner les cryptomonnaies et les crypto-actifs.
{% endhint %}

## Crypto-actif

{% hint style="info" %}
Plus largement, les crypto-actifs représentent des actifs virtuels stockés sur un support électronique permettant à une communauté d’utilisateurs, les acceptant en paiement, de réaliser des transactions sans avoir à recourir à la monnaie légale.
{% endhint %}

## Crypto-monnaie

{% hint style="info" %}
Une crypto-monnaie est une devise électronique (ou virtuelle). Cette monnaie est émise de pair à pair, sans nécessité de banque centrale, utilisable au moyen d’un protocole informatique de transactions cryptées et décentralisées, appelé [blockchai](glossaire.md#blockchain)n ou chaine de blocs.
{% endhint %}

## DAG (Direct Acyclic Graph)

{% hint style="info" %}
Technologie inspirée de la blockchain mais différente dans ca manière d'organiser la succession des transactions, ce protocole a été introduit par la crypto NANO.

Un DAG est une structure qui n’a que des liens directs entre ses noeuds et aucun cycle. Pour faire simple, chaque utilisateur dispose de sa propre chaine de transaction, en n’ayant jamais connaissance de la structure globale des données. Si une transaction avec un autre compte doit avoir lieu, on vérifie uniquement les soldes des deux comptes. L’utilisation d’un DAG apporte donc des avantages de rapidité de transactions qui ne sont pas architecturés par blocs (comme le bitcoin) et a pour effet de réduire les frais de transactions. Mais ne reposant pas forcément sur une validation des transactions par le biais de la preuve de travail (blockchain), cela peut apporter des transactions conflictuelles puisqu’elles sont validées en parallèle sans que les mineurs ne soient au courant. Dans le cas d’une transaction conflictuelle (bug ou arnaque), les noeuds votent pour la transaction valide. Les cryptos basées sur les DAGs souhaitent briser le moule de la blockchain en améliorant les performances avec des ressources minimales et en évitant le [minage](glossaire.md#minage).
{% endhint %}

## Dark Pool

{% hint style="info" %}
C’est la face cachée du trading. Cette pratique permet à un acteur important dans une cryptomonnaie de réaliser une transaction anonyme sur une plateforme spécifique, sans que le reste du marché en soit aussitôt informé, dans le but d’éviter un inévitable mouvement baissier ou haussier sur le cours de la devise. Cela permet à cet acteur de nouer une grosse transaction à l’achat ou à la baisse sans que cela affecte la valeur de la cryptomonnaie en sa défaveur.
{% endhint %}

## Dapps (Applications Décentralisées)

{% hint style="info" %}
Les applications décentralisées sont des services fonctionnant sur une [blockchain](glossaire.md#blockchain) comme un site web, un service financier, un jeu vidéo, une marketplace, etc. Contrairement à leur antithèses centralisées, les applications décentralisées ne dépendent pas d’un seul et unique serveur, mais d’un réseau de machines. Cela leur permet d’être résilientes et insensibles à de nombreuses attaques, comme les attaques par dénis de service (DoS). Point important : cela leur permet également d’être résistantes à tout type de censure.

Prenons un exemple. Lorsque vous créez un site internet classique, celui-ci est hébergé sur un unique serveur. Si le serveur venait à avoir un quelconque problème, le site en question ne serait plus accessible. Dans le cas d’une application décentralisée, même si une machine venait à tomber en panne, l’exécution de l’application serait maintenue, car distribuée entre l’ensemble des machines du réseau.

Pour bien comprendre les avantages d’un application décentralisée, vous trouverez ci-après comment fonctionne une application centralisée :

Au début de l’ère informatique, les applications étaient systématiquement installées directement sur votre ordinateur. Il s’agissait par exemple de jeux, ou de programmes comme Microsoft Word. Par la suite, grâce à l’apparition d’Internet, il est devenu possible d’utiliser des applications à distance, sans que celles-ci n'aient à être installées sur votre machine. Mais avec cet avantage apparaissait un défaut majeur : chacune de ces applications était centralisée sur un serveur tiers.

Les problèmes de la centralisation :

* vos données personnelles ne vous appartiennent pas forcément. Par exemple, Facebook peut savoir avec précision quels sont vos centres d’intérêts, possède vos photos, sait à quel endroit vous voyagez grâce à la géolocalisation, connaît votre âge, etc. Confier autant de données personnelles à un tiers tel que Facebook est généralement une mauvaise idée, étant donné les risques de fuites d'informations, que ces fuites soient accidentelles ou non.
* leur mode de fonctionnement : une application centralisée utilisable par Internet doit être hébergée sur un ou des serveurs. Ces serveurs possèdent des adresses IP que l’on peut identifier pour ainsi remonter jusqu’à leur localisation, ou bien pour tenter de s'y introduire par le biais de failles informatiques. Si une personne avec de mauvaises intentions se décide à attaquer ces serveurs, alors l’application pourrait ne plus fonctionner.
* le propriétaire d'une application centralisée peut faire ce qu’il veut. Par exemple, il peut refuser qu’une personne utilise ses services, simplement parce que la personne en question a fait quelque chose qui ne lui plaît pas. Ce qui est déjà régulièrement le cas avec YouTube, qui peut décider qu’une vidéo véhiculant des idées politiques différentes des siennes ne soit pas admise sur son réseau.

C'est pour ces raisons qu'ont été imaginées les applications décentralisées.
{% endhint %}

## Day Trading

{% hint style="info" %}
C’est un trader qui fait des achats/ventes tous les jours contrairement à un investisseur sur le long terme qui achète et garde ([hodl](glossaire.md#hold)) sa cryptomonnaie pendant longtemps.
{% endhint %}

## DeFi (Decentralized Finance) ou finance décentralisée

{% hint style="info" %}
C’est une application des cryptomonnaies et des technologies blockchain. La principale cryptomonnaie impliquée dans la DeFI est [Ethereum](glossaire.md#ethereum). Cette dernière permet de créer de nombreuses applications financières comme Maker avec son token DAI et autre.

L’objectif de la finance décentralisée est de permettre la transmission de valeur et la création d’une finance pour tous et sans intermédiaire comme peuvent l’être les banques ou les plateformes d’échange.\
La DeFi permet à n’importe qui d’obtenir des prêts. C’est un système totalement décentralisés pour les emprunteurs et il n’est pas possible qu’un prêt vous soit refusé. Il vous suffit d’avoir un accès à internet.\
Cela permet également aux prêteurs de faire travailler leur argent avec des taux d’intérêts décents !

Plusieurs millions d'ethers sont ainsi mis en collatéral (bloqués) pour une valeur de plusieurs centaines de millions de dollars.
{% endhint %}

## DEX (échange décentralisé)

{% hint style="info" %}
Les DEX permettent des transactions directes (paire-à-paire) de crypto monnaies entre ses utilisateurs, de façon sécurisée et sans intermédiaire. Le DEX se contente de connecter deux utilisateurs désirant échanger leurs fonds directement depuis leurs portefeuilles. Cette caractéristique diminue ainsi les risques liés au piratage puisqu’il n’y a pas de fonds stockés sur des serveurs.
{% endhint %}

## Difficulty (difficulté)

{% hint style="info" %}
La difficulté de mining d’une cryptomonnaie comme le bitcoin permet d’évaluer la puissance et le temps nécessaires au [hashage](glossaire.md#hashage) de chaque bloc :

* C’est une unité de mesure utilisée au cours du procédé de mining,
* Elle permet d’évaluer la difficulté de la résolution d’un casse-tête cryptographique,
* La difficulté de miner de nouvelles unités augmente ou diminue dans le temps en fonction du nombre de mineurs sur le réseau,
* L’ajustement de la difficulté est nécessaire pour maintenir le « target block time » (le temps nécessaire à la création d’un bloc).

Plus une cryptomonnaie est populaire, comme le Bitcoin, plus le nombre d’ordinateurs participant au réseau pair-à-pair augmente. Les mineurs se livrent en compétition pour remporter des récompenses de bloc limitées. La difficulté de mining, ou simplement difficulté, désigne la puissance de **hashage** (le « hashpower ») de l’ensemble du réseau qui augmente en fonction du nombre de participants et de la puissance informatique en jeu.
{% endhint %}

## Digital signature (signature éléctronique)

{% hint style="info" %}
Une signature numérique est un mécanisme de cryptographie utilisé pour vérifier l’authenticité et l’intégrité de données numériques.

Un système de signature numérique se compose souvent de trois étapes de base : le hachage, la signature et la vérification.

1 - [Hachage](glossaire.md#hashage) des données

La première étape, c'est le hachage du message ou des données numériques. Ce dernier est réalisé en soumettant les données à travers un algorithme de **hachage** afin qu'une valeur de hachage soit générée (c'est-à-dire un résumé du message). Les messages peuvent varier de manière significative en taille, mais quand ils sont hachés, toutes leurs valeurs de hachage sont de même taille. C'est la propriété la plus fondamentale d'une fonction de hachage.

Cependant, le hachage des données n'est pas une condition obligatoire pour produire une signature numérique, puisque l'on peut utiliser une [clé privée](glossaire.md#cle-privee) pour signer un message sans que celui-ci n'ait été haché. Concernant les crypto-monnaies, les données sont systématiquement hachées car le fait de manipuler des empreintes dont la taille est fixe et invariable facilite le procédé.

2 - Signature

Après le hachage de l'information, l'expéditeur du message doit le signer. C'est le moment où la cryptographie à clé publique entre en jeu. Il existe plusieurs types d'algorithmes de signature numérique, chacun avec son propre mécanisme. Mais de manière générale, le message haché sera signé avec une clé privée, et le destinataire du message pourra ensuite vérifier sa validité en utilisant la clé publique correspondante (fournie par le signataire).

Autrement dit, si la clé privée n'est pas incluse lorsque la signature est générée, le destinataire du message ne sera pas en mesure d'utiliser la clé publique correspondante pour vérifier sa validité. Les clés publiques et privées sont générées par l'expéditeur du message, mais seule la clé publique est partagée avec le récepteur.

Il est important de noter que les signatures numériques sont directement liées au contenu de chaque message. Donc contrairement aux signatures manuscrites, qui tendent à être systématiquement les mêmes peut importe le message auquel elles sont rattachées, chaque message signé numériquement possédera une signature numérique différente.

3 - Vérification

Prenons un exemple pour illustrer l'ensemble du processus jusqu'à la dernière étape de vérification : Julie écrit un message à Paul, procède au hachage de celui-ci, et combine ensuite la valeur de hachage avec sa clé privée pour générer une signature numérique. La signature fonctionnera comme une empreinte numérique unique pour ce message particulier.

Quand Paul reçoit le message, il peut vérifier la validité de la signature numérique en utilisant la clé publique fournie par Julie. De cette façon, Paul peut être sûr que la signature a été créée par Julie, parce qu'elle est la seule à posséder la clé privée qui correspond à cette clé publique.

Ainsi il est crucial pour Julie de garder sa clé privée secrète. Si une autre personne met la main sur la clé privée de Julie, cette personne pourra créer des signatures numériques et prétendre être Julie. Dans le contexte de Bitcoin, cela signifie que quelqu'un pourrait utiliser la clé privée de Julie pour déplacer ou dépenser ses Bitcoins sans sa permission.

Pourquoi les signatures numériques sont-elles importantes?

Les signatures numériques sont souvent utilisées dans trois objectifs que leur propriétés permettent d'atteindre:

L'intégrité des données : Paul peut vérifier que le message de Julie n'a pas été modifié entre l'envoi et la réception. Toute modification du message produirait une signature complètement différente.

L’Authenticité : tant que la clé privée de Julie est gardée secrète, Paul peut se servir de sa clé publique pour confirmer que les signatures numériques ont été créées par Julie et personne d'autre.

Non-répudiation : une fois la signature générée, Julie ne pourra pas nier l'avoir appliqué à l'avenir, à moins que sa clé privée ne soit compromise d'une quelconque manière.
{% endhint %}

## Dildo

{% hint style="info" %}
Un **dildo** ou gode est une longue barre verte ou rouge située sur un graphique indiquant l'évolution du prix d'une **cryptomonnaie**, par rapport aux bougies verte et rouge trouvées sur les tableaux de prix.
{% endhint %}

## DLT (Distributed Ledger Technologies)

{% hint style="info" %}
Par définition, une technologie de registre distribué est simplement une base de données décentralisée gérée par plusieurs participants. Elle enregistre l’historique des transactions sur des nœuds de manière décentralisée. Chaque nœud valide et enregistre les transactions simultanément. Les enregistrements ont chacun un horodatage unique et doivent faire l’objet d’une signature cryptographique, gage de la sécurité et de l’incorruptibilité du réseau.

Chaque changement ou modification du registre doit faire l’objet d’un consensus des nœuds, qui doivent voter pour s’assurer de la sécurité et de la légitimité de chaque mise à jour.

Chaque transaction (représentée par un « bloc ») est liée à la suivante par un code et s’ajoute ainsi à la « chaîne de blocs » (le fameux « registre ») après avoir été vérifiée par les membres du réseau. Toute mise à jour des données se répercute alors sur l’ensemble du réseau de sorte que chaque utilisateur possède en permanence la dernière version de ces registres.

Une DLT n’est donc régie par aucune autorité centrale agissant comme un arbitre ou un gestionnaire. Ces registres distribués permettent de garantir une meilleure transparence, mais aussi une meilleure sécurité d’un réseau, plus compliqué à pirater qu’une base de données centralisée.

Une chaîne de blocs, ou blockchain, est un type particulier de DLT, dont l’un des grands mérites est d’avoir relancé l’engouement des chercheurs, des entrepreneurs et même du grand public autour des problématiques techniques liées aux DLT, qui n’étaient jusqu’alors dignes d’intérêt que pour une minorité de spécialistes acharnés.
{% endhint %}

## Double spending (double dépense)

{% hint style="info" %}
La double dépense est un acte frauduleux dans lequel le même jeton numérique est dépensé deux fois.

Comment empêcher la double dépense :

* Le hachage,
* La signature,
* La vérification.
{% endhint %}

## Dump

{% hint style="info" %}
Le dump est une chute soudaine et brutale du prix d’une cryptomonnaie et souvent suspecte (car souvent liée à une tentative de manipulation du marché).
{% endhint %}

## DYOR (Do your Own Research)

{% hint style="info" %}
En français, faites vos propres recherches.

Le mélange d’une jeune technologie et de beaucoup d’argent attire forcément les arnaqueurs.

Il existe de nombreuses arnaques à la cryptomonnaie, par exemple :

les arnaqueurs créent un faux profil ressemblant à celui d’une personnalité crypto très populaire et légitime, font une offre généreuse à la communauté crypto en reversant des cryptomonnaies « pour remercier les gens d’avoir cru en son projet », c’est le fameux « giveaway ». La manipulation est simple : il faut envoyer à telle adresse Ethereum un petit montant de la crypto et en échange, les donateurs vont en recevoir bien plus. Un joli cadeau qui, bien sûr, n’existe pas puisque l’arnaqueur n’est pas la personne qu’il prétend être. Une simple recherche internet avec les mots « giveaway Ethereum » leur aurait permis de trouver plusieurs articles mentionnant cette pratique comme étant frauduleuse.

Ainsi si vous cherchez à investir dans la cryptomonnaie, vous devez commencer par établir un plan et faire vos propres recherches :

Définir les monnaies et les biens numériques qui vous intéressent le plus —> chercher des informations sur ce que vous avez sélectionné auprès de sources indépendantes, ailleurs que sur le site web du projet lui-même.

Créer une liste d’objectifs d’investissements : à court, moyen ou long terme ?

* A court terme : consultez les graphiques des prix des devises cryptographiques plutôt que de lire la documentation relative au sujet mais assurez-vous que votre aptitude en tant que **Day-trader** est à la hauteur de la tâche.
* A moyen et long terme : moins risqués, ils conviennent mieux pour des objectifs d’investissement plus conservateurs. De plus, vous trouverez des informations, des sites, des graphiques, … plus fiables.
{% endhint %}

## ERC-20

{% hint style="info" %}
ERC pour Ethereum Request for Comments et 20 car c’est la vingtième proposition retenue pour sa création en novembre 2015. Ces jetons ont révolutionné le monde des [**ICO**](glossaire.md#ico-initial-coin-offering) et ont beaucoup contribué à leur développement. Il en existe plus de 20 000 différents en circulation.\
Un token ERC-20 n’est pas une nouvelle technologie mais une sorte de jeton avec des caractéristiques spécifiques. Il contient un registre avec différentes informations, c’est un standard. A partir du moment ou vous créez un jeton qui contient ces infos, il appartient à la norme ERC-20. Voici ses spécificités :

* Name : pour son nom
* Symbol : pour l’abréviation comme BTC pour Bitcoin
* Decimals : pour le nombre de décimales à utiliser
* TotalSupply : il indique le nombre total de jetons en circulation
* BalanceOf : informe du solde du compte contenant les tokens.
* Allowance : pour le nombre de jetons qui peuvent être retirés
* Transfer : comme son nom l’indique pour permettre de transférer des jetons
* Transferform : pour des transferts en passant par un compte externe
* Approve : permet de valider une opération

Il est devenu très utile pour lancer une ICO : avant les équipes devaient recoder une ‘base’ pour chaque projet. Désormais il suffit de prendre le modèle ERC-20 qui permettra une mise en place très rapide de l’ICO. C’est la norme la plus utilisée aujourd’hui et elle permet de diminuer les problèmes grâce à une complexité réduite.

Lors de sa création, les développeurs ont voulu créer quelque chose de très basique qui pourra être utilisé facilement et permettra à plus de personnes de développer des idées basées sur les crypto-monnaies.

Cependant il n’est pas parfait et des propositions ont vu le jour pour améliorer les défauts sur Github certaines ont été retenues. Une extension baptisée ERC223 propose d’implanter un filtre au coeur du mécanisme afin d’annuler toutes opérations d’envoi si l’adresse de réception ne gère pas la norme.

Stocker et mettre en sécurité vos jetons ERC-20 sur un [**portefeuille hardware**](glossaire.md#hardware-wallet) semble la méthode la plus sure pour garder ses jetons hors ligne et à l’abri des personnes malintentionnées.
{% endhint %}

## Escrow Bitcoin

{% hint style="info" %}
Le système Escrow Bitcoin a été développé pour augmenter la sécurité des paiements en Bitcoin.

C’est un système d’entiercement qui permet de bloquer ou de geler des fonds jusqu’à ce que les conditions de vente soient remplies à la satisfaction des deux parties participant à la transaction.

En utilisant le séquestre Bitcoin, l'utilisateur n'envoie pas BTC directement au vendeur, mais à une adresse d'entiercement spéciale. Il peut vérifier si les fonds ont été versés, mais ils sont bloqués jusqu'à ce que le client reçoive les marchandises conformément au contrat.

Cependant, ce n'est pas la seule application de ce système.

En cas de litige entre le consommateur et le vendeur, Bitcoin Escrow fournit un arbitre qui décide si l'acheteur doit être remboursé ou si le paiement doit être effectué au vendeur. Il s'agit d'un système analogue à celui utilisé dans le cas de PayPal. Il est actuellement utilisé par plusieurs plates-formes cryptographiques, notamment LocalBitcoin.
{% endhint %}

## ETF (Exchange Traded Fund)

{% hint style="info" %}
Les ETFs (Fonds Négociés en Bourse) sont des produits financiers qui répliquent les variations d’un indice, qu’il soit à la hausse ou à la baisse. Ces titres peuvent être achetés ou vendus en temps réel sur les marchés et leur valeur est corrélée à celle de leur indice sous-jacent ; ils sont aussi appelés crackers. Les ETFs donnent ainsi aux investisseurs un accès simple, direct et bon marché à l’investissement sur la totalité d’un indice boursier : on parle de gestion « passive » de portefeuille. Le panier d’actifs sous-jacent à l’ETF est généralement composé d’un ou plusieurs indices, de fonds divers concernant un ou plusieurs domaines, de matières premières, …

Le 11 février 2021, le Canada approuve la première création d’un fonds négocié en bourse (ETF) sur Bitcoin (BTC). Cet ETF est porté par Purpose Investments Inc, une société d’investissement.

En décembre 2020, le Canada avait déjà accepté un premier ETF basé sur l’éther (ETH). Nommé « The Ether Fund », il avait recueilli plus de 75 millions de dollars auprès d’investisseurs canadiens avant son lancement.
{% endhint %}

## Ether

{% hint style="info" %}
Unité de compte d’Ethereum dont le rôle principal n’est pas d’être une monnaie mais un carburant pour la plateforme.
{% endhint %}

## Ethereum

{% hint style="info" %}
La blockchain de Bitcoin a été conçue pour des applications monétaires alors qu’Ethereum permet de créer tout types d’applications. Ethereum, dont le code informatique est profondément différent de Bitcoin, vise plus à créer un nouveau web qu’une nouvelle monnaie. Il s’agit de 2 utilisations différentes et complémentaires des technologies blockchains.
{% endhint %}

## EVM (Ethereum Virtual Machine)

{% hint style="info" %}
A la manière des autres [blockchains](glossaire.md#blockchain), Ethereum permet l’interaction de nombreux noeuds sur lesquels fonctionnent des programmes.

La machine virtuelle d'Ethereum permet notamment deux principes :

1. de garantir la sécurité des programmes fonctionnant sur cette dernière (notamment contre les DDOS par exemple),
2. d’interpréter et de compiler ces programmes écrits en [**Solidity**](glossaire.md#solidity), permettant le fonctionnement de smarts-contracts. Elle garantit trois opérations cruciales pour le développement de [**smart-contract**](glossaire.md#smart-contract) et de [**DApp**](glossaire.md#dapps-applications-decentralisees) :
3. La validation des transactions, des signatures et des adresses de ces dernières.
4. Le calcul des frais des transactions.
5. La réalisation de ces différentes transactions.
{% endhint %}

## Fiat

{% hint style="danger" %}
Une monnaie fiat est une monnaie dont la valeur provient essentiellement du fait qu’un gouvernement impose son cours légal sur un territoire donné.\
Elle s'oppose historiquement aux monnaies-marchandises comme l'or, et se distinguent des cryptomonnaies qui tirent leur valeur de la confiance dans les systèmes crypto-économiques les soutenant. Les exemples les plus connus de monnaie fiat sont l'euro, le dollar étasunien, le yuan chinois et le yen japonais.

Le mot fiat est un mot latin signifiant « qu’il soit fait », qu'on retrouve notamment dans l'expression «fiat lux» (« que la lumière soit »). Il véhicule la notion d'une autorité qui décrète quelque chose et en anglais, le terme a été repris pour désigner un ordre ou un décret émanant d'un roi ou d'un président (« a royal fiat » par exemple). C'est donc de l'anglais que l'expression « monnaie fiat » nous vient : il s'agit en effet d'un calque direct du terme fiat money (ou fiat currency) qui est une devise d'échange établie par un fiat gouvernemental.

En France, c'est l'euro qui a cours légal, ou plus précisément sa forme liquide.
{% endhint %}

## FOMO (Fear Of Missing Out)

{% hint style="info" %}
Le FOMO (peur de manquer quelque chose) décrit la peur de rater une bonne affaire : une monnaie peut donc être achetée à n’importe quel prix et la valeur peut monter jusqu’à des prix très élevés avant de s’effondrer.
{% endhint %}

## Fork

{% hint style="info" %}
Tout logiciel nécessite des mises à jour constantes pour résoudre des problèmes qu’il rencontre ou améliorer ses performances. Dans le monde de la cryptomonnaie, ces mises à jour s’appellent des « forks ».

Ce mot anglais est utilisé pour désigner un embranchement, c'est-à-dire une division en plusieurs branches. Au niveau de la blockchain, il désigne une division de la chaîne de blocs en deux chaînes distinctes.

Le registre utilisé par une crypto-monnaie est, en règle générale, une chaîne de blocs. Chaque bloc est un ensemble horodaté de transactions, qui est validé en étant ajouté à la chaîne. Chaque bloc est lié au bloc précédent grâce à l'action d'un validateur.

Dans le cas de Bitcoin, la validation a lieu par le calcul d'[une preuve de travail](glossaire.md#pow-proof-of-work-preuve-de-travail) pour un [mineur](glossaire.md#mineur) : pour rattacher le bloc au bloc précédent, le mineur doit prouver qu'il a dépensé de l'énergie en trouvant la solution à un problème mathématique lié au contexte. Le mineur partage ensuite son bloc avec les noeuds du réseau qui le vérifient.

Cependant, rien n'interdit à un mineur d'ignorer un bloc, et de rattacher son bloc à la suite d'un bloc antérieur : cela crée ce qu'on appelle un fork ou embranchement de la chaîne. Ce fork peut être tout à fait bénin : si deux mineurs trouvent chacun un bloc dans un intervalle de temps réduit, alors ils diffusent leur solution tous les deux au même moment, et ceci en toute bonne foi. Mais il peut aussi être provoqué par un acteur malveillant voulant censurer une transaction contenue dans le dernier bloc.

Dans les deux cas, cela crée un conflit sur le réseau, car les deux blocs sont valides aux yeux du protocole. Il faut donc faire en sorte de les départager.

Les forks et le consensus : les forks communs sont résolus grâce à une règle simple, énoncée par Satoshi Nakamoto dans le livre blanc de Bitcoin : la chaîne la plus longue (c'est-à-dire celle qui a le plus de travail accumulé) est la chaîne qui doit être sélectionnée par le réseau.

Ainsi, s'il y a un conflit entre deux chaînes de même longueur, ce conflit est résolu dès qu'un nouveau bloc est trouvé. La chaîne la plus longue (qui est généralement celle qui contient le plus de blocs) est acceptée comme valide par le réseau.

Comme un fork est basé sur la blockchain d'origine, toutes les transactions de la blockchain d'origine sont également copiées dans le nouveau fork. Par exemple, si vous avez 100 pièces d’une crypto-monnaie appelée Coin A et qu’un « hard fork » basé sur cette crypto-monnaie crée une nouvelle crypto-monnaie appelée Coin B, vous obtiendrez également 100 pièces du Coin B.

En raison de la nature open source de la crypto-monnaie et de la multiplication du nombre d'individus et d'organisations ayant des objectifs différents au sein de la cryptosphère, les forks continueront de faire partie intégrante du développement de la crypto-monnaie.
{% endhint %}

## FUD (Fear Uncertainty and Doubt)

{% hint style="info" %}
Terme visant à semer la peur, l’incertitude et le doute afin d’inciter les investisseurs à vendre leurs valeurs pour faire baisser le cours d’une cryptomonnaie.
{% endhint %}

## Futures

{% hint style="info" %}
Les futures sur cryptomonnaie sont des contrats dérivés dits à terme qui obligent les parties prenantes à trader la cryptomonnaie sous-jacente à une date et un prix déterminés à l’avance.

Les futures permettent de bloquer le prix de l’actif à l’avance. En plus du prix, le trader connait la date d’expiration du contrat à l’avance. Il s’agit habituellement d’un mois d’expiration.

Il existe deux catégories principales d’investisseurs qui utilisent les futures : les **hedgers** et les spéculateurs.

Les hedgers sont des investisseurs qui détiennent déjà l’actif financier sous-jacent et qui utilisent la technique du hedging pour se protéger de changements de prix défavorables. En effet, ils vont acheter ou vendre des contrats à terme pour compenser le risque de pertes potentielles.

Les spéculateurs sont simplement des traders qui veulent faire des profits en spéculant sur la direction d’un actif. Si un trader achète un contrat à terme sur le Bitcoin et que le prix du BTC augmente au-dessus du prix du contrat à l’expiration, alors il pourra réaliser un bénéfice.

Avantages d’utiliser des contrats à terme

* Faible barrière à l’entrée ;
* Outil de spéculation ou de protection ;
* Utilisation d’un effet de levier et de la marge qui réduit le montant du contrat ;
* Règlement du contrat possible en cash ;
* Portefeuille non nécessaire si le règlement se fait en numéraire ;
* Utilisation d’exchanges américains réglementés par la Commodity Futures Trading Commission (CFTC) ;
* Tous les éléments du contrat sont connus à l’avance ;
* Possibilité de profiter d'un mouvement haussier ou d'un mouvement baissier ;
* Les contrats à terme sur le Bitcoin ne peuvent pas être piratés ou volés comme peuvent l'être les BTC.

Risques d’utiliser des contrats à terme

* Indisponibilité de certains types d’ordre de trading en fonction de l'exchange utilisé ;
* Pas de trading du vendredi après-midi aux dimanche matin (USA sur le CME Group par exemple) ;
* Pas de fractionnement des contrats possible ;
* Danger lié au trading sur marge et à l'utilisation de l'effet de levier ;
* Possibilité de faire perdre des opportunités à un trader qui n’utilise que des contrats à terme.

Conclusion

Bien que les futures sur Bitcoin soient des produits d’investissement intéressants dans une stratégie de couverture (hegding) ou de spéculation, il est important de rappeler que le Bitcoin est un produit non réglementé dans la plupart des juridictions.

Les futures sur Bitcoin sont aussi des produits relativement nouveaux qui sont sujets à l’extrême volatilité du cours du Bitcoin. Ainsi, ils peuvent ne pas convenir à tous les types d'investisseurs.
{% endhint %}

## ICO (Initial Coin Offering)

{% hint style="info" %}
Une ICO est une méthode de levée de fonds durant la phase de démarrage d’un projet. Pour investir, l’internaute doit posséder de la cryptomonnaie qu’il échange contre des tokens émis par l’organisation à l’origine de l’ICO. Acheter ces tokens ne représentent pas des parts de l’entreprise, à la différence d’actions, mais revient en fait à pré-payer le produit ou le service appelé à être développé. Deux principaux objectifs expliquent les mises des investisseurs dans les ICO : une objectif spéculatif (valeur token à la revente) et un objectif utilitaire (valeur token dans le cadre du projet financé). Le risque de cet investissement : l’équipe organisatrice part avec les fonds.
{% endhint %}

## IEO (Initial Exchange Offereing)

{% hint style="info" %}
Contrairement à l’ICO, ce n’est pas une équipe mais une plateforme qui effectue la levée de fonds. En passant par une place de marché à la réputation établie, le projet génère confiance (la plateforme prendrait un risque de réputation à promouvoir un projet que ne serait pas sérieux ou une arnaque) et visibilité car la plateforme en fait la proposition à tous ses clients.
{% endhint %}

## Gas

{% hint style="info" %}
Le gas, que l’on peut traduire en français par gaz ou essence est une unité virtuelle présente dans Ethereum qui permet d’organiser le paiement des frais de transaction.

Ethereum est semblable à un ordinateur mondial décentralisé permettant d’exécuter des programmes appelés [**smart contract**](glossaire.md#smart-contract)**s**. Il repose sur une machine virtuelle appelée [**EVM**](glossaire.md#evm-ethereum-virtual-machine) qui fonctionne simultanément sur chacun des noeuds d’un réseau pair à pair.

Ainsi, chacun des ordinateurs connectés au réseau Ethereum exécute toutes les opérations traitées par le système. Les opérations sont incluses dans les transactions. Afin d'empêcher les attaques par déni de service, ces opérations demandent des frais, frais qui sont payés grâce au système du gaz.

Les intérêt du gas sont multiples :

1. En tant que système imposant aux transactions de payer des frais, il permet de limiter les attaques par déni de service : afin de paralyser le réseau avec un grand nombre de transactions, un attaquant devrait en effet dépenser beaucoup d'argent. De plus, en faisant cela, il ferait monter le niveau général des frais, et ne pourrait pas soutenir son attaque sur une longue période de temps.
2. Le gaz permet de décorréler les coûts de fonctionnement du réseau Ethereum du prix de l'éther. Contrairement au système des frais de transactions sur Bitcoin qui sont mesurés par rapport au poids d'une transaction (en satoshis par octet virtuel), le modèle Ethereum est de donner un coût fixe à chaque opération de sorte à avoir une estimation aussi réaliste que possible du traitement réalisé par les nœuds.
3. Grâce à la limite de gaz, ce modèle permet d'avoir une machine virtuelle pouvant faire marcher des programmes généralistes tout en arrêtant les boucles infinies.
{% endhint %}

## Gas Cost (Cout du gaz)

{% hint style="info" %}
Le [gas](glossaire.md#gas) est une unité dans Ethereum qui sert d'intermédiaire entre l'utilisateur qui réalise une transaction et le validateur (mineur) qui confirme cette transaction. Le gaz est entièrement virtuel et personne ne peut en détenir ou en échanger : l'utilisateur paie les frais en éthers (ETH) et le validateur récupère également ces frais en éthers.

Le gaz est « acheté » (en éthers) au moment de la validation de la transaction, puis il est « consommé » comme carburant pour la machine virtuelle. Le validateur qui inclut la transaction dans son bloc récupère l'éther utilisé pour acheter le gaz.

Chaque opération dans Ethereum a un **coût fixe** en gaz. Celui-ci est calculé en fonction de la ressource en calcul nécessaire par rapport aux autres opérations.

Un transfert d'éther (ETH) entre deux comptes consomme ainsi toujours **21 000 gaz**. Du côté de l'exécution des smart contracts, chaque opération a son coût propre.
{% endhint %}

## Gas Limit

{% hint style="info" %}
Lorsqu'un contrat est exécuté par la machine virtuelle d'Ethereum, il consomme du gaz. Lorsqu'il ne dispose plus de gaz, il arrête de fonctionner.

Il existe donc un paramètre de la transaction, la limite de gaz ou gas limit, qui correspond à la quantité maximale de gaz que l'utilisateur est prêt à utiliser.

Puisque les contrats peuvent s'appeler les uns les autres, il est en effet souvent très difficile de savoir à l'avance combien de gaz va consommer une transaction : il faut l'estimer.

Trois situations peuvent se présenter :

* L'utilisateur indique une limite trop basse. L'exécution se fait mais ne peut pas aller au bout, la transaction est donc invalidée mais les frais sont conservés par le validateur.
* L'utilisateur estime correctement le coût en gaz et indique une limite égale. Ce cas de figure arrive régulièrement lorsqu'il s'agit d'effectuer un transfert d'éthers entre deux comptes : cela ne sert à rien d'indiquer une limite de gaz autre que 21 000 puisque le coût est fixe.
* L'utilisateur communique une limite de gaz trop haute. Dans ce cas, tout se passe comme prévu et le gaz inutilisé est \*\*\*\*remboursé (en ETH) à l'utilisateur. C'est pour cela qu'il est conseillé, lorsqu'on ignore combien de gaz va consommer notre transaction, de mettre une limite haute.

Calculer la bonne limite de gaz pour une transaction :

Pour un transfert d'éther, le coût en gaz est de 21 000. Vous n'avez donc pas à changer la limite de gaz : en effet, même si vous indiquez une limite de, disons, 50 000, les 29 000 gaz non consommés vous sont remboursés.

Pour un transfert de jetons [**ERC-20**](glossaire.md#erc-20), le coût en gaz peut varier, allant de 25 000 à 150 000 gaz. Les portefeuilles règlent généralement ce paramètre de manière automatique. Si jamais il arrive que ce ne soit pas le cas, n'hésitez pas à indiquer une limite de gaz haute : le montant non consommé vous sera renvoyé.

Pour une interaction avec un smart contract, comme celui gérant une [**ICO**](glossaire.md#ico-initial-coin-offering) par exemple, le coût en gaz n'est pas toujours connu à l'avance. Veillez bien à vous renseigner auprès des développeurs du smart contract qui indiquent généralement ce genre de chose dans leurs communiqués officiels.
{% endhint %}

## Gas Price

{% hint style="info" %}
Le prix du gas est le second paramètre à spécifier lors de l'envoi d'une transaction. Comme son nom l'indique, il s'agit du prix en éthers auquel l'utilisateur achète le gaz.

Le prix du gas est généralement exprimé en gigaweis (Gwei). Le wei est à Ethereum ce que le satoshi est à Bitcoin : il s'agit de la plus petite sous-unité de l'éther, étant égale à un attoéther soit 10-18 ETH. Un Gwei correspond à un milliardième d'éther. En résumé :

1 ETH = 1 000 000 000 Gweis

```
       = 1 000 000 000 000 000 000 weis
```

Le prix du gas permet d'augmenter les frais payés par une transaction, et donc la priorité avec laquelle elle sera traitée par les validateurs (mineurs). En effet, puisqu'un bloc est limité à une certaine quantité de gaz consommé (12,5 millions de gaz en juillet 2020), celui-ci ne peut pas accueillir toutes les transactions en attente, et les validateurs sélectionnent les transactions les plus rentables en priorité.

Les frais payés sont calculés par la formule :

frais (Gwei) = coût en gaz (gaz consommé) × prix du gaz (Gwei)

Par exemple, pour une transaction classique (21 000 gaz consommés) et un prix du gaz de 30 Gwei, les frais seront de 630 000 Gweis c'est-à-dire 0,00063 ETH, soit 17 centimes d'euro au prix actuel (juillet 2020).

Estimer le prix du gaz correctement

Le prix du gas (mesuré en Gwei) est la manière dont l'utilisateur modifie le niveau de frais payés par sa transaction, et par conséquent la priorité avec laquelle celle-ci va être traitée par le réseau. Plus vous serez pressé, plus vous aurez à augmenter ce paramètre pour que votre transaction passe avant les autres. Cela peut se révéler crucial lors des [ICO](glossaire.md#ico-initial-coin-offering) populaires qui ne durent que peu de temps.

Bien souvent, votre portefeuille estime directement le montant des frais, et peut vous proposer des alternatives pour que vous choisissiez le montant correspondant à votre usage.

Si vous désirez calculer vous-même le prix optimal, il existe un site web donnant une estimation du temps d'attente selon le niveau de prix : ETH Gas Station. Sur la page principale du site, vous aurez trois indications de prix :

* **Safe Low** : le nombre minimum de Gwei pour que la transaction soit confirmée en moins de 30 minutes.
* **Standard** : le nombre minimum de Gwei pour que la transaction soit confirmée en moins de 5 minutes.
* **Fast** : le nombre minimum de Gwei pour que la transaction soit confirmée en moins de 2 minutes.

Le prix que vous indiquerez dépendra de votre **préférence** : désirez-vous économiser en frais de transaction quitte à attendre plus longtemps, ou voulez-vous que votre transaction soit confirmée très vite, quitte à payer beaucoup de frais ?
{% endhint %}

## Genesis Block

{% hint style="info" %}
Il s'agit du premier bloc d'une [blockchain](glossaire.md#blockchain). Techniquement parlant, il s'agit d'un bloc particulier. Il n'a aucune référence vers un bloc précédent, une singularité sans réelles conséquences. Si aujourd'hui il est déterminé comme le bloc n°0, les premières versions de Bitcoin le considéraient comme le bloc n°1.

Ce premier bloc ne contient aucune transaction. Néanmoins il est possible d'écrire tout type de données dans un bloc, tant que l'on en paye le coût. Ainsi, ce bloc est composé d'une phrase, ou plutôt le titre d'un article du Financial Times du 3 janvier 2009 :

Chancellor on brink of second bailout for banks (Chancelier sur le point du 2ème sauvetage des banques)
{% endhint %}

## Halving

{% hint style="info" %}
Un halving est un évènement périodique qui se produit sur une [blockchain](glossaire.md#blockchain) et qui a pour but de diviser par deux les récompenses attribuées aux mineurs.

De nouveaux bitcoins sont émis par le réseau Bitcoin toutes les 10 minutes et sont attribués aux [**mineurs**](glossaire.md#mineur) en échange du travail qu’ils fournissent pour sécuriser le système. Cette émission est divisée par deux tous les 210 000 blocs de transactions, soit tous les quatre ans environ :

* Montant récompense de 2009 à 2012 : 50 BTC (soit 10,5 millions de bitcoins),
* Montant récompense de 2012 à 2016 : 25 BTC le 28 novembre 2012 (soit 5,25 millions de bitcoins),
* Montant récompense de 2016 à 2020 : 12,5 BTC le 9 juillet 2016 (soit 2,625 millions de bitcoins),
* Montant récompense le 11 mai 2020 : 6,25 BTC.
{% endhint %}

## Hard Fork

{% hint style="info" %}
Un « Hard Fork » est une modification d'un protocole d'une crypto-monnaie qui deviendra incompatible avec les versions précédentes, ce qui signifie que les [nœuds](glossaire.md#node-noeud) qui ne se mettent pas à jour vers la nouvelle version ne pourront pas traiter les transactions, ni insérer de nouveaux blocs dans la chaîne de blocs.

Les « hard forks » peuvent être utilisées pour modifier ou améliorer un protocole existant, ou même pour créer un nouveau protocole et une nouvelle chaîne de blocs indépendants.

Imaginez un changement de protocole qui augmente la taille des blocs de 2 Mo à 4 Mo. Si un nœud mis à jour tente de placer un bloc de 3 Mo dans la blockchain, les nœuds plus anciens, et non mis à jour, ne verront pas ce bloc comme valide et ils le rejetteront.

Les « hard forks » peuvent être planifiés ou controversés :

* Dans un « fork » planifié, les participants mettront volontairement à niveau leur logiciel afin de suivre les nouvelles règles, en délaissant l’ancienne version. Ceux qui ne se mettent pas à jour restent alors à miner dans l'ancienne chaîne, que très peu de gens utiliseront.
* Mais si le « fork » est controversé, ce qui signifie qu’il y a un désaccord au sein de la communauté au sujet de la mise à niveau, le protocole est généralement divisé en 2 chaînes de blocs incompatibles - 2 crypto-monnaies différentes. Les deux blockchains auront leur propre communauté et de chaque côté les développeurs avanceront de la manière qu'ils jugent être la meilleure.
{% endhint %}

## Hardware

{% hint style="info" %}
Le terme hardware est utilisé pour désigner le matériel tangible comme la carte mère, le processeur, l'unité centrale, … tandis que le software désigne comme son nom l'indique un matériel virtuel : un logiciel ou une application.
{% endhint %}

## Hardware Wallet

{% hint style="info" %}
Un portefeuille hardware est une des manières les plus sûres de gérer vos crypto-monnaies. Ce qui rend cette sorte de portefeuille très sécurisée est que l’accès à vos crypto-monnaies est cryptée à travers l’appareil. Cela le rend plus sécurisé qu’un portefeuille online.
{% endhint %}

## Hashage

{% hint style="info" %}
Les fonctions de hachage (hash functions en anglais) sont des suites d’opérations mathématiques et cryptographiques produisant un résultat que l’on appelle empreinte ou **signature**. Elles servent généralement à sécuriser un transfert d’informations entre deux systèmes informatiques.

Les fonctions de hachage sont donc censées répondre à plusieurs critères précis :

* Le déterminisme : le résultat de la fonction doit être invariable en toutes circonstances. Quel que soit le moment où la fonction est utilisée, la personne qui s’en sert ou la quantité de fois que la fonction est utilisée, si le message de départ est le même, alors le résultat doit être le même.
* L’efficacité : la fonction de hachage doit permettre d’obtenir un résultat immédiat, autrement elle risque de ralentir de manière excessive les systèmes informatiques qui en dépendent.
* La résistance aux attaques : il ne doit pas être possible de recréer le message d’origine à partir du résultat de la fonction, sauf en essayant tous les résultats possibles un par un.
* L’aisance de distinction : deux messages extrêmement similaires doivent générer deux résultats facilement différenciés.
* L’unicité des résultats : il doit être impossible de générer deux résultats identiques avec deux messages différents.
{% endhint %}

## Head and Shoulder

{% hint style="danger" %}
Formation graphique représenté comme une ligne à trois pics. Les deux extérieurs sont proches en hauteur et celui-ci milieu sont plus élevé. De façon plus technique, une configuration head and shoulders est la description, d’une formation graphique spécifique qui prédit un renversement de tendance haussier à baissier.

Head and shoulders est considérée comme l'une des figures de renversement de tendance les plus fiables. C'est l'une des nombreuses figures de sommet qui signalent, avec plus ou moins de précision, qu'une tendance à la hausse touche à sa fin.
{% endhint %}

## Hedger

{% hint style="info" %}
Terme anglo-saxon désignant le fait de chercher à se couvrir contre un risque non anticipé.

Les stratégies d’hedge permettent aux traders d'utiliser plus d'un pari simultané dans des directions opposées pour minimiser le risque de pertes conséquentes.

C’est une stratégie du marché financier comme une forme de technique de gestion des risques pour les traders crypto. Elle vous permet de maintenir une valeur stable pour vos investissements (sans réaliser un rendement considérable) dans des conditions de marché indésirables.
{% endhint %}

## Hold

{% hint style="info" %}
Hold signifie conserver sa cryptomonnaie. Quand le marché est agité, il y a donc ceux qui hold et ceux qui revendent, soit parce-qu’ils savent ce qu’ils font, soit parce-que ce sont des [**weak hands**](glossaire.md#weak-hands)**.**
{% endhint %}

## Impermanent Loss (pertes intermittentes)

{% hint style="info" %}
L’impermanent loss est une perte temporaire de fonds qui peut se produire lorsque vous déposez vos actifs sur une plateforme [**DeFi**](glossaire.md#defi-decentralized-finance-ou-finance-decentralisee) comme liquidité pour une [**liquidity pool**](glossaire.md#liquidity-pool-reserve-de-liquidite).

La valeur de vos actifs peut changer avec le temps. En conséquence, vous subissez une perte intermittente car la conception des [**AMM**](glossaire.md#amm-automated-market-maker) l'a fait ainsi.

Certaines piscines ont une perte moins intermittente. Elles sont destinées à échanger des jetons dont la valeur est limitée. Les Stablecoins sont de bons exemples ici. Leur valeur ne change pas et les fournisseurs de liquidité ont l'esprit tranquille en ce qui concerne la perte intermittente.

Une perte intermittente n'est pas quelque chose qui empêche de fournir des liquidités sur les plates-formes DeFi. Les frais de négociation que les plateformes offrent aux [fournisseurs de liquidité (LP)](glossaire.md#liquidity-provider) compensent d'une manière ou d'une autre la perte intermittente. Tout dépend de l'algorithme de la plateforme DeFi.

Les fournisseurs de liquidités doivent être conscients des risques de pertes intermittentes qui se produisent, que le changement de prix soit positif ou négatif. De nombreuses procédures des plates-formes DeFi tentent d'atténuer les risques, mais certaines pools ont une perte intermittente importante et ne conviennent qu'aux traders expérimentés.

Le calcul de la perte diffère selon les plateformes DeFI. Il est basé sur le protocole, les algorithmes et les jetons.

Pour compenser les risques il vaut mieux commencer à fournir des liquidités avec des petits montants et ne pas déposer tous ses avoirs sur une plateforme DeFI et un pool de liquidités. Vous pouvez ensuite estimer le montant de la perte et décider d’augmenter ou de réduire vos avoirs.

Comment éviter les pertes intermittentes ?

* Regarder les offres de frais de négociation des plateformes qui peuvent être des escroqueries ou ne pas avoir le protocole de sécurité requis pour compenser les pertes,
* Fournir des liquidités aux pools de monnaies stables
* Participer à des programmes d'extraction de liquidité. Certaines plateformes DeFi ont des programmes d'extraction de liquidité qui compensent votre perte intermittente.
* Gardez la liquidité jusqu'à ce que les taux reviennent au taux initial
* Éviter les paires de crypto-monnaie volatiles
* Fournir des liquidités aux pools avec des crypto-monnaies pondérées de manière inégale.

Vos pertes restent intermittentes (et non permanentes) si vous ne retirez pas vos actifs de la plateforme.
{% endhint %}

## Inflation

{% hint style="info" %}
L’inflation est une augmentation du prix des biens et des services dans une économie donnée et sur une période donnée.

Plusieurs conditions définissent l’inflation :

* La hausse des prix doit être soutenue et ne pas être un évènement isolé,
* Elle implique une augmentation de presque tous les éléments de l’économie,
* Elle est basée sur le long terme.

Les causes :

* L’augmentation rapide de la quantité d’une devise en circulation (les réserves),
* Une pénurie d’offre d’un bien spécifique et très demandé qui peut entrainer une hausse du prix de ce bien et se répercuter sur le reste de l’économie.

Les aspects positifs de l’inflation :

* elle peut stimuler l’économie car plus d’argent circule, il y a plus d’argent à dépenser, ce qui crée plus de demande. Cela stimule la production, réduit le chômage et injecte plus d’argent dans l’ensemble de l’économie,
* Elle peut inciter les consommateurs à acheter des biens et des services rapidement avant que les prix n’augmentent davantage.

Les aspects négatifs de l’inflation :

* Elle touche les personnes les plus vulnérables, les personnes sans ressources et les personnes âgées, réduit les revenus réels de la classe ouvrière,
* Elle réduit la valeur de l’épargne et les taux d’intérêts augmentent.

Alors que les gouvernements nationaux tentent de contrôler l’inflation, Bitcoin est considéré par beaucoup comme une protection efficace contre les ravages de l’inflation. Ceci s’explique par le fait que Bitcoin possède une réserve totale fixe de 21 millions de pièces. Malgré certaines controverses, beaucoup pensent que cela fait de Bitcoin une monnaie déflationniste, et donc, résistante à l'inflation.
{% endhint %}

## KYC (Know Your Customer)

{% hint style="info" %}
Le KYC (ou connaissance de la clientèle) est aujourd’hui obligatoire dans tous les exchanges réputés et le nombre d’exchanges sans KYC diminue rapidement. Fini le temps ou une simple adresse mail suffisait pour s’enregistrer sur la plupart des plateformes.

Les leaders des exchanges internationaux ont incorporé des mesures de vérification d’identité dans leur plateforme afin de protéger les investisseurs.

Les petits traders qui déposaient et retiraient que quelques centaines de dollars par mois n’ont pas été affectés. Alors que pour les traders et les whales (les gros portefeuilles), ils n'ont eu d’autres choix que de s’identifier au moyen de procédures KYC standards en ligne comme c’est le cas dans les sociétés de courtage.
{% endhint %}

## Lending

{% hint style="info" %}
Le lending consiste à prêter des cryptomonnaies durant une certaine période. Ce prêt peut être à vue ou à terme fixe et impose un blocage des cryptomonnaies durant toute la durée du prêt.

Le rendement du lending est la plupart du temps calculé de manière « annualisé ». On trouve des prêts de cryptomonnaies rémunérés à seulement quelques dixièmes de pour cent (ex : 0,30% annuel) jusqu’à plus de 15 ou 20%. Ce rendement dépend de la durée du prêt et de la crypto-monnaies prêtée. Plus la durée du prêt est longue et la cryptomonnaie prêtée est rare (demandée), plus le rendement du lending sera important pour l’investisseur ayant souscrit à l’offre de lending.

A l’inverse du lending, les investisseurs ont désormais également la possibilité d’emprunter des cryptomonnaies et paye par conséquent des intérêts pour cet emprunt. Pour exemple, les traders effectuant du trading avec marge (« margin ») empruntent des cryptomonnaies à la plateforme d’échanges afin de profiter d’effet de levier. Ces traders utilisent donc une ligne de crédit en crypto-monnaie.
{% endhint %}

## Leverage (effet de levier)

{% hint style="danger" %}
L’effet de levier est une technique de **margin-trading**. Le levier est synonyme de multiplicateur. Il consiste à emprunter des capitaux à la plateforme d’échange qui va vous prêter des liquidités pour augmenter la taille de vos positions. Ainsi si vous avez mis 100€ en levier x 5 cela équivaut à avoir une position de 500€. Un levier est dangereux, bien que vos gains peuvent être multipliés, il en est de même pour vos pertes, soyez vigilants.\
Dans le cas où la valeur de la perte est équivalente à la valeur de l'investissement initial, la position est alors "liquidée". C'est-à-dire que votre position est vendue et que vous perdez votre investissement.
{% endhint %}

## Lightning Network

{% hint style="info" %}
Le lightning network est une technologie qui se présente comme un réseaux de canaux de paiements ou tous les hôtes sont connectés pair à pair sans hiérarchie centrale, formant une structure en forme de filet. Chaque noeud peut donc recevoir, envoyer et relayer les transactions.

Les avantages du Lightning Network sont:

1. Aucune limite sur le nombre de transactions par seconde sur le réseau,
2. Des transactions instantanées d’un bout à l’autre du monde. Plus d’attente de confirmation par les mineurs,
3. Des frais de transaction extrêmement faibles ouvrant la voie aux micro-transactions.

Ces nouvelles caractéristiques sont une amélioration conséquente à ce que Bitcoin propose déjà.

La naissance d’un système d’échanges illimités et instantanés va permettre à Bitcoin de se développer comme un réel moyen de paiement supranational et adoptable par tout un chacun.
{% endhint %}

## Limit Buy / Limit Sell

{% hint style="info" %}
Ordre d’achat placé par un investisseur qui souhaite acheter/vendre des cryptomonnaies à un prix fixé à l’avance.
{% endhint %}

## Liquidity (Liquidité)

{% hint style="info" %}
Le terme liquidité est défini comme la capacité d'acheter ou de vendre des actifs sur le marché sans provoquer de changement radical du prix des actifs.

Le terme de liquidité peut faire référence à deux domaines différents :

1. La liquidité d'un marché qui désigne le fait qu'il y a en permanence sur ce marché des investisseurs disposés à réaliser des transactions de commerce(trading).
2. La liquidité d'un actif qui désigne le fait que ce dernier peut facilement être converti en espèces— également appelées argent liquide.

Pour pouvoir vendre et acheter rapidement des[ jetons](glossaire.md#token-jeton) (tokens), sans qu’il soit nécessaire de faire fluctuer le prix ou d’attendre trop longtemps pour trouver un ordre correspondant, le marché sur lequel vous êtes doit être liquide.

En d'autres termes, il se doit d'y avoir une activité commerciale intense et les prix acheteurs/vendeurs ne doivent pas être trop écartés les uns des autres en valeur.
{% endhint %}

## Liquidity Pool (Réserve de Liquidité)

{% hint style="info" %}
Les Liquidity Pool sont des réserves de jetons bloqués dans un [**smart contract**](glossaire.md#smart-contract).

Leurs utilités :

* dans des protocoles d’échanges décentralisés (DEXs) comme Uniswap ou Balancer,
* dans des protocoles de prêts ([**lending**](glossaire.md#lending)) comme Compound ou Aave.

Leurs utilisateurs :

* les fournisseurs de liquidités qui déposent des jetons dans la réserve en échange d’une récompense (frais, intérêts, …) et
* les utilisateurs pour effecteur diverses actions telles que des échanges ou encore des emprunts.

Les Liquidity Pool assurent la présence de liquidité, en tout temps, dans le protocole.

Bien que le concept en lui-même ne soit pas particulièrement compliqué, il fait office de révolution dans l’écosystème de la finance décentralisée.
{% endhint %}

## Liquidity Provider

{% hint style="info" %}
Les personnes qui apportent la liquidité
{% endhint %}

## Litecoin

{% hint style="info" %}
Le litecoin (version modifiée du bitcoin) vise à proposer des frais et des délais de transaction réduits par rapport à ceux du bitcoin.
{% endhint %}

## Long

{% hint style="info" %}
Faire un long consiste à miser à la hausse du cours en utilisant le **margin trading.** C’est à dire emprunter de l’argent à un instant T, en espérant que le prix augmente afin de rembourser les montants empruntés tout en dégageant un profit.
{% endhint %}

## Margin Call

{% hint style="info" %}
Le trading sur marge est une méthode de négociation d'actifs à l'aide de fonds fournis par un tiers. Comparés aux comptes de trading ordinaires, les comptes sur marge permettent aux traders d’accéder à des sommes de capital plus importantes, et ainsi d’appliquer un effet de levier à leurs positions. Toutefois, cette méthode de négociation peut également amplifier les pertes et comporter des risques beaucoup plus élevés. Ainsi, elle n’est implicitement réservée qu’aux traders hautement qualifiés.
{% endhint %}

## Margin Trading

{% hint style="info" %}
C’est une méthode risquée qui consiste à emprunter de l’argent pour faire du trading.
{% endhint %}

## Market Buy

{% hint style="info" %}
Il s’agit de l’ordre d’achat au meilleur prix du marché au moment de l’achat.
{% endhint %}

## Market Sell

{% hint style="info" %}
Il s’agit de l’ordre de vente au meilleur prix du marché au moment de la vente.
{% endhint %}

## Market Cap

{% hint style="info" %}
Le market cap ou capitalisation de marché est un indicateur qui permet de mesurer et suivre la valeur d’un crypto-actif.

Market cap = prix de la monnaie x quantité en circulation (CIRCULATING SUPPLY)
{% endhint %}

## Market Makers

{% hint style="info" %}
Ce sont des acteurs du marché assurant que chaque ordre soit complété en apportant des liquidités propres, espérant profiter du spread (différence entre prix de vente et d’achat) sur un marché donné. Ce sont ces market makers qui permettent d’assurer la liquidité et l’utilisabilité d’un échange.
{% endhint %}

## Mempool

{% hint style="info" %}
Le mempool Bitcoin est le pool de transactions Bitcoin non confirmées sur le réseau. Une fois qu’une transaction Bitcoin est effectuée sur la blockchain, elle n’est pas immédiatement ajoutée ; elle va plutôt dans ce pool de transactions en attente de procès.
{% endhint %}

## Minage

{% hint style="info" %}
Le minage techniquement surnommé [« Proof of work » (preuve de travail) ](glossaire.md#pow-proof-of-work-preuve-de-travail)permet de sécuriser la blockchain. Le système de minage a été pensé de manière à ce que n’importe qui sur la planète puisse devenir un mineur et contribuer à son échelle à la sécurisation et au développement de la blockchain : le mineur agrège des opérations en attente, non encore incluses dans un bloc et donc non présentes dans la blockchain, Il vérifie la validité de toutes les opérations en attente (compte approvisionné, pas de doublon, …) Le mineur regroupe alors les opérations dans un même bloc, Il soumet ensuite le bloc au réseau, Le réseau étudie la validité du bloc, dans la forme (respect du protocole informatique) et dans le fond (validité des transactions saisies), Le réseau accepte le nouveau bloc et tous les membres l’ajoutent à leur registre de la blockchain. Le minage est avant tout une histoire de mathématique. La validation de transaction s’effectue en résolvant un problème mathématique complexe. Pour trouver la solution au problème, le mineur va essayer une multitude de possibilités jusqu’à trouver le bon résultat. C’est pourquoi, plus le mineur dispose de puissance de calcul, plus il a de chance de trouver le bon résultat avant les autres mineurs. Ce système entraine naturellement de la concurrence et une hausse de la puissance de calcul dans le temps. Ainsi, pour s’adapter à l’augmentation de cette puissance, le protocole prévoit que la difficulté s’ajuste pour maintenir un temps moyen par bloc constant (10 min pour Bitcoin et 15 secondes pour Ethereum par exemple).
{% endhint %}

## Mineur

{% hint style="info" %}
Personne ou groupe de personnes qui connectent sur le réseau une ou plusieurs machines pour effectuer du [minage](glossaire.md#minage). Chaque mineur est rémunéré au prorata de la puissance de calcul qu’il apporte au réseau.
{% endhint %}

## MNBC (Monnaie Numérique de Banque Centrale)

{% hint style="info" %}
Ce sont des monnaies qui sont à la fois digitales et émises par la Banque Centrale, comme la monnaie fiduciaire (pièces et billets).

C’est une pièce de monnaie dont la valeur serait représentée par un code crypté au moyen d’un algorithme, à la place de son matériau physique.

La plupart des MNBC développées actuellement par les pays du monde sont encore à l’état de test.
{% endhint %}

## Nano

{% hint style="info" %}
Nano est une cryptomonnaie qui a pour but d'assurer des paiements très rapides et sans frais. Pour se faire, l'équipe a dévellopé le [DAG (Direct Acyclique Graph)](glossaire.md#dag-direct-acyclic-graph), un dérivé de la blockchain.
{% endhint %}

## Node (Noeud)

{% hint style="info" %}
Un noeud (node) est un dispositif sur un réseau blockchain, qui est le fondement de la technologie, lui permettant de fonctionner et de survivre. Les nœuds sont répartis sur un réseau étendu et exécutent une variété de tâches.

Un nœud peut être n’importe quel dispositif électronique actif, y compris un ordinateur, un téléphone ou même une imprimante, à condition qu’il soit connecté à Internet et qu’il possède une adresse IP.

Le rôle d’un nœud est de soutenir le réseau en gérant une copie d’une blockchain et, dans certains cas, de traiter les transactions. Les nœuds sont souvent disposés dans la structure des arbres, connus sous le nom d’arbres binaires. Chaque cryptomonnaie a ses propres noeuds, qui conservent les enregistrements de transaction des tokens.
{% endhint %}

## Nonce

{% hint style="info" %}
Un nonce est un nombre arbitraire utilisé une seule fois dans une communication cryptographique. C'est souvent un nombre aléatoire ou pseudo-aléatoire. Dans un protocole de vérification de mot de passe avec nonce, le nonce est envoyé du serveur vers le client. L’ajout d'un nonce de client (envoyé du client vers le serveur) améliore la sécurité. Pour s'assurer qu'un nonce est utilisé une seule fois, il doit contenir une composante de temps (comme un horodatage suffisamment précis) ou il doit contenir suffisamment de bits aléatoires pour que la probabilité de génération de deux nonces identiques soit très faible.
{% endhint %}

## Oracle

{% hint style="info" %}
Un Oracle est une source d’informations qui permet d’intégrer des variables issues du monde réel dans des contrats intelligents (voir [**smart contract**](glossaire.md#smart-contract)).

En effet, la blockchain ne permet pas de collecter des données provenant de sources externes (monde extérieur). Ce modèle n'est pas viable car le contenu externe devrait être téléchargé dans un bloc via un tiers. Ainsi, à chaque fois que la blockchain serait téléchargée, la donnée externe serait appelée. Si cette dernière venait à ne plus être disponible, cela compromettrait la blockchain.

Les contrats auto-exécutants (ou smart-contracts en anglais) sont des contrats qui s’exécutent uniquement si des conditions, préalablement fixées, sont remplies. Cela déclenche un événement sur la blockchain comme par exemple un transfert de valeur.

L’Oracle est chargé de fournir des données externes permettant, ou ne permettant pas, le fonctionnement d’applications décentralisées via l’exécution de contrats intelligents.

L’Oracle permet d’ajouter des données du monde extérieur dans un réseau blockchain. Ces oracles sont des services tiers qui fournissent de nombreuses données comme par exemple des températures, des résultats sportifs, des retards aériens...

Ils font office d'autorité et de vérité. En fonction des informations fournies par les Oracles, le contrat intelligent se déclenchera ou non. Rappelons que la blockchain ne peut pas accéder à des données stockées en dehors de son réseau.

Il existe différents types d’oracles :

* Oracles logiciels : ils gèrent des informations disponibles sur internet. Leurs sources sont majoritairement des sites web. Ils permettent de récolter des données comme les températures, retards de vols, prix de produits…
* Oracles physiques : ils envoient des informations provenant directement du monde réel. Il peut par exemple s'agir de capteurs de mouvement ou de puces RFID qui permettent de connaître l’emplacement d’un objet.

Les Oracles physiques et logiciels sont appelés des Oracles entrants. Ils permettent d’intégrer des données du monde extérieur dans la blockchain, particulièrement au travers de contrats intelligents.

D'autres types d'oracles existent :

* Oracles sortants : Ils permettent d'envoyer des données issues de la blockchain au monde extérieur. Par exemple, un transfert de valeur a lieu sur la blockchain, ce qui permet le déblocage d’une serrure dans le monde réel.
* Oracles prédictifs : Ils permettent de confirmer des résultats futurs, notamment grâce à la sagesse des foules.

Pour faire confiance aux Oracles il est nécessaire de ne pas sélectionner une seule source de données. Si cette source venait à être erronée (piratage, erreur, manipulation...), alors la blockchain se baserait sur des données erronées également.

Il est préférable de sélectionner plusieurs Oracles pour que les sources se recoupent entre elles. L'information rapportée par le plus grand nombre d’Oracles sera celle choisie et ajoutée à la blockchain. Il est alors nécessaire de choisir, lors de la création du contrat intelligent, quels seront les Oracles pris en comptes.
{% endhint %}

## Order Book (carnet d'ordre)

{% hint style="info" %}
Un carnet d'ordres est une liste électronique d'ordres d'achat et de vente d'un titre ou d'un autre instrument organisé par niveau de prix.

Les carnets d’ordres sont utilisés par presque tous les échanges pour divers actifs tels que les actions, les obligations, les devises et même les crypto-monnaies.

Ces listes contribuent à améliorer la transparence du marché car elles fournissent des informations sur le prix, la disponibilité, la profondeur du commerce et qui initie les transactions.

Un carnet de commandes comprend trois parties : les ordres d'achat, les ordres de vente et l'historique des commandes :

* Les ordres d'achat contiennent des informations sur l'acheteur, y compris toutes les offres, le montant qu'ils souhaitent acheter et le prix vendeur.
* Les ordres de vente ressemblent aux ordres d’achat.
* Les historiques des ordres de marché montrent toutes les transactions qui ont eu lieu dans le passé.

Bien que le carnet d’ordres soit censé assurer la transparence aux investisseurs, certains détails ne sont pas inclus dans la liste. Parmi ceux-ci figurent les [**darks pools**](glossaire.md#dark-pool)**.** Ce sont des blocs d’ordres cachés maintenus par de grands investisseurs qui ne veulent pas que leurs intentions de trading soient connues.
{% endhint %}

## OTC (Over The Counter)

{% hint style="info" %}
Un marché OTC (marché de gré à gré en français), encore appelé marché hors côte, fait référence aux échanges de titres qui ne se font pas sur une bourse officiellement régulée comme la Bourse de Paris ou le New York Stock-Exchange (NYSE). Différents instruments peuvent faire l’objet d’échange OTC : actions, cryptomonnaies, devises, produits dérivés, etc.

Les transactions de gré à gré se font donc sans la supervision d’une plateforme qui favoriserait la liquidité, la transparence, et réduit le risque entre les différentes parties en imposant un prix d’achat et de vente basé sur l’offre et la demande.

Dans le cas des cryptomonnaies ce sont des transactions qui s'effectuent en dehors des plateformes d'échange comme Binance ou Kraken.

Un marché OTC joue un rôle important pour les institutionnels et les particuliers les plus fortunés. Un marché de gré à gré permet d'acheter ou vendre rapidement et facilement de grandes quantités de cryptomonnaies, sans pour autant que cela n'affecte le cours de la cryptomonnaie impliquée.

Cas concret de l'utilisation des marchés OTC, celui des mineurs. Ceux qui participent à la sécurité du réseau Bitcoin et à la création de nouveaux blocs sont rétribués à hauteur de 6,25 BTC par bloc à l'heure de l'écriture de ces lignes. Cela représente des récompenses conséquentes qui peuvent rapidement s'accumuler.

Ainsi, les mineurs ont très souvent recourt aux marchés OTC pour convertir leurs BTC en monnaie locale, et ainsi payer les dépenses liées au fonctionnement de leur infrastructure.

Il est dans leur intérêt de faire en sorte que le cours du Bitcoin se maintienne même lorsqu'ils vendent leurs fonds. C'est donc pour cette raison qu'ils ont recourt aux marchés OTC.
{% endhint %}

## Perpetual ( contrat perpetuel )

{% hint style="info" %}
Un contrat à terme perpétuel, également connu sous le nom de swap perpétuel, est un contrat d'achat ou de vente non optionnel d'un actif à un moment non spécifié dans le futur. Les contrats à terme perpétuels sont réglés en espèces et se distinguent des contrats à terme normaux par l'absence de date de livraison prédéterminée. Ils peuvent donc être détenus indéfiniment sans qu'il soit nécessaire de reconduire les contrats à l'approche de leur expiration. Des paiements sont périodiquement échangés entre les détenteurs des deux côtés des contrats, long et short.
{% endhint %}

## PoS (Proof of Stake) - Preuve d'enjeu

{% hint style="info" %}
La PoS est un autre moyen de sécuriser une blockchain. Elle demande à l’utilisateur de prouver la possession d’une certaine quantité de crypto-monnaie pour prétendre à pouvoir valider des blocs supplémentaires dans la chaine de blocs et de pouvoir toucher la récompense, s’il y en a une, à l’addition de ces blocs. La chance qu'il soit désigné pour écrire le block suivant est proportionnel à son immobilisation par rapport aux immobilisations totales.
{% endhint %}

## Pishing (hameconnage)

{% hint style="info" %}
Le **phishing** est une pratique malveillante sur le web qui consiste à récupérer des informations personnelles sur un utilisateur, en :

* Utilisant de fausses publicités sur Google,
* Créant de site web frauduleux
* Utilisant l’image d’un domaine pour renvoyer sur un faux site par le biais de sms et par mail.

Pour s’en prémunir :

* Ne cliquer que sur des liens directs, faire attention aux liens sponsorisés,
* Ne jamais communiquer vos phrases de récupération si vous n’êtes pas certain que votre interlocuteur est légitime,
* Vérifier scrupuleusement l'adresse d'expédition du courriel, l'URL du lien hypertexte,
* Repérer les fréquentes fautes d'orthographe ou de syntaxe que contiennent ces e-mails.
{% endhint %}

## Platform (Plateforme)

{% hint style="info" %}
La plateforme est l’espace par lequel transite l’ensemble des informations et désigne tout lieu d’échanges ou se rencontrent l’offre et la demande.\
Comment choisir ?

Même si la plupart des places de trading partagent les même fonctionnalités de base, chacune présente ses spécificités. Voici quelques éléments clefs pour faire votre choix.

Les frais

Les frais d'échanges sont proportionnellement dégressifs au volume sur la majorité des plateformes (0,30 % pour un petit échange, 0,10% pour un gros). N'oubliez pas de vous renseigner sur les commissions de dépôt ou retrait en euro. Les achats par carte bancaire sont certes plus rapides mais restent les plus couteux (jusqu'à 10 % sur certains sites).

Sécurité et législation

En raison de la lutte contre le financement des activités illégales, les places de marché demandent à l'utilisateur de renseigner ses informations personnelles pour accéder aux échanges. La photographie d'une pièce d'identité est souvent nécessaire (voir [**KYC**](glossaire.md#kyc-know-your-customer)). Plusieurs niveaux de vérification sont possibles et certaines plateformes demeurent plus souples que d'autres.

Le délais de vérification peut varier (très rapide pour Coinbase, réputé long chez Kraken).

Volume d'échange

Le volume commercial permet d'apprécier la confiance et le succès d'une plateforme. Ce dernier est sensiblement lié au nombre de cryptomonnaies disponibles à l'échange. Un volume élevé favorise des échanges plus justes en regard du cours moyen sur toutes les places de marché.
{% endhint %}

## PoW (Proof Of Work) - Preuve de travail

{% hint style="info" %}
La PoW est une manière de sécuriser les blockchains. Elle fait appel aux mineurs pour vérifier les données entrantes sur le registre, valider l’authenticité des transactions et créer de nouveaux blocs. Concrètement la preuve de travail consiste à demander aux mineurs de résoudre un problème mathématique complexe nécessitant une puissance de calcul informatique importante.
{% endhint %}

## Produits Dérives (Derivatives)

{% hint style="info" %}
Les produits dérivés sont généralement des produits utilisés par deux parties pour convenir du prix d’un actif sous-jacent sur une période donnée ou à une date future spécifiée. La valeur d’un contrat dérivé vient de la valeur de l’actif sous-jacent.

Il existe différents produits financiers que vous pouvez utiliser pour tirer profit des produits dérivés sur le marché des crypto-devises : futures, swaps, warrants, turbos, contrats perpétuels, options et[ **CFD**](glossaire.md#cfd-contrat-sur-la-difference).
{% endhint %}

## Protocole

{% hint style="info" %}
Les crypto-monnaies fonctionnent grâce à des réseaux décentralisés. Tous les participants du réseau, appelés [nœuds](glossaire.md#node-noeud) «nodes» en anglais, doivent suivre les mêmes règles pour bien fonctionner ensemble. Cet ensemble de règles s'appelle un «protocole».

Les règles typiques d'un protocole incluent par exemple la taille d'un bloc sur une chaîne de blocs, les récompenses reçues par les mineurs pour l'extraction d'un nouveau bloc, et de nombreux autres attributs et propriétés.
{% endhint %}

## Pseudonyme

{% hint style="info" %}
En crypto, votre pseudonyme est l’adresse publique de votre portefeuille. Si vous utilisez le même portefeuille pour payer, ce sera à chaque fois la même adresse publique affichée.
{% endhint %}

## ROI (Return On Investment)

{% hint style="info" %}
Le retour sur investissement, ou ROI en abrégé, est un ratio ou une valeur en pourcentage qui reflète la rentabilité ou l'efficacité d'un certain commerce ou investissement. Le retour sur investissement peut également être utilisé pour comparer différents types d'investissements ou plusieurs opérations de trading.

Plus précisément, le ROI évalue le retour sur investissement par rapport à son coût d'achat. Cela signifie que le calcul du ROI est simplement le retour (bénéfice net) divisé par le total des coûts d'acquisition (coût net).

Un **ROI** de 100% signifie que l'on a doublé sa mise de départ.
{% endhint %}

## Rebase

{% hint style="info" %}
L’univers des cryptomonnaies regorge de projets innovants et d’offres en pleine construction. C’est le cas des jetons de type **rebase**. Une formule de [stablecoins](glossaire.md#stablecoin) hybride qui ne repose plus (uniquement) sur la volatilité de son cours mais sur le nombre de ses unités en circulation.

L’obstacle principal à l’adoption des cryptomonnaies dans le cadre de paiements de la vie courante est sans conteste leur forte volatilité.

Personne n’a envie de payer un objet le prix indiqué pour que quelques minutes plus tard la somme reçue ait perdu plus de 10%. En tout cas pas le vendeur. Ce qui fait qu’à l’heure actuelle les offres de stablecoins rencontrent un grand succès.

Dans le domaine, les offres sont multiples. Cela même si le but est toujours de rester dans un rapport le plus proche possible de 1:1 avec le dollar USD. Mais cette réalité s’accompagne de certaines contraintes. Cela peut aller de l’absence totale – ou presque – de volatilité à la possibilité d’être rémunéré pour en générer des unités. Et il semble qu’une troisième voie permette d’en transférer la volatilité sur [l’offre en circulation](glossaire.md#circulating-supply) (supply). Il s’agit du principe de rebase.

Le principe a le mérite d’être innovant et de répondre à la principale problématique des cryptomonnaies sans en annuler tous les avantages. Il s’agit donc d’une solution de type stablecoin, mais visant une stabilité relative et non absolue.

A terme, c’est le nombre d’unités qui sera volatile et pas le cours de la cryptomonnaie.
{% endhint %}

## Ripple (XRP)

{% hint style="info" %}
C’est un système de paiement construit sur un protocole internet distribué, open source et basé sur une monnaie appelée ripples (XRP). Lancé en 2012, le réseau Ripple vise à permettre des transactions financières mondiales sécurisées, instantanées et presque gratuites.
{% endhint %}

## Refill

{% hint style="info" %}
Racheter une certaine quantité d'une crypto-monnaie que l'on possède déjà à un prix que l'on juge intéressant.
{% endhint %}

## Sats

{% hint style="info" %}
Le terme satoshi et son abréviation SAT désignent la plus petite fraction d’1 Bitcoin. C’est un terme de plus en plus utilisé dans la communauté Bitcoin (BTC), Bitcoin SV (BSV) et Bitcoin Cash (BCH). 1 satoshi = 0,00000001 Bitcoin, dans le sens opposé 1 Bitcoin = 100 000 000 satoshis.
{% endhint %}

## Scalability (Scalabilité)

{% hint style="info" %}
La scalabilité, ou la mise à l’échelle, est la capacité d’une blockchain à s’adapter à un nombre croissant d’utilisateurs et de transactions. Il s’agit d’une problématique à laquelle se heurtent beaucoup de blockchains, dont le Bitcoin et l’Etherum.
{% endhint %}

## Scalping

{% hint style="danger" %}
Le scalping est un style de trading destiné aux accros à l'adrénaline. Le but des traders scalp est de récolter du profit à partir de petits mouvements de prix. Leur objectif est de faire du profit sur plusieurs reprises
{% endhint %}

## SCAM (arnaque)

{% hint style="info" %}
Un Scam est une escroquerie sur Internet. Les exemples les plus courants dans le monde des crypto-monnaies sont les levées de fonds pour un projet ([ICO](glossaire.md#ico-initial-coin-offering)) où les fondateurs du projet disparaissent avec l'argent récolté.
{% endhint %}

## Seed (Phrase de sauvegarde)

{% hint style="info" %}
C'est une phrase de plusieurs mots (12,18 ou 24) permettant d'accéder à tous les fonds qui lui sont liés. L'avantage est qu'une seed permet d'accéder à plusieurs [clés privées](glossaire.md#seed-phrase-de-sauvegarde) de différentes crypto. Ce qui évite de devoir stocker toutes les clés privées. C'est très pratique mais à ne surtout jamais divulguer (au même titre que la clé privée).
{% endhint %}

## Segwit (Segregated Witness)

Un Segwit est un [soft-fork](glossaire.md#fork) du Bitcoin, qui permet de changer le format des transactions dans la blockchain, afin d'augmenter la capacité d'un block, ainsi que la sécurité des transactions.

## Sharding

{% hint style="info" %}
Le sharding (partitionnement en français) est une solution de scalabilité développée pour le réseau Ethereum. Elle permet de fragmenter les données utilisées sur le réseau, afin d’améliorer sa capacité de travail.
{% endhint %}

## Shitcoin

{% hint style="info" %}
On qualifie une cryptomonnaie de shitcoin (littéralement pièce de monnaie de merde) quand celle-ci a perdu presque toute sa valeur avec le temps, ou bien quand elle ne supporte aucun projet solide, voire aucun projet du tout ; on parle alors de « scam » (arnaque).
{% endhint %}

## Short

{% hint style="info" %}
Parier sur la baisse du cours. L'investisseur anticipe la baisse du cours et vend des crypto-monnaies afin de les racheter à un prix plus bas.
{% endhint %}

## Short Squeeze

{% hint style="info" %}
Evènement inattendu qui consiste pour les traders à racheter leur position dans l’urgence car ils ont vendu à découvert. De ce fait, il y a une forte hausse des cours.
{% endhint %}

## Sidechain

{% hint style="info" %}
Il s'agit d'une blockchain secondaire qui se développe parallèlement à une blockchain principale, mais qui y est rattachée afin de pouvoir en connaitre toutes les informations. Les sidechains permettent d'accroître le volume d'informations pouvant être traitées au sein d'une blockchain (volume normalement limité), tout en restant sur une même blockchain principale.
{% endhint %}

## Slippage (dérapage)

{% hint style="info" %}
Lorsque le volume d'échange est trop important ou que des positions entrent en phase de liquidation il est possible de voir le prix exploser dans un sens. Cela peut être tellement rapide et puissant que la plateforme peut être surchargée et votre ordre peut s'exécuter en retard. Un [**Stop Loss**](glossaire.md#stop-loss) ou toute forme d'ordre peut s'activer bien trop tard et vous faire perdre plus que prévu. On appelle ceci l'effet de glissement ou slippage en anglais.
{% endhint %}

## Smart contract

{% hint style="info" %}
Le smart contract, ou contrat intelligent, s'appuie sur la technologie blockchain pour sécuriser et rendre infalsifiables les termes et les conditions de son exécution. Le concept du smart contract est de garantir la force obligatoire des contrats non plus par le droit, mais directement par le code informatique. Ils sont exécutés automatiquement quand certaines conditions sont remplies. Moins couteux, plus rapide et ne nécessitant aucun tiers de confiance, le smart contact trouve déjà de multiples applications dans les domaines de l’assurance, de l’immobilier, de la banque, de la « supply chain », …
{% endhint %}

## Soft Fork

{% hint style="info" %}
Un « Soft Fork » est une modification apportée à un protocole crypto-monnaie, qui reste compatible avec les versions antérieures. Cela signifie que les nœuds non mis à jour sont toujours en mesure de traiter les transactions et de traiter de nouveaux blocs dans la chaîne de blocs, tant qu'ils n'enfreignent pas les nouvelles règles du protocole.

Imaginez un « Soft fork » qui établit une nouvelle règle de protocole réduisant la taille des blocs de 3 à 2 Mo. Les nœuds plus anciens pourront toujours traiter les transactions et extraire des nouveaux blocs de 2 Mo ou moins. Toutefois, si un nœud non mis à jour tente d'extraire un bloc supérieur à 2 Mo sur le réseau, les nœuds ayant été actualisés rejetteront le bloc car il enfreint les nouvelles règles. Cela encourage les nœuds plus anciens à se mettre à jour vers le nouveau protocole, car ils ne sont plus aussi efficaces que ceux qui possèdent la nouvelle version du protocole.
{% endhint %}

## Software

{% hint style="info" %}
Le terme software désigne le matériel virtuel (Logiciel, ...)
{% endhint %}

## Solidity

{% hint style="info" %}
Solidity est un langage de programmation, de type orienté objet, tout comme peuvent l'être le Javascript, le Python ou le C++. Il permet le développement de [smart-contract](glossaire.md#smart-contract) sur la blockchain Etherum. Mais également sur d’autres blockchains liées, comme Tomochain. Afin de permettre à n’importe quel développeur de travailler rapidement avec ce nouveau langage (et aux néophytes d’apprendre facilement) il emprunte beaucoup à d’autres langages de programmations, notamment Javascript, C++ ou C#.
{% endhint %}

## Spot ( au comptant )

{% hint style="info" %}
Le terme spot peut soit qualifier les conditions de négociation d'un marché à l'instant présent ou les modalités de règlement d'un actif négocié par un investisseur.

Les opérations spot s'appliquent régulièrement aux transactions sur les marchés d’actifs, au contraire des marchés derivés dont les négociations ont une échéance à terme.
{% endhint %}

## Spread

{% hint style="info" %}
Le spread représente la différence de prix entre l’offre d’achat (bid) et l’offre de vente (ask) les plus proches. Il est exprimé en pourcentage.
{% endhint %}

## Stablecoin

{% hint style="info" %}
Le stable coin est une monnaie qui diffère de par la stabilité de son cours. La volatilité de son cours est très faible. Son but n’est donc pas de générer une plus-value mais de vous proposer un support qui conserve sa valeur en toute circonstance.

Elle est souvent adossé à une monnaie fiat comme le dollar ou l'euro
{% endhint %}

## Stack

{% hint style="info" %}
Le stack désigne l’ensemble du capital en cryptomonnaies possédé par un investisseur.
{% endhint %}

## Stacking

{% hint style="info" %}
Le staking est un procédé rendu possible par le consensus [Proof-of-Stake (PoS)](glossaire.md#pos-proof-of-stake-preuve-denjeu). Pour faire du staking, un utilisateur verrouille une partie de ses crypto-monnaies. Celles-ci ne peuvent plus être utilisées, mais elles contribuent à soutenir les opérations du réseau. En échange de ce travail, l’utilisateur reçoit des récompenses de « staking », qui sont proportionnelles au nombre de tokens qu’il a verrouillés.
{% endhint %}

## Stop loss

{% hint style="info" %}
Un Stop Loss est un ordre conditionnel, c'est-à-dire que c'est un ordre qui sera envoyé sur le marché après qu'une condition soit remplie. Cette condition prend la forme d'un prix à ne pas franchir. Par conséquent, si ce prix est dépassé, la position est automatiquement clôturé (les crypto-monnaies achetées sont alors vendues).

Le Stop Loss, à l'inverse du [**Take Profit**](glossaire.md#take-profit-tp), protège face à une baisse du prix du marché.(Sauf dans le cas des shorts ou c'est l'inverse) Le prix de vente doit donc être en dessous du prix actuel du marché.
{% endhint %}

## Swing trading

{% hint style="danger" %}
La méthode du swing trading consiste à trader en suivant les mouvements de balance du marché, ses hauts et bas. Cette technique d’investissement boursier est utilisée depuis le 19e siècle et s’applique surtout dans les cycles de trading très courts.

En somme, le swing trading consiste à suivre de manière approfondis les allers et retours des vagues sur le marché boursier. Trader en suivant le sens du courant, le trader a le choix de vente ou d’achat selon les tendances, la décision se doit d’être prise rapidement.
{% endhint %}

## Support

{% hint style="info" %}
Zone à partir de laquelle le marché estime que le prix d'achat est correcte et où de nombreux ordres sont placés faisant office de supports.
{% endhint %}

## Supply

{% hint style="info" %}
Le supply c'est la quantité, bien regarder si il s'agit de quantité totale (max supply) ou en circulation (circulation supply)
{% endhint %}

## Take Profit TP

{% hint style="info" %}
Un Take Profit (TP) est un ordre conditionnel, c'est-à-dire qu'il n'est pas exécuté automatiquement sur le marché au moment de sa création, mais lorsque une condition est remplie. Celle-ci prend la forme d'un prix fixé à l'avance, qu'il est nécessaire d'atteindre pour que l'ordre se déclenche. Lorsque ce prix est atteint, la position est fermée, les coins sont vendus dans le cas d'une position à la hausse (long), ou achetés dans le cas d'une position à la baisse (short). L'objectif du TP est de pouvoir fermer une position lorsque le prix varie, afin de sécuriser ses bénéfices.
{% endhint %}

## Timestamp (horodatage)

{% hint style="info" %}
Le timestamping ou l’horodatage est l’action de prouver l’existence d’un fichier ou d’une donnée à un moment précis.
{% endhint %}

## Testnet

{% hint style="info" %}
Le Testnet est une blockchain alternative destinée à l’expérimentation et aux tests. Les bitcoins du Testnet sont clairement distincts des bitcoins réels et ne sont pas censés avoir une valeur quelconque.

Ce réseau permet aux développeurs d’applications, ou à ceux qui travaillent sur les améliorations de Bitcoin, d’expérimenter sans avoir à utiliser de vrais bitcoins, sans se soucier du consensus et sans faire courir le moindre risque au registre officiel.
{% endhint %}

## Token (jeton)

{% hint style="info" %}
Le token (contrairement au [Coin](glossaire.md#coin-piece)) a un sens symbolique : il représente quelque chose qui n’est pas là. Il est l’équivalent « d’un bon pour » quelque chose, un laisser passer, un signe de reconnaissance, … Les tokens ne sont pas « minables » car ils utilisent une blockchain appartenant à un coin.
{% endhint %}

## Token Swap

{% hint style="info" %}
Lorsque vous investissez dans des crypto-actifs, il se peut que les jetons que vous recevez ne soient que des jetons temporaires qu'on vous donne en attendant que les jetons définitifs soient créés. Lorsque ces derniers sont disponibles, on remplace alors les anciens jetons par ces nouveaux. C’est ce qu’on appelle un token swap, que l'on peut traduire par remplacement de jetons en français.

Le swap vous octroie un nouveau jeton qui continuera à fonctionner avec une mise à niveau importante du crypto-actif, comme par exemple la création d’une nouvelle blockchain. C'est pour cela qu'on parlera parfois de coin ou de pièce pour désigner le nouveau crypto-actif.

Le token swap a lieu selon des modalités déterminées par l'équipe de développement en charge du projet. Il peut être plus ou moins long selon ce qu'elle estime nécessaire.
{% endhint %}

## TOR

{% hint style="info" %}
Le nom Tor est à l'origine un acronyme pour The Onion Router,, littéralement « le routeur oignon ». C’est un réseau informatique mondial et décentralisé qui permet de naviguer de façon anonyme sur internet grâce à des relais.\
Tor est utilisé pour se protéger contre une certaine forme de surveillance sur Internet, connue sous le nom d'analyse de trafic. Cette analyse est utilisée pour déterminer qui communique avec qui sur un réseau public. Connaître la source et la destination de votre trafic peut permettre à des personnes de traquer votre comportement et vos intérêts.

Tor est aussi un outil de contournement de la censure sur Internet. Il permet aux personnes l'utilisant d'accéder à des sites, contenus ou services bloqués dans certaines zones du monde. Facebook ainsi que le site internet de The New York Times proposent ainsi une version de leur site utilisant le système de service caché du réseau.

Tor fait circuler le trafic des personnes utilisatrices via une série de relais. Ce procédé permet de ne pas être suivi par les sites web consultés, d'accéder à des services, contenus ou sites bloqués par un FAI (fournisseur d’accès internet). Il est aussi possible pour chaque personne utilisatrice de publier des contenus via les services « onion » de Tor, sans révéler la position de ces services.

Ces avantages peuvent être utiles pour chaque personne utilisatrice qui souhaite maîtriser ses traces laissées en ligne. Ils sont notamment mis en œuvre dans les échanges entre personnes lanceuses d'alerte, journalistes, avocats, dissidents politiques, représentants d'organisations non gouvernementales, ou pour échanger en maîtrisant la sécurité de leurs données, de leur connexion, de leurs destinataires et de leur position.

Il peut aussi servir à des personnes ou organisations malveillantes en permettant un certain anonymat.

Le navigateur Tor permet aussi à ses utilisateurs de pénétrer dans ce qu'on appelle parfois le Dark Web13, dans une discrétion absolue et sans le besoin d'utiliser un VPN ou un Proxy.
{% endhint %}

## Trading bot

{% hint style="info" %}
Programme informatique configuré pour passer des ordres d'achats et de ventes automatiques (sans intervention humaine) en fonction de paramétrages définis à l'avance par son programmeur.
{% endhint %}

## Transaction fees (frais de transaction)

{% hint style="info" %}
Les frais de transaction sont étroitement liés au [mining](glossaire.md#minage). Les mineurs mettent leur puissance informatique au service du réseau Bitcoin qui peut ainsi garantir l’efficacité des transactions et la sécurité du réseau, sans être contrôlé par aucune autorité :

* Des frais sont nécessaires pour inclure une transaction dans le prochain bloc,
* Le réel montant des frais que vous devez payer varie en fonction du réseau que vous utilisez,
* Les frais de transaction de bitcoins sont d'environs quelques euros, quel que soit le montant que vous envoyez.

Le calcul ou la détermination de la valeur de la commission ou des frais miniers dépend de plusieurs facteurs. L'un des facteurs les plus déterminants est la taille de la transaction au sein du bloc. Mais en plus, l'activité du réseau influence également au moment de la transaction. Ainsi que l'urgence ou la vitesse à laquelle vous souhaitez que votre opération soit confirmée.

Un autre facteur important dans la détermination d'une commission ou d'une redevance minière est l'état du réseau au moment de la transaction. S'il est encombré ou surchargé, il y a de fortes chances que les frais à payer soient beaucoup plus élevés. Sinon, votre transaction peut prendre des heures.
{% endhint %}

## Transaction On-chain

{% hint style="info" %}
Les transactions on-chain font référence aux transactions de crypto-monnaies qui ont lieu sur la blockchain et dont la validité dépend de l'état de la blockchain. Les transactions on-chain ne sont considérées comme valides que lorsque la blockchain a été mise à jour pour refléter les transactions sur le grand livre public. Les transactions sur la chaîne de blocs offrent sécurité et transparence puisqu'elles ne peuvent pas être modifiées une fois qu'elles ont été vérifiées et enregistrées sur le réseau. Cependant, les transactions on-chain présentent certains inconvénients, notamment des frais plus élevés et des délais de traitement plus longs.
{% endhint %}

## Trustless (sans confiance)

{% hint style="info" %}
Cela défini un type d'échange pour lequel il n'est pas nécéssaire de disposer d'un tiers de confiance. Quand vous faites un payement via CB, votre banque fait office de tiers de confiance. Quand vous payez pour un service directement en Bitcoin, il peut être qualifié de trustless. Vous restez en pleine maîtrise de vos fonds.
{% endhint %}

## Turing complete / Turing incomplete

{% hint style="info" %}
Alan Mathison TURING est l’inventeur de l’ordinateur.

Un langage de programmation est appelé « Turing-complet » s’il peut exécuter des programmes quel que soit leur langage, et qu’une machine de Turing peut exécuter avec suffisamment de temps et de mémoire.\
La plupart des langages de programmation modernes sont tous Complets, car ils implémentent toutes les fonctionnalités nécessaires à l’exécution de programmes tels que l’addition, la multiplication, la condition « if-else, » les moyens de stocker, récupérer des données etc.

Mais imaginez que pour une raison quelconque, votre langage de programmation ne puisse pas effectuer cette action.

Cela signifie alors que le programme est « Turing Incomplet ».
{% endhint %}

## UTXO

{% hint style="info" %}
Unspent transaction output (UTXO) désigne une sortie (output) d'une transaction qui n'a pas encore été utilisée comme entrée (input) dans une nouvelle transaction.

Le modèle UTXO peut paraître compliqué mais finalement il est assez simple. C'est le modèle que nous utilisons dans la vie de tous les jours quand nous effectuons des transactions avec du Cash.

Dans ce modèle, chaque transaction a comme origine un output d’une transaction précédente et va générer à son tour de nouveaux outputs (UTXO). Votre wallet va garder la trace de toutes les UTXO associées aux adresses qu’il possède. Lorsque l’on consulte le solde de ses Bitcoins, il va en fait parcourir toutes les UTXO présentes afin de les consolider et d'en afficher la somme.

Dans ce modèle chaque propriétaire de jeton transfère une pièce qu'il possède à un autre en signant numériquement le hachage d'une transaction précédente et la clé publique (adresse) du propriétaire suivant et en les ajoutant à la fin de la pièce. Le mécanisme est essentiellement une transgression continue des entrées et des sorties où le propriétaire des jetons ne possède en fait pas directement les jetons, mais possède plutôt la sortie vers un nombre spécifique de jetons qui peuvent ensuite être transférés en tant qu'entrée à un nouveau propriétaire qui ensuite contrôle les nouvelles sorties.

Il existe 3 règles fondamentales dans le schéma UTXO :

* Chaque transaction doit prouver que la somme de ses entrées est supérieure à la somme de ses sorties.
* Chaque entrée référencée doit être valide et pas encore dépensée.
* La transaction doit avoir une signature correspondant au propriétaire de l'entrée pour chaque entrée.

Malgré certains avantages substantiels du modèle UTXO dans son application dans un cadre comme celui de Bitcoin, il existe encore des inconvénients majeurs, en particulier lorsque le modèle est appliqué à une plate-forme complète Turing plus complexe telle qu'Ethereum. Par exemple, la création d'applications sur la conception UTXO oblige les développeurs à limiter la quantité d'état affectée par chaque sortie.

De même, le schéma de transaction UTXO n'est pas en soi compatible avec le développement de contrats intelligents, car le concept ne convient vraiment que pour une utilisation dans des applications où chaque sortie n'appartient qu'à une seule personne et peut tomber en panne si la sortie peut être consommée par deux personnes ou plus à le même temps.
{% endhint %}

## Vanity adress

{% hint style="info" %}
Correspond à une adresse bitcoin personnalisée, à opposer aux adresses classiques qui sont générées de façon aléatoires.
{% endhint %}

## Volatilité

{% hint style="info" %}
Lorsque le cours d'une crypto-monnaie varie beaucoup on dit de lui qu'il est volatile.
{% endhint %}

## Volume

{% hint style="info" %}
Le volume reflète la force d’une cryptomonnaie : plus celle-ci est échangée, plus le volume de transactions sera important. C'est l'indicateur le plus utile avec le prix pour faire du trading, la plupart des autres indicateurs sont en réalité basés sur des formules de relations entre le prix et le volume d'échanges. Par ailleurs, plus celui-ci est élevé moins le cours est susceptible d'être manipulé par des acteurs isolés et plus l'analyse technique est fiable.
{% endhint %}

## Wallet (Portefeuille)

{% hint style="info" %}
Les portefeuilles ne stockent pas les coins mais génèrent des informations telles que les clés publiques et/ou privées. Dans le cas du bitcoin, par exemple, la cryptomonnaie est stockée de manière décentralisée et conservée dans un registre distribué accessible au public appelé la blockchain. Les différents types de portefeuilles peuvent être divisés en trois groupes : logiciels, matériels et papier. Selon leur mécanisme de fonctionnement, ils peuvent également être appelés portefeuilles chauds (connectés à internet) ou froids (non connectés mais utilisent un support physique pour stocker les clés hors ligne). Les portefeuilles froids sont une alternative beaucoup plus sûre pour stocker vos coins. Cette méthode convient particulièrement aux investisseurs à long terme. Quelque soit le portefeuille, une « seed » (ou phrase de sauvegarde) est générée aléatoirement. Votre seed est le titre de propriété de vos fonds et le portefeuille est l’outil qui vous permet d’en disposer.
{% endhint %}

## Weak hands

{% hint style="info" %}
Représente les personnes qui paniquent facilement et vendent à la moindre rumeur ou dès que le cours d'une crypto-monnaie baisse (quitte à perdre de l'argent).
{% endhint %}

## WEB3

{% hint style="info" %}
WEB3 est une bibliothèque javascript qui permet de communiquer avec la blockchain Etherum et d’interagir avec les contrats qui y sont déployés.
{% endhint %}

## Whale (baleine)

{% hint style="info" %}
C'est le surnom donné aux personnes possédant beaucoup de bitcoins (ou altcoins) et qui peuvent, par le simple fait d'acheter ou de vendre, faire varier le cours d'une crypto-monnaie de façon significative.
{% endhint %}

## White paper (libre blanc)

{% hint style="info" %}
Adapté de l'expression white paper, le terme livre blanc désigne un guide pratique de quelques pages consacré à la présentation d'un projet ou d'une crypto-monnaie. Les livres blancs sont surtout utilisés pour convaincre de l'intérêt d'un projet.
{% endhint %}

## Yield Farming

{% hint style="info" %}
Le Yield farming, littéralement « l'agriculture de rendement », est une approche qui utilise plusieurs stratégies pour optimiser les rendements générés par les cryptomonnaies. La tendance de Yield farming s'est ensuite démocratisée avec la création de nouveaux protocoles DeFi et l'évolution des stratégies.

Le Yield Farming ne s’improvise pas. Sa mise en place nécessite une compréhension des mécanismes liés au protocole de la DeFi pour en tirer un maximum de bénéfices.

Pour schématiser, le principe de fonctionnement du Yield Farming peut se résumer à une technique d’arbitrage. Cette dernière consistant à gagner de l’argent en jouant avec les taux des différents protocoles et des différents pools disponibles. Le tout en fournissant de la liquidité pour le prêt ou l’échange.

« C’est un tout nouveau type de rendement sur un dépôt. En fait, c’est une façon de gagner un rendement sur un prêt. Qui a déjà entendu parler d’un emprunteur tirant profit d’une dette de son prêteur ? » – Maya Zehavi
{% endhint %}
