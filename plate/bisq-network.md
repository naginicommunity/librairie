---
description: >-
  Bisq est une application pair-à-pair open-source qui vous permet d'acheter et
  de vendre des cryptomonnaies en échange de devises nationales. Aucune
  inscription n'est requise.
---

# Bisq network

## Introduction

Rendez-vous sur le site [https://bisq.network/fr/](https://bisq.network/fr/)&#x20;

![page d'accueil ](<../.gitbook/assets/Screenshot 2021-12-22 at 10.04.54.png>)

## Installation et vérification

* Installer le logiciel

![](<../.gitbook/assets/Screenshot 2021-12-22 at 10.07.26.png>)

* Vérifier la signature du logiciel afin d'éviter toute compromission (facultatif mais très important)

Se rendre sur [https://bisq.network/downloads/](https://bisq.network/downloads/) et télécharger la signature PGP.

&#x20;

![](<../.gitbook/assets/Screenshot 2021-12-22 at 10.12.33.png>)

Télécharger le logiciel Gpg4win (windows) afin de procéder à la vérification [https://www.gpg4win.org/index.html](https://www.gpg4win.org/index.html) ou  gnupg (mac) [https://sourceforge.net/projects/gpgosx/files/GnuPG-2.2.33.dmg/download](https://sourceforge.net/projects/gpgosx/files/GnuPG-2.2.33.dmg/download).

Importer la signature publique avec:

```
curl https://bisq.network/pubkey/29CDFD3B.asc | gpg --import
```

Vérifier la signature avec:

```
gpg --digest-algo SHA256 --verify Bisq-1.8.0.dmg.asc Bisq-1.8.0.dmg
```

Il doit apparaitre queqlue chose comme ca&#x20;

![](<../.gitbook/assets/Screenshot 2021-12-22 at 10.44.02.png>)

Je vous conseille de vous rendre sur [https://bisq.wiki/Downloading\_and\_installing#Verify\_installer\_file](https://bisq.wiki/Downloading\_and\_installing#Verify\_installer\_file) en cas de problème.

## Créer un wallet

#### &#xD;Choisir un mot de passe wallet

Allez dans Account et Wallet password

![](<../.gitbook/assets/Screenshot 2021-12-22 at 10.56.17.png>)

![](<../.gitbook/assets/Screenshot 2021-12-22 at 10.59.08.png>)

Si vous venez de créer votre compte, vous pouvez cliquer sur "set password" et passer à l'étape suivante.

#### Sécuriser la phrase de récupération&#x20;

Allez dans account wallet seed et noter la phrase ainsi que la date

![](<../.gitbook/assets/Screenshot 2021-12-22 at 11.05.43.png>)

#### Back up le fichier de données

Il est très important de conserver également ce fichier, il sera beaucoup plus facile pour vous de restaurer toutes vos données en cas de perte.

![](<../.gitbook/assets/Screenshot 2021-12-22 at 11.14.49.png>)

Téléchargez le fichier bisq et le stocker bien au chaud

## Conclusion

Votre installation est terminée et vous êtes pret. Dans la suite on vera pour utiliser Bisq avec GRIN.
