# présentation

## **Introduction**

Une Blockchain comme Bitcoin est souvent considérée à tort comme anonyme. D’une certaine manière on peut appeler cette blockchain pseudonyme. Aucun nom n’est requis pour entrer sur la blockchain et toutes les transactions se font grasse aux clés publiques qui ne sont pas forcément raccordées à une clé publique. Cependant, toutes les informations sur la blockchain sont publiques. Il est possible de retracer chaque bitcoin depuis sa création. On peut donc savoir quelle adresse fait tel ou tel transaction. Cela peut poser problème et il n’est pas forcément agréable de savoir que tout le monde peut accéder à votre historique de transaction à partir du moment ou il est possible d’identifier votre adresse à votre identité. Aujourd’hui, nous allons voir un protocole qui tentent de résoudre ce problème et de créer un anonymat plus solide que ceux proposé par des blockchains « classiques »

## **MimbleWimble (MW)**

Réduction de la blockchain

Pas d’adresses identifiables ou réutilisables -> 1 adresse = 1 transaction

Pour connaitre une transaction il faut en être l’auteur, sinon il n’est pas possible de connaitre les informations.

1 Bloc = 1 grosse transaction

Mimblewimble utilise également une fonctionnalité appelée découpe, qui réduit les données de bloc en supprimant les informations de transaction redondantes -> blockchain moins grosse : plus facile à explorer

Cf Transactions Confidentielles (autre tech)

## **Confidentialité de MW**

Prenons l’exemple du Bitcoin

Lors d’un échange, une personne A envoie une transaction qui n’a pas déjà été utilisé à une personne B et la personne B renvoie la somme moins le montant à la personne A

Tout cela est écrit sur la blockchain

Grâce au protocole Mimble Wimble, tout est inconnu aux yeux d’une personne extérieure

On ne peut connaitre ni les adresses ni le montant des transactions.

Le problème est qu’avec des montant et des adresses inconnues il est difficile de savoir si une transaction est valide, c’est-à-dire si A a un solde suffisant/si il n’a pas déjà envoyé cet argent quelque part (double spending)

Cependant, des méthodes d’encryptions permettent de vérifier que les transactions sont correctes sans connaitre le montant exact des transactions

Ces méthodes d’encryptions rendent cependant le volume d’une transaction plus grand et réduisent donc le nombre de transaction par minute.

Afin de résoudre ce problème, une blockchain MW peut être réduite en taille en enlevant les informations redondantes
