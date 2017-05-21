# Mises en page CSS

Ce dossier contient des exemples de mise en page CSS.

Pour chaque exemple, le code (CSS et JavaScript) est contenu directement dans le fichier HTML principal.

Voici quelques éléments communs que tous les projets utilisent:

- **CSS / normalize.min.css** : [Normalize](https://github.com/necolas/normalize.css/) est un reset CSS qui corrige certains comportements par défaut de navigateurs.
- **CSS / main.css** : Contient quelques éléments de base que nous utilisons partout. Applique le fonctionnement **box sizing: border-box** à tous les éléments (voir [documentation](http://cours-web.ch/css/box-model)).
- **JS / prefixfree.min.js** : Cet outil, [créé par Lea Verou](http://leaverou.github.io/prefixfree/), ajoute les préfixes navigateurs à notre CSS lorsque c'est nécessaire. Cela nous permet d'écrire un CSS plus sobre, sans préfixes redondants.

Voici les exemples de mise en page proposés:

## carousel.html

Une mise en page comprenant plusieurs sections, qui deviennent visibles au fur et a mesure de l'avancement. La navigation utilise le JavaScript.

* [Voir l'exemple](carousel.html)
* [Notes explicatives](notes/carousel.md)

## carousel-vertical.html

Variation sur la mise en page précédente, avec navigation verticale.

* [Voir l'exemple](carousel-vertical.html)

## batonturbo.html

Exemple de chargement de webfont.

* [Page d'exemple](batonturbo.html)
* [Notes explicatives](notes/batonturbo.md)

## gradient-corners.html

Un effet de coin transparent, obtenu avec un dégradé CSS.

* [Page d'exemple](gradient-corners.html)
* [Article de Lea Verou](http://lea.verou.me/2011/03/beveled-corners-negative-border-radius-with-css3-gradients/) sur cette technique
* [Documentation couleurs et dégradés](http://cours-web.ch/css/color)

## grille.html

Un exemple utilisant le "CSS Grid Layout".

* [Page d'exemple](grille.html)
* [Un article explicatif](https://www.alsacreations.com/article/lire/1388-css3-grid-layout.html) (par Raphaël Goetter) 


------

## Licence 

Le code est mis à disposition sans restrictions de licence et peut être utilisé librement ([The Unlicense](http://unlicense.org/)).