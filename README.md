# Exercice d'accessibilité des contenus

## Équipe
- Isabel Hurtado
- Laurie Martineau

## Objectifs
- Expérimenter le versionnage de fichiers avec GIT
- Acquérire des compétences en accessibilité des contenus

## Prérequis
- Avoir lu et pris connaissance des notes du cours 10
- Avoir un compte GitHub
- Avoir installé et configurer GIT sur votre ordinateur
- Avoir installé l'outil CCA (colour-contrast-analyzer)

## Instructions

### 0. 
- Initialiser un dépôt GIT dans le dossier du projet
- Créer un fichier `index.html` et un fichier `style.css`

### 1.	Donner une alternative textuelle aux images

#### 1.1 Baliser dans le fichier `index.html` les images du dossier `1-textes-alternatifs` 

Pour vous guider dans le choix des balises, des attributs et des valeurs d'attributs, utiliser l'arbre de décision et référez-vous aux notes de cours.

#### 1.2 Évaluer la pertinence des contenus textuels alternatifs

Pour chacune des pages ci-dessous, les textes alternatifs sont-ils adéquats ?Commenter votre observation. Pourrait-on faire mieux ? Donnez un exemple de ce que vous proposeriez.

- https://www.sail.ca/fr/chaussures/junior/multi-sport-et-plein-air 
Les chaussures sont bien identifiés dans les catégories différentes de Junior : enfant, tout-petit, garçon)
Les types d'utilisations des chaussures sont mentionnés comme chaussure de course en sentier, chaussure multisports, ect.
Pour faire mieux, il faudrait ajouter les couleurs des chaussures dans les alt des vignettes en bas des images. De plus, il serait utile d'ajouter la marque de la chaussure dans le alt.
-----
[capture-écran](images/1-textes-alternatifs/1-2/pageSailChaussures_analyseAlt.png)
- https://amzn.to/2NnbKPN 
Il y a une trop grosse présence d'informations dans le alt et il y manque d'organisation. Cela peut être difficile de s'en rappeler et donc la personne non-voyante devra réécouter plusieurs fois la description.
Pour faire mieux, il faudrait réduire la quantité d'informations et la structurer. De plus, il manque l'information sur la couleur du vélo.
-----
[capture-écran](images/1-textes-alternatifs/1-2/pageAmazonVelo_analyseAlt.png)
- https://www.lesoleil.com/  
Les alt remplace les titres des articles. C'est une bonne méthode puisque les images sont à titre décoratif et ne présentent pas d'informations.
Pour s'améliorer, le site devrait rajouter la catégorie de nouvelles dans les alt. De cette façon, les utilisateurs peuvent savoir s'ils visionnent un article de tel type, soit d'actualités, de faits divers, ect dans leurs nouvelles du jour.
-----
[capture-écran](images/1-textes-alternatifs/1-2/pageSoleil_analyseAlt.png)
- https://www.rad.ca/  
Les pages ne présentent aucuns textes alternatifs sur les images. L'accessibilité n'est pas du tout présente.
Même si les images ne présentent pas d'informations, il serait important de leurs ajouter un alt afin de décrire ce qui s'y trouve pour mieux comprendre le sujet de l'article ou de la chronique.
[capture-écran](images/1-textes-alternatifs/1-2/pageRad_analyseAlt.png)

Astuce  
Parfois, l’affichage des alt ne donnent pas un résultat facile à lire… lorsque cela se produit, faites un clic droit de la souris et choisir inspecter pour positionner l’inspecteur de DOM sur le HTML de l’image.
Essayer d’identifier l’emplacement du alt et puis regarder s’il y a une description tout de suite après.

### 2.Vérifier les contrastes de couleurs

#### 2.1	Utiliser l’outil d’analyse de contraste des couleurs (CCA) pour identifier les problèmes de contrastes sur cette page : http://2016.webaquebec.org/

