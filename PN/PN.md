# La photographie Numérique (source : David Roche)

## Vidéo 

<iframe width="560" height="315" src="https://www.youtube.com/embed/UnNPNc-F9ks" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Les images

Une image est composée de petits points appelés pixel. La définition d’une image vous donne le nombre de pixels qui compose l’image, par exemple une image de définition 800 x 600 (800 par 600), signifie que cette image est composée de 800 pixels en largeur et de 600 pixels en hauteur, soit en tout 800 x 600 = 480000 pixels. <br>

Un pixel est composé de trois parties : une partie rouge, une partie verte et une partie bleue. À chaque pixel on associe donc 3 couleurs : le rouge, le vert et le bleu. On parle du canal rouge, du canal vert et du canal bleu d’un pixel (on parle de système RVB ou RGB en anglais). La théorie physique de la synthèse additive des couleurs (pour plus d’informations sur cette théorie, voir ici) montre que la variation de l’intensité lumineuse de chaque canal permet d’obtenir un très grand nombre de couleurs. La valeur de l’intensité lumineuse associée à chaque canal de chaque pixel d’une image est très souvent comprise entre 0 et 255 (256 valeurs possibles). On codera donc un pixel à l'aide d'un triplet de valeur (par exemple "247,56,98"). La première valeur donnant l'intensité du canal rouge, la deuxième valeur donnant l'intensité du canal vert et la troisième valeur donnant l'intensité du canal bleu. <br>

![Pixel](./PN/Pixel.png "Image d'un Pixel")

Quand on observe un pixel "à la loupe", on peut constater que le pixel est bien constitué de trois parties : une partie rouge, une partie verte, et une partie bleue (voir schéma ci-dessus). Et là, je suis sûr que vous vous posez une question fondamentale : quand nous regardons une image sur un écran d'ordinateur, nous "voyons" des pixels de différentes couleurs (jaune, mauve,...) et pas des pixels constitués de rouge, de vert et de bleu, pourquoi ?

Cela est dû à une limitation de notre oeil : son pouvoir séparateur !
Un pixel est tellement petit que notre oeil superposera la partie rouge, la partie verte et la partie bleue du pixel, voilà pourquoi nous voyons des pixels de différentes couleurs.

---
### Ex 1

Combien de couleurs différentes est-il possible d’obtenir avec ce système RVB ?

---
### Ex 2

Sur [le site](http://www.proftnj.com/RGB3.htm), faites varier les canaux rouge, vert et bleu (à l'aide des boutons + et des boutons -) afin d'obtenir différentes couleurs.

- Comment obtenir du rouge ?

- Comment obtenir du blanc ?

- Comment obtenir du noir ?

- Comment obtenir du jaune ?

- Que se passe-t-il quand les trois canaux ont la même valeur (par exemple 125,125,125) ?

---

La taille est une autre caractéristique d'une image, elle correspond à la taille de l'image en cm ou en pouce (inch en anglais), toujours en utilisant la largeur et la longueur de l'image. Le papier photo vendu dans le commerce que l'on trouve le plus couramment fait 15 cm en largeur et 10 cm en hauteur. En cas d'impression sur ce papier, on obtiendra des photos de taille 15x10.

En combinant la taille et la définition d'une image, l'on obtient la résolution de cette image. La résolution d'une image est définie par le nombre de pixels par unité de longueur : nombre de pixels par cm ou plus couramment nombre de pixels par pouce (ppp ou dpi).

---

### Ex 3
Soit une image de définition 800x533 que l'on imprime sur du papier photo de taille 15x10 (en cm), calculez la résolution de cette image en ppp (rappel 1 pouce = 2,54 cm).

---

### Ex 4
Sachant que l'on estime que pour avoir une impression de qualité il faut atteindre une résolution de 300 ppp, calculez la définition minimale d'une image dans le cas d'une impression sur du papier photo 15 x 10.

---

### Ex 5
L'écran d'un smartphone a une résolution de 458 ppp, il affiche des images de définition 2436 x 1125. Calculez la taille de cet écran (largeur, hauteur) en cm.

---

## Capteur photo

Au siècle dernier on trouvait dans tous les appareils photo des pellicules. Une pellicule est une surface photosensible (surface qui réagit à la lumière) qui capte les informations lumineuses. Une fois la pellicule terminée (avec une pellicule on peut faire un nombre variable de photos : 6, 12, 24 ou 36), elle était extraite (je parle au passé, mais certains photographes utilisent encore des appareils photo avec pellicule) de l'appareil photo puis développée dans un laboratoire spécialisé grâce à des procédés chimiques, bref, tout cela était quelque peu complexe et quelque peu contraignant (par exemple une photo ratée, était tout de même développée et donc facturée...). Aujourd'hui, fini ces contraintes, on peut prendre autant de photos que l'on veut (dans la limite des capacités mémoires de l'appareil), effacer une photo si elle ne nous convient pas, imprimer uniquement certaines photos sur l'imprimante familiale. Cela a été rendu possible grâce au progrès de l'informatique et de l'électronique et plus particulièrement grâce à l'arrivée dans l'électronique grand public des capteurs photo.<br>

