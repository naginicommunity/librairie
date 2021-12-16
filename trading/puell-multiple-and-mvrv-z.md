# Puell multiple & MVRV – Z

## **Introduction**

Aujourd’hui nous allons nous intéresser à deux indices permettant de définir des zones d’achat et de vente. Ces deux indices sont le Puell Multiple et le MVRV-Z score.

Ces indices nous donnent des informations sur l’état du marché, mais n’ont pas énormément d’intérêt seuls. Ils sont à mettre en corrélation avec d’autres indices afin de prendre une décision d’investissement raisonnée. Il est à noter que ces indices sont dit « on-chain ». Ils utilisent des informations disponibles sur la blockchain (transfert de bitcoin, adresses, …) et pas uniquement des informations présentes sur les échanges (prix usd, volume, …)

## **MVRV**

Le MVRV (Market Value / Realized Value) est un ratio entre deux valeures : d’une part la Market value ou Market cap, qui se calcule en multipliant le prix au nombre de token créé, et d’autre part la Realized Value, qui se calcule en multipliant chaque token avec le prix auquel il était échangé la dernière fois qu’il a changé d’adresse.

Exemple :

Imaginons 3 bitcoins en circulation. L’un d’entre eux a été dernièrement échangé le 1er janvier 2021 à un prix de 30 000 $.

Les deux autres ont été dernièrement échangés le 1er janvier 2020 à un prix de 8 000 $.

Dans ce cas la Market value du bitcoin est de 3 x 30 000 = 90 000 $

Et la Realized Value est de 2 x 8 000 + 1 x 30 000 = 46 000 $

Concrètement, la réalized value se calcule grâce aux UTXO (Unspent Transaction Output) qui traquent les derniers changements de main du bitcoin qui sont publiques sur la blockchain. Il est donc possible de multiplier ces UTXO par le prix lors du dernier changement de main afin d’obtenir la Realized Value

Le MVRV, donc le rapport entre ces deux valeurs et nous informe sur le profit potentiellement réalisé si tous les tokens étaient vendus au prix actuel du marché.

Plus ce rapport est élevé, plus les détenteurs sont à profit, et plus il y a de chance que le marché se renverse. Traditionnellement, la valeur signal du MVRV pour la vente est de 3.7. Un MVRV au-delà de 3.7 est un signal de vente, la valeur a de grande chance de chuter prochainement. De la même manière un MVRV en dessous de 1 est un signal d’achat.

**MVRV-Z score**

Le MVRV-Z score est une variante du MVRV mais transmet des informations similaires avec une zone d’achat et de vente, il est généralement plus précis et plus lisible

![](<../.gitbook/assets/MVRV Z-Score.png>)

Source : [https://www.lookintobitcoin.com/](https://www.lookintobitcoin.com)

## **Le Puell Multiple**

![](<../.gitbook/assets/image (17).png>)

Le Puell multiple s’intéresse aux mineurs de bitcoin. En effet, ceux-ci jouent un rôle important dans l’économie du bitcoin, leurs motivations financières sont souvent reflétés dans le prix. D’une part, les mineurs sont souvent perçus comme des vendeurs compulsifs, en effet, il leur est souvent nécessaire de vendre les bitcoins gagnés en minant afin de supporter les couts de leurs machines.

Le puell multiple est un ratio entre les revenus à une date, et la moyenne des revenus sur l’année passée

Si les revenus sont beaucoup plus hauts que ceux précédant alors le mineur a tout intérêt à vendre ses tokens (et donc le prix chutera) d’une autre manière, si le prix aujourd’hui est plus faible que ceux de l’année précédente, alors le mineur aura intérêt à garder ses bitcoins et à les revendre plus tard. Ce qui créera un manque d’offre et fera donc monter le prix.
