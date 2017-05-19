# Baton Turbo

**Exemple de chargement de la fonte Baton Turbo**

Cet exemple montre comment charger les différentes variantes de la fonte avec la méthode @font-face.

La fonte Baton Turbo propose cinq épaisseurs différentes, allant de *Regular* à *Heavy*. Voici comment des niveaux d'épaisseur peuvent être définis avec la propriété CSS font-weight:

```
Regular = 400
Book = 500
Medium = 600
Bold = 700
Heavy = 800
```

## Utilisation dans votre CSS

Si on souhaite utiliser la version "Book", voici comment charger les fichiers. Il y a deux déclarations, car on charge le style normal et italique.

```css
@font-face {
  font-family: 'BatonTurbo';
  font-weight: 500;
  font-style: normal;
  src: url('https://fonts.cours-web.ch/BatonTurbo/Book.woff') format('woff');
}

@font-face {
  font-family: 'BatonTurbo';
  font-weight: 500;
  font-style: italic;
  src: url('https://fonts.cours-web.ch/BatonTurbo/BookItalic.woff') format('woff');
}
```

Si on veut appliquer à un élément de notre page la variante "Book Italic", on peut procéder ainsi:

```css
.titre {
  font-weight: 500;
  font-style: italic;
}
```

Pour toutes les variantes, la "font-family" reste identique. Cela permet de déclarer la "font-family" de manière globale, sur notre élément "body":

```css
body {
  font-family: BatonTurbo, monospace;
}
```

Dans cet exemple, on déclare volontairement une fonte alternative (monospace) très différente, pour vérifier durant le développement du site que la webfont BatonTurbo est correctement chargée.

Dans le projet finalisé, on veillera à définir des fontes alternatives se rapprochant du style "sans-serif":

```css
body {
  font-family: BatonTurbo, "Avenir Next", Helvetica, Arial, sans-serif;
}
```

## Restrictions de téléchargement

Afin d'empêcher un téléchargement de la fonte, une sécurisation à été mise en place sur le serveur.

Cela se fait au moyen d'un fichier .htaccess, qui (sur un serveur Apache) peut contenir dès réglages indiquant au serveur qu'une ressource ne pas être accédée depuis n'importe où.

Dans notre cas, l'accès à la fonte n'est possible que depuis le domaine "eaa-3imd-2017.github.io". Si on essaye de télécharger la fonte en accédant [directement au fichier woff](http://fonts.cours-web.ch/BatonTurbo/RegularItalic.woff), le serveur retourne une erreur 403 (eccès interdit).

Plus d'infos sur cette technique: 

* [Documentation cours-web.ch](http://cours-web.ch/divers/htaccess/)
* [.htaccess](https://fr.wikipedia.org/wiki/.htaccess) sur wikipédia