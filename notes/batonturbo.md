# Baton Turbo

**Exemple de chargement de la fonte Baton Turbo**

Cet exemple montre comment charger les différentes variantes de la fonte avec la méthode @font-face.

La fonte propose cinq épaisseurs différentes, allant de *Regular* à *Heavy*. Voici comment des niveaux d'épaisseur peuvent être obtenus avec la propriété CSS font-weight:

```
Regular = 400
Book = 500
Medium = 600
Bold = 700
Heavy = 800
```

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

Pour toutes les variantes, la "font-family" reste identique. Cela permet de déclarer la "font-family" de manière globale, sur notre élément "body":

```css
body {
  font-family: BatonTurbo, monospace;
}
```

Dans cet exemple, on déclare volontairement une fonte alternative très différente pour vérifier que BatonTurbo soit bien chargé.



## Explications:

