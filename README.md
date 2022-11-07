# Intro

Pour ce devoir, j'avais pour but de reproduire au mieux la [capture d'écran du site](maquettes/ordinateur.png) donnée.

Ne connaissant pas encore bien Bootstrap, j'ai décidé de l'utiliser uniquement pour la mise en page, et de faire le
reste en CSS.

Je souhaitais aussi modifier au minimum le HTML fourni, et ne pas utiliser de JavaScript.

Celui-ci peut être trouvé [ici](https://devoirs.rogeaux.com/eliottrogeaux/devoir-css/)

# Résultat

Selon moi, j'ai réussi à reproduire le site plutôt précisément, tout en restant dans les conditions que je m'étais
fixées.

## Modifications HTML

Malgré mon envie de le laisser tel quel, j'ai tout de même légèrement modifié le HTML.

### Liens `<a>`

Tout d'abord, j'ai vidé les `href` initialement présents qui ne fonctionnent évidemment pas ici (chemin relatif).

### Images

Ensuite, j'ai retiré les attributs `height` et `width` sur les images, ceux-ci correspondants à leurs dimensions pas
défaut. J'ai aussi ajouté un `alt` pour les rendre accessibles.

### Header

J'ai ajouté le role `banner` à la `div` contenant le logo et le titre.

Par la même occasion, j'ai remplacé la valeur par défaut de la barre de recherche par un placeholder.

### Navbar

Pour la navbar, j'ai premièrement ajouté un `role="navigation"` pour la rendre accessible. J'ai ensuite retiré les `>`
présents devant chaque ligne pour l'ajouter dans le code CSS à l'aide du pseudo-élément `::before`.

### Contenu

Dans cette partie, j'ai modifié différentes balises pour les rendre plus accessibles, notamment en remplaçant
le `section` principal par un `main`, et en ajoutant un `role="main"`.

J'ai à l'intérieur de celui-ci remplacé la balise `main` pour une `section` avec un `role="contentinfo"`. De même pour
les deux `div` présentes dans le `aside`, auquel j'ai ajouté un `role="complementary"`.

### Footer

Enfin, j'ai ajouté un `role="contentinfo"` au `footer`.

## Complémentaire

### Head

J'ai ajouté la partie du gauche de la bannière comme favicon.

J'ai laissé `Devoir à la maison` comme titre, cependant, j'ai ajouté mon nom et prénom ensuite.

### CSS

J'ai préféré utiliser du SCSS plutôt que du CSS, juste pour simplifier la lecture du code, ainsi que son écriture.

Dans l'optique de reproduire le site au mieux, j'ai tenté de recréer les dégradés présents ainsi que les bordures, les
ombres et les espacements. De ce fait le code CSS est assez long et peut sembler un peu compliqué mais je pense que le
résultat est plutôt satisfaisant.