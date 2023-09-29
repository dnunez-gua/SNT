# Thème 3 : Les Structures de données
## Vidéo 

<iframe width="560" height="315" src="https://www.youtube.com/embed/IJJgcZ2DEs0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Vocabulaire

### Identifier un objet 

1. Je souhaite un film s'appelant "la Guerre des Boutons" 

    a. Pourquoi cette information est insuffisante pour identifier le film ?
    
    b. Quelle information dois-je ajouter pour trouver mon film ?
    
 2. Je cherche un livre s'appelant Raisonnements divins, de Martin Aigner et Günter M. Ziegler.

     a. Pourquoi cette information n'est-elle pas suffisante pour identifier ce livre ?
     
     b. Quelle information devrais-je ajouter à ma recherche pour préciser de quel livre il s'agit ?
    
### Etudier des données d'un livre 
 
Dans cette partie, on étudie les données du livre Histoires et cultures du libre, de Camille Paloque-Bergès et Christophe Masutti. Sur sa notice sur le site de la BNF, on lit les informations suivantes.

* Type(s) de contenu et mode(s) de consultation : Texte noté : sans médiation
* Titre(s) : Histoires et cultures du libre [Texte imprimé] : des logiciels partagés aux licences échangées / sous la direction de Camille Paloque-Berges, Christophe Masutti
* Publication : [Paris] : Framasoft : Inno cube ; [Rocquencourt] : INRIA, DL 2013
* Impression : impr. aux États-Unis
* Description matérielle : 1 vol. (XXIII-556 p.) : ill., couv. ill. ; 21 cm
* Collection : Framabook ; 13
* Note(s) : Notes bibliogr.
* Autre(s) auteur(s) : 
        -   Paloque-Bergès, Camille - Directeur de publication 
        -   Masutti, Christophe (1975-....). Directeur de publication
 * Sujet(s) :
        -   Logiciels libres -- Histoire
        - Logiciels libres -- Aspect économique -- Histoire
* Indice(s) Dewey : 005.3 (23e éd.)
* Numéros :
ISBN 978-2-9539187-9-3 (br.) : 25 EUR
EAN 9782953918793
 * Notice n° : FRBNF43580627 <br>

**Questions**

1. Quelles sont les données permettant d'identifier précisement le livre ?
2. Quelles données sont plutôt destinées à des personnes ? Quelles données sont plutôt destinées à des ordinateurs ? 
3. Quelles sont les types de données ? Donner la nature et un exemple. 


### Bilan 

Recopier dans Word la syntèse suivante : 

* Une **collection** est un ensemble d'objets (concrets ou abstraits) dont on collecte des données, partageant les mêmes descripteurs.
* Un **objet** est un élément de cette collection.
* Un **descripteur** désigne l'aspect de l'objet concerné par la donnée.
* Une **valeur** est l'information elle-même.
* Le **type d'une valeur** est la nature de cette information.

De plus, si une donnée concerne une personne, on dit que c'est une **donnée personnelle**. 

### Applications 
1. On considère le sac que vous emenez avec vous au lycée. La collection auquel il appartient est donc l'ensemble des articles vendus par le magasin où vous l'avez acheté. Donner quelques descripteurs pouvant s'appliquer à ce sac à dos, ainsi que les valeurs correspondantes.

2. On considère les données vous concernant, dans la base de donnée d'Ecole Directe.
Donner quelques descripteurs pouvant vous concerner, ainsi que les valeurs correspondantes.

## Données et tableur

1. Créer un document Word - Enregristrer le dans votre OneDrive/SNT en le nommant SD-Tableur-NOM-Prénon