Pour chaque problème de contraste identifié,
documenter le problème par une capture-écran incluant dans son cadre, la zone fautive à gauche et à droite, les résultats détaillés de l’outil, tel que démontré dans l’exemple ci-dessous.

Sauvegarder les captures dans le dossier images. Compléter les liens ci-dessous:
- [Contraste insuffisant 1](images/2-contrastes-couleurs/1contrasteCouleur_SiteWebAQuebec.png)
- [Contraste insuffisant 2](images/2-contrastes-couleurs/2contrasteCouleur_SiteWebAQuebec.png)
- [Contraste insuffisant 3](images/2-contrastes-couleurs/3contrasteCouleur_SiteWebAQuebec.png)

### 3. Structurer avec les h1-h6 une table des matières

#### 3.1 Vérifier la structure

D’après les captures-écrans que vous trouverez dans le dossier [images/3-table-des-matieres_h1-h6/3-1/](images/3-table-des-matieres_h1-h6/3-1) , est-ce que la table des matières du document est correcte?  

Sinon, expliquez le problème en vous basant sur les règles de base énoncées dans les notes de cours. 

__Tutoriel sur les formulaires du w3c__  
[Article](images/3-table-des-matieres_h1-h6/3-1/tuto-form-w3c.pdf)  

[Table des matières (outline)](images/3-table-des-matieres_h1-h6/3-1/tuto-form-w3c-outline.png) 

Réponse : 
Oui le document est correct dans le formulaire du w3c. Il respecte la hiérarchie des titres. Le titre principal est le titre de la page courante et non du site. Tout respecte les régles sur les h1-h6.


__L’affaire Savtchenko__ 
[Article](images/3-table-des-matieres_h1-h6/3-1/article-savtchenko.pdf)  
[Table des matières (outline)](images/3-table-des-matieres_h1-h6/3-1/article-savtchenko-outline.png) 
  
Réponse : 
Le H1 doit être le sujet principal de la page et donc placer dès le début. On ne peut pas n'en mettre aucun ou le mettre après des h2. On doit suivre l'ordre logique, ce qui n'est pas respecter dans l'article savtchenko à cause du h1 placé après des h2.

#### 3.2 S'exercer à bien structurer

- Ouvrir la capture-écran [concevoir-un-design-sans-la-couleur](images/3-table-des-matieres_h1-h6/3-2/concevoir-un-design-sans-la-couleur.pdf) que vous trouverez dans le dossier `sources > h1h6-partie-2` dans le logiciel PhotoShop.  
- Ajouter un calque de blanc à 50% de transparence
- Dans un 3e calque, par-dessus, identifiez les titres et leurs niveaux (h1-h6) de manière voyante (couleur rouge et font-size suffisant)
- Sauvegarder au format .psd ou .png dans le même dossier.
- [Relier ce fichier-réponse ici]()

### 4. Baliser un tableau de données pour qu’il soit accessible

D’après la capture-écran et le texte fourni dans le dossier [4-tableau-de-donnees](images/4-tableau-de-donnees), balisez de manière accessible ce tableau de données.  
  
Votre tableau de données doit comporter un titre (caption) : 

> "Recommandations de consommation de poissons selon l’âge, le sexe et la condition physique".  


Les __entêtes de rangées et de colonnes__ doivent être balisées comme des `<th>` plutôt que des `<td>` et puisque le tableau est *complexe*, vous devez utiliser des attributs `id` dans les `<th>`. 

Chaque cellule `<td>` du tableau doit avoir un attribut headers avec comme valeur(s), le ou les identifiants de ses entêtes de colonnes et de rangées.

Styler le tableau conformément au fichier [consommation-poissons.pdf](images/4-tableau-de-donnees/consommation-poissons.pdf).

#### Ressources
•	balisage accessible d’un tableau (voir les notes du cours 10)
•	balisage html : https://www.w3schools.com/TAGs/tag_table.asp
•	balisage css de tableau: https://www.w3schools.com/css/css_table.asp





