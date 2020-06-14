# Dimanche 14 Juin - HTML / CSS

## Récapitulatif

Pour inclure un fichier CSS dans une page HTML, il suffit d'ajuter la balise `<link href="styles.css" rel="stylesheet" />` dans le `head`.

On peut également écrire du CSS dans une balise `<style></style>` également située dans le `head`. Cependant, on évitera d'utiliser cette méthode pour écrire du style, bien qu'elle peut se réveler utile, étant donné que ces sélecteurs CSS prennent le dessus sur ceux écrit dans le fichier spécifique.

Pour finir, on peut directement styliser un élément HTML en ajoutant du CSS avec un attribut `style`. Ex: `<p style="color:red;"></p>`. Cette pratique peut être utilisée pour surcharger un style appliqué depuis une feuille de Style ou les balises `<style></style>`.

### Display `block` ou `inline` ?

#### Block

Certains éléments (h1, h2..., p, ul, div) sont des éléments dits de type `block`. Il prennent la totalement de la largeur disponible à l'écran et les éléments frères sont systématiquement affichés en DESSOUS d'eux.

#### Inline

Au contraire, les éléments `inline` ne prennent que l'espace dont ils ont besoin pour s'afficher (a, img, span). Leur éléments frères seront donc à côté d'eux.

### Display `flex`

Lorsque l'on souhaite positioner des éléments de façon particulière (changer le positionnement par défaut), on peut utiliser les `flexboxs`: `display: flex;`.

![Flexbox exemple](https://i.pinimg.com/564x/9c/83/89/9c8389214caea9999e7ee5084b34e316.jpg)

Par défaut, les éléments se positionnent en ligne (`flex-direction: row;`). On peut changer l'**axe** principal en colonne (`flex-direction: colmun;`).

Il existe de nombreuses propriétés pour changement le positionnement des éléments enfants : [voir cet article Medium](https://medium.com/code-sketch/flexbox-visual-guide-17ab04d6a536).

Dans notre cours, nous avons utilisé le `justify-content: space-between;` qui permet d'opposer les éléments de la ligne.

Pour centrer verticalement le paragraphe, nous avons utilisé le `align-self: center;` qui permet de définir l'alignement de l'élément en question ("self").

### Classes et IDs

#### Classes

Ajouter une classe sur un élément HTML pour pouvoir le customer en CSS

`<p class="paragraphe-rouge">Lorem ipsum.</p>`

```css
.paragraphe-rouge {
  color: red;
}
```

_Note: On peut ajouter autant de classes que l'on souhaite à un élément._

#### IDs

Ajouter un ID sur un élément HTML pour pouvoir le customer en CSS ou être rediriger vers l'élément via l'URL (ex. http://mon-site.fr/page1#paragraphe-special)

`<p id="paragraphe-special">Lorem ipsum.</p>`

```css
#paragraphe-rouge {
  font-size: 3rem;
}
```

**_ATTENTION: Un ID doit être UNIQUE._**

### Exemple fichier CSS

```css
balise {
  background-color: aqua;
}

#id {
  color: red;
}

.classe {
  color: green;
}

.classe2,
.classe3 {
  color: yellow;
}

selector:pseudo-selector {
  color: blue;
}
```

## Documentation

[Mémento des balises CSS](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1608902-memento-des-proprietes-css)