2. Sur internet, aller sur [data.gouv.fr](https://www.data.gouv.fr/fr/)

3. Recherchez *Films entrées* dans le champ de recherche.

4. Téléchargez et ouvrir le fichier *Films ayant réalisé plus d'un million d'entrées* au format .xlsx.

5. Notez vos réponses dans Word:
    
    a.  Quel est le film ayant fait le plus d'entrées en 2021 ?
    
    b. Quel est le film français ayant fait le plus d'entrées en 2018 ?
    
    c. Quelle est la nationalité du film ayant fait le plus d'entrées en 2010 ? 

6. Dans l'onglet *2021*, sélectionner la ligne 7, aller dans le menu *Données* et cliquer sur *Filtre*. 
    
    a. Filtrer par nationalité, cocher *FR* puis valider. 
    
    b. Quels sont les trois films français ayant fait le plus d'entrée en 2021 ?

7.  On souhaite connaître le nombre de films français de cette liste. 

8.  Dans une cellule vide colonne B, écrivez =SOUS.TOTAL(3;B8:B32) (cette fonction permet de calculer le nombre de cellules de la colonne E, mais seulement pour les cellules filtrés). La cellule devrait afficher 7, soit 7 films dans cette liste.

9. On souhaite connaître le nombre d'entrées réalisées par les films français de cette liste. Dans une cellule vide colonne E , écrivez =SOUS.TOTAL(9;E8:E32) (cette fonction permet de calculer la somme de la colonne E, mais seulement pour les films filtrés). La cellule devrait afficher 12,40, soit 12,40 millions d'entrées.

10. Supprimez le filtre sur la nationalité (vous devez à nouveau voir toutes les nationalités), puis triez la colonne sortie par date.  Les trois premiers films affichés devraient être Adieu les Cons, Conjuring 3: The Devil Made Me Do It, Cruella.

11. Le premier de ces films est sorti en 2020. Pourquoi est-il affiché dans cette liste qui concerne l'année 2021 ?

12. On veut connaître, parmi les films des États-Unis sortis en 2021, quels sont les trois films ayant réalisé le plus d'entrée.
Décrire sur votre compte-rendu votre démarche pour répondre à cette question : Quels filtres appliqués ? Quels tris ?
Répondre à la question.

13. Exporter votre fichier Word en pdf et envoyer dans Devoir > 2GTx-Tableur

## format .csv

1. Créer un document Word, enregristrer-le dans votre dossier OneDrive/SNT sous le nom csv-python-NOM-prenom
2. Que signifie les initiales du format csv, donner la signification en anglais et une traduction en français. 
3. Telecharger le document [Informaticiens](./SD/informaticiens.csv).
4. Quels sont le descripteurs de ce fichier ? 
5. Quel est le symbole utilisé comme séparateur ? 
6. En quelle année est née Ada Lovelace ? 
7. Quel est le prénom de Mme Hamilton ?
8. Qui, parmi les personnes listées dans le fichier, est né plus tard ? 

## csv et python

aller sur [le site](https://www.insee.fr/fr/statistiques/2540004?sommaire=4767262),téléchargez *Fichiers par départements de naissance* au format csv.
Ouvrez le fichier .zip ainsi obtenu, et extrayez le fichier dpt2021.csv, que vous enregistrez dans votre Ipad, avec les carnets (ni onedrive, ni Icloud).
Ne pas ouvrir le fichier qui est très lourd, il faut juste le déposer dans Carnets de votre Ipad.

Télécharger [pandas.nbbloc](./SD/Python-csv.ipynb), **ENREGISTER CE FICHIER SUR VOTRE IPAD (DANS CARNETS, MEME DOSSIER QUE dpt2021.csv**, suivre les consignes. Ce fichier sera à rendre sur TEAMS/Devoir 

<!--
## Les données personnelles - Paragraphe argumenté 

Pour ou contre : 

"Si je n'ai rien à me reprocher, je n'ai rien à cacher."


### vidéo 


<iframe width="560" height="315" src="https://www.youtube.com/embed/5otaBKsz7k4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


[documents](./SD/corpus.pdf)

A l'aide d'un paragraphe argumenté, vous exposerez ce qu'est une donnée, qu'est ce qu'une donnée personnelle, comment elle est stockée. Après avoir pris position sur la question pour ou contre, vous exposerez votre avis argumenté. 
Toute recherche réfléchie sur internet ou au CDI est bienvenue. 

-->




