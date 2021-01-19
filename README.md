#TD Gestion de projet - Déployer une application sans code

##Question 4
vercel -v 
=> Vercel CLI 21.1.0

##Question 5 
vercel init

##Question 6
vercel

##Question 7
vercel list gestionprojet

project          latest deployment                     state    age    username
gestionprojet    gestionprojet-lndqm6ah2.vercel.app    READY    9m     agrigoryan5

##Question 8
vercel logs https://gestionprojet.vercel.app

##Question 9
vercel inspect url
Cela permet d'obtenir des information à propos d'un déployement en particulier, comme l'id, name, les builds et les routes

##Question 10
Les variables d'environnement sont des valeurs dynamiques qui permettent les configurations des éléments, ce qui permet d'avoir des variables différentes selon l'environnement, prodution ou developpement par exemple.
L'intérêt de ces variables est qu'elles sont protégées et non accessible directement depuis l'application.

##Question 11
vercel env add plain TEST
(vercel env add type name environnement)

##Question 12
vercel env ls

##Question 13
Cela permet de gerer les secrets dans les varibales d'environnement, donc les données plus sensibles qui ne doivent pas être visible telle que les mots de passe

##Question 15
En ajoutant une varible env secrete depuis l'application, on voit bien qu'il faut d'abord créer une variable de type secret puis l'ajouter dans les varibles d'environnement, on a donc:
	vercel secrets add autre_secret unautremdpsecret
	vercel env add secret AUTRE_SECRET \ autre_secret

##Question 16
Les trois environnements mis à disposition sont : production, preview (correspond au test) et developpement
Il est necessaire d'avoir plusieurs environnement, en effet l'environnement de production sera celui accessible par le public une fois déployé, cependant les développements ne peuvent pas être réalisés dans cet environnement car trop sensible et cela pourrait entraîner des bugs difficilement rattrapable. 
Il y a donc un environnement de developpement qui permet aux personnes de développer localement. Une fois les développements réalisés on utilise l'environnement de test afin de verifier que tout est fonctionnel car ce qui fonctionne en local ne fonctionne pas forcement sur les autres environnement. Une fois les tests validés on peut passer en production. 

##Question 18 
angular.agrigoryan5.vercel.app

##Question 19
Le pull request permet de demander de faire un pull et permet de notifier aux autres qu'une modification va être apporté, et qu'il sera necéssaire de merge la branch master pour avoir accès aux fonctionnalités ajoutées

voir screenshot.png

##Question 20 
Une fois le merge réaclisé, vecrel deploie en test (preview) et l'environnement de production est en attente de validation

##Question 21




