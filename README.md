Introduction :

Dans ce laboratoire, vous allez créer deux fonctions : getPrices() et getDiscount() pour simuler le comportement d'un fabricant de tickets de caisse pour le restaurant Little Lemon. Vous travaillerez avec un ensemble de données représentant les plats, leurs prix et le calcul des taxes. Ce laboratoire renforce les concepts de tableaux, d'objets, de boucles, de conditionnelles et de codage défensif en JavaScript.

Objectif :

Le but de ce laboratoire est de construire un générateur de reçus dynamique en implémentant une logique pour calculer les prix des plats avec ou sans taxe et en offrant des réductions basées sur le nombre de clients.

Objectifs : 

Comprendre et appliquer les boucles et les conditionnelles pour manipuler et afficher les données d'un tableau.

Apprendre à gérer efficacement les paramètres et les arguments dans les définitions de fonctions.

Pratiquer un codage défensif en validant les entrées.

Utiliser des opérations logiques pour mettre en œuvre des prix et des remises dynamiques.

Instructions pour l'apprenant : 

Etapes :
Etape 1 : Ouvrez le fichierProject.js présent dans le dossier LEARN. C'est là que vous écrirez votre code JavaScript.

Etape 2 : Définir la fonction getPrices():

Ajoutez un paramètre nommé taxBoolean à la fonction getPrices().

Étape 3 : Bouclez sur le tableau dishData:

À l'intérieur de la fonction getPrices(), créez une boucle for pour parcourir tous les objets du tableau dishData.

Étape 4 : Déclarer la variable finalPrice:

Dans la boucle, déclarez une variable finalPrice sans lui attribuer de valeur.

Étape 5 : Traiter la tarification conditionnelle : 

Ajoutez une instruction if pour vérifier si taxBoolean est vrai.

Attribuez le prix actuel du plat à finalPrice. 

Étape 6 : Gestion de la tarification sans taxe :

Ajouter une instruction else if pour vérifier si taxBoolean est false.

Attribuer le prix actuel du plat au prix final.

Étape 7 : ajouter un cas par défaut : 

Dans le bloc else, gérer les entrées non valides pour taxBoolean: 

Enregistrez :"You need to pass a boolean to the getPrices call !"(Vous devez passer un booléen à l'appel getPrices !)

Retourner pour quitter la fonction.

Étape 8 : Enregistrer les détails du plat :

Toujours à l'intérieur de la boucle, enregistrez ce qui suit :

"Plat : ", le nom du plat,"Price : $", et finalPrice.

Étape 9 : Définir la fonction getDiscount():

Ajoutez deux paramètres à la fonction getDiscount(): taxBoolean et guests. 

Étape 10 : Appeler getPrices():

Sur la première ligne, appelez getPrices() à l'intérieur de getDiscount() en utilisant taxBoolean comme argument.

Étape 11 : Valider les entrées :

Utilisez le codage défensif pour vérifier :

guests est un nombre.

guests est supérieur à 0 et inférieur à 30.

Si les conditions sont valides, exécutez le bloc if.

Dans le cas contraire, traitez les entrées non valides dans le bloc else.

Étape 12 : Calculer la remise :

Dans le bloc if:

Déclarez une variable "remise" et donnez-lui la valeur 0.

Utiliser if...else if pour attribuer une remise :

Si les invités < 5, fixer la remise à 5.

Sinon, siles invités >= 5, fixer la remise à10.

Enregistrez : "La remise est de : $" + remise. 

Étape 13 : Gestion des entrées non valides pour les invités :

Dans le bloc else :

Enregistrez :"Le deuxième argument doit être un nombre entre 0 et 30". 

Étape 14 : Testez votre code :

Appelez getDiscount() avec différentes combinaisons de taxBoolean et de guests pour vérifier la fonctionnalité.

Exemple: 
getDiscount(true, 2);
getDiscount(false, 10);

Étape 15 : Après avoir modifié avec succès le fichier finalProject.js , naviguez vers File > Save pour enregistrer les changements dans le fichier.  

Pour exécuter votre code JavaScript modifié et vérifier que la fonction fonctionne :

Cliquez sur le bouton Exécuter le code dans le coin supérieur droit (en forme de bouton triangulaire "Play").

Principaux enseignements :

Les tableaux d'objets sont des structures puissantes pour représenter les données.

Les boucles combinées aux conditionnelles permettent de traiter les données de manière dynamique. 

Le codage défensif permet aux fonctions de traiter les entrées non valides avec élégance.

Le pseudo-code et la répartition claire des tâches simplifient les implémentations complexes.