Le capteur photo remplace la pellicule, un capteur photo est donc une surface photosensible. Le capteur photo est composé d'un grand nombre de photosites, chaque photosite va recevoir de la lumière, l'intensité lumineuse va être "convertie" en tension électrique grâce à un effet physique très complexe qui ne sera pas abordé ici : l'effet photoélectrique. Plus l'intensité lumineuse reçue par le photosite est importante plus le photosite produira une tension électrique importante.

![Capteur](./PN/Capteur.png "Capteur")


La tension électrique produite par un photosite sera ensuite "converti" en nombre (on parle de numérisation), à chaque photosite on associera donc un nombre qui sera fonction de la quantité de lumière reçue par ce même photosite. C'est ces nombres qui seront "stockés" dans la mémoire de l'appareil photo.<br>

Si l'on se contentait de ce système, nous aurions uniquement des images en niveau de gris (souvent appelé à tort image en "noir et blanc"). Afin de pouvoir gérer les couleurs, on rajoute donc un filtre coloré devant chaque photosite. Nous avons vu, dans la partie consacrée aux images, qu'il est possible de générer un grand nombre de couleurs uniquement à partir du rouge, du vert et du bleu, nous allons donc trouver 3 types de filtres : des filtres "rouges" (qui laisseront uniquement passer la lumière rouge), des filtres "verts" (qui laisseront uniquement passer la lumière verte) et des filtres "bleus" (qui laisseront uniquement passer la lumière bleue). À chaque photosite on associera soit un filtre rouge, soit un filtre vert, soit un filtre bleu. Il existe différentes façons d'agencer les filtres sur le capteur photo, mais nous ne rentrerons pas dans ces détails ici.

![Grille de Bayer](./PN/gbayer.png "Grille de Bayer")


Comme vous pouvez le constater sur l'image ci-dessus, les filtres dits "Bayer" sont constitués de 50% de filtres vert, de 25% de filtre rouge et de 25% de filtre bleu afin d'imiter la physiologie de l'oeil humain (notre oeil est plus sensible au vert qu'au bleu et au rouge). Dans ce genre de capteur, 50% des photosites enregistrent uniquement la lumière verte, 25% des photosites enregistrent uniquement la lumière rouge et 25% des photosites enregistrent uniquement la lumière bleue.<br>

Précédemment nous avons vu qu'une image est constituée de pixels, mais dans le cas d'une photo d'où vient l'information (canal rouge, canal vert et canal bleu) associée à chaque pixel de la photo ?<br>

La réponse est simple : des photosites du capteur photo. L'association de 4 photosites (deux verts, un rouge et un bleu) donnera les informations qui permettront de créer un pixel de l'image. <br>


![Filtre de Bayer](./PN/FB2.png "Filtre de Bayer")

Comme vous pouvez le constater sur le schéma ci-dessus, l'information produite par un photosite pourra être utilisée pour "construire" 2 pixels se trouvant l'un à côté de l'autre dans l'image finale.

### Ex 6
Rédigez un résumé de quelques lignes qui explique le fonctionnement du capteur d'un appareil photo numérique.

## Le traitement de l'image

Cliquer sur [NBBlock](./PN/Python-photo.ipynb "Python-Photo")

