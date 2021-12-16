# Uniswap

## Introduction

Les cryptomonnaies sont apparues dans le but de résoudre le problème de la centralisation. Comment faire pour échanger de la valeur sans passer par un intermédiaire de confiance. Dans le cas de la monnaie, cet intermédiaire prend la forme d’une banque ou d’un état. Grâce à la cryptomonnaie, il est désormais possible de réaliser cet échange sans avoir à faire confiance à un tiers. Il est possible d’échanger un bitcoin de manière transparente sans avoir à faire confiance à une entité. Cependant, pour acheter ce bitcoin, il est toujours nécessaire de faire confiance à une plateforme d’échange. En effet, disons que nous voulons acheter des bitcoins contre des Dollars. Nous nous mettons d’accord avec un vendeur sur un prix (proche du prix du marché) et afin de réaliser la transaction, nous donnons nos dollars à un échange, le vendeur donne ses bitcoins à l’échange puis l’échange nous donne les bitcoins et donne les dollars au vendeur. En contrepartie de ce service, l’échange prend une commission.

Cette méthode est dite centralisée. Il est nécessaire de passer par un intermédiaire de confiance (ici l’échange) afin de réaliser un échange. Nous allons voir dans cet article comment il est possible de réaliser un échange entre différentes valeurs grâce à Uniswap.

## **ERC20 et UNISWAP**

Uniswap est une plateforme d’échange décentralisée (DEX) permettant d’échanger des tokens ERC20.

Pourquoi seulement des tokens ERC20 ?

Les tokens ERC20 sont des tokens répondant à un nombre de critères leur permettant d’être intégré à la blockchain Ethereum. Ceci leurs permet notamment d’intégrer des smart contracts ou contrat intelligents en français. Ces contrats sont des morceaux de codes enregistrés sur la blockchain Ethereum qui ont pour vocation d’être exécuté. Ces contrats sont scellés grâce à la blockchain et ne peuvent donc plus être modifiés.

Uniswap utilise ces contrats pour permettre d’échanger différents tokens. Cette technologie permet à l’échange d’être complètement transparent et décentralisé.

Le projet a été initié par un développeur d’Ethereum, et est venu d’une idée de Vitalik Buterin (fondateur d’Ethereum)

## **POOL DE LIQUIDITÉ**

L’échange Uniswap fonctionne grâce à des pools de liquidité. Contrairement aux échanges traditionnels qui utilisent des « order book » c’est-à-dire que les acheteurs et vendeurs renseignent les prix auquels ils s’engagent à acheter ou vendre afin de permettre aux échanges de se réaliser, les pools de liquidité sont formés de réserve de tokens (par exemple dans le cas ETH/USDT la pool sera constitué de x ETH et y USDT.) Ces pools sont formés par les market makers qui prêtent une paire de tokens en échange de quoi ils recevront tout ou partie des frais de transaction.

**Comment est Calculé le prix**

Dans le cas de pool de liquidité, le prix est calculé en fonction de la liquidité présente dans la pool.

Uniswap utilise un principe de liquidité 50/50. C’est-à-dire que le prix est égal à la proportion de liquidité dans la pool.

En reprenant l’exemple de la paire ETH/USDT avec x ETH et y USDT

Le prix respecte l’equation x\*y = k avec k une constante fixée

En simplifiant

1 ETH vaudra y/x USDT

Si dans la pool il y a 1 ETH et 400 USDT alors 1 ETH vaut 400 USDT.

Si un Market Maker (personne rajoutant de la liquidité) veut prêter des tokens à la pool de liquidité, alors il devra le faire dans la proportion de la pool

S’il veut rajouter 0.5 ETH, il devra rajouter également 200 USDT

Ainsi, la nouvelle pool sera de 1.5 ETH pour 600 USDT (remarquons au passage que le prix ne change pas), et notre nouvau Market maker detiendra 1/3 de la pool.

Il sera donc rémunéré à 1/3 des frais de transactions effectués sur cette pair.

Imaginons qu’un tradeur veuille acheter pour 1USDT d’ETH, il devra payer 0,30 % de frais de transaction. Ces frais de transactions seront redistribués à la pool de liquidité.

Ainsi, en détenant 1/3 de la pool de liquidité, notre market maker recevra :

0.003 x 1 x 1/3 = 0.001 USDT

## **Comment sont effectués les échanges ?**

Revenons au problème de base : comment échanger des tokens ERC20 sur un Echange décentralisé ?

La personne désirant faire la transaction ira piocher dans la liquidité disponible. Ce qui fera au passage varier le cours du jeton sur l’échange

Reprenons le cas de notre trader disposant d’un USDT et voulant acheter de l’ETH dans une pool d’1 ETH pour 400 USDT

Le prix de l’ETH est donc de 400 USDT

Avec 1 USDT, notre trader achètera donc 1/400 = 0,0025 ETH

CALCUL FAUX (uniquement vrai dans le cadre d’une approximation si le montant de la pool est très supperieur au montant du trade)

Par exemple pour acheter un ETH dans ce cas le prix serait de 400 usdt alors qu’en réalité le prix devrait être de +inf

Je n’arrive pas à trouver de formule exacte correspondante (de toute façon trop compliquée je pense)

De plus cette formule ne prend pas en compte les frais de transaction

Regarder slippage

[https://uniswap.org/docs/v2/advanced-topics/](https://uniswap.org/docs/v2/advanced-topics/)

[https://uniswap.org/whitepaper.pdf](https://uniswap.org/whitepaper.pdf)

Ainsi 0,0025 ETH seront pris de la pool de liquidité et 1 USD sera rajouté à la pool

Ce qui donnera une nouvelle pool de 0.9975 ETH pour 401 USDT

Remarquons que le nouveau prix de l’ETH est de 401/0.9975 ≃ 402 USDT

En effet, en achetant de l’ETH, la demande d’ETH a augmenté et donc son prix par la même occasion.

Plus la pool de liquidité est grande, moins le trade aura d’impact sur le prix du token (plus l’actif sera liquide)

## **Le token UNISWAP (UNI)**

Lors du lancement de leur V2, uniswap ont également lancé leur propre token ERC20 afin de financer le développement de la plateforme.

Au total, 1 milliard de jetons ont été créés et seront distribués au cours des 4 années suivant le lancement d’UNI.

60 % iront aux fournisseurs de liquidités

21,51 % sont destinés au développement du projet

17,8 % sont destinés aux investisseurs

0,069 % sont destinés aux conseillers du projet.

15% des 60% sont destinés aux utilisateurs qui ont utilisés uniswap avant le 1er septembre 2020. Chacun d’entre eux pourront recevoir 400 UNIS

Après ces 4 années, le token aura un taux d’inflation annuel de 2%

(source : coinmarketcap)
