# HTML

## Récapitulatif

Une page HTML, par exemple la page `index.html` (par défaut, la page d'accueil du site), à une **structure arborescente**. Un exemple est représenté ci-dessous:

- `html`
  - `head`
    - `meta [charset]`
    - `meta [name, content]`
    - `title`
  - `body`
    - `a [href, target]`
    - `img [src, alt]`
    - `div`
      - `p`
      - `ul`
        - `li`
        - `li`
        - `li`

_Légende `balise [attribut1, attribut2]`_

### Commentaires

Parfois, on a besoin d'avoir une note pour se rappeler à quoi sert tel ou tel balise, ou tout simplement "cacher" l'élément pendant les tests de développement. Pour se faire, on peut utiliser des commentaires : `<!-- MON SUPER COMMENTAIRE -->`. Les commentaires peuvent être mutilignes si nécessaire.

### `div` et `span`

Les balises `div` et `span` n'ont pas de sens à proprement parler, leur fonction est de "représenter" leurs enfants. C'est très utile pour structurer logiquement son code. On pourra plus tard, appliquer du CSS à ces balises.

Par exemple, on peut assembler plusieurs `div` pour créer une section de commentaires sur son site :

```html
<div id="commentaire">
  <div id="com-1">
    <img src="" />
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Recusandae rerum
      aliquam in vitae veniam nobis eligendi ducimus ea non voluptates?
    </p>
  </div>
  <div id="com-2">
    <img src="" />
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Recusandae rerum
      aliquam in vitae veniam nobis eligendi ducimus ea non voluptates?
    </p>
  </div>
  <div id="com-3">
    <img src="" />
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Recusandae rerum
      aliquam in vitae veniam nobis eligendi ducimus ea non voluptates?
    </p>
  </div>
</div>
```

Une balise `div` prend tout l'espace disponible à l'écran, les éléments qui suivent (et précèdent) une balise `div` ne pourront donc pas (sans ajout de CSS) être sur une même ligne.

Quant à elle, la balise `span` n'impose pas de retour à la ligne, et englobe juste ses enfants (pour leur appliquer un style particulier en CSS par exemple).

### Balises sémantiques

Il existe de nombreuses balises ayant un sens (sémantique) pour le navigateur et les moteurs d'indexations. Elles se comportent de la même façon d'une `div`, à part qu'elles rajoutent du sens en décrivant son contenu.

Par exemple, on retrouvera les balises `header` (qui désigne que ses enfants sont liés à l'en-tête de notre site), `nav` (qui contient la navigation de notre site), `article`, etc. Cf. [documentation](#documentation).

## Todo

- Créer plusieurs pages que tu vas pouvoir lier entre-elles à l'aide de lien (`<a href="">xx</a>`).

- Créer un `header` pour ton site avec le nom de ton site/logo et le menu dedans pour naviguer entre les différentes pages précédemment créées.

  Exemple :

  ```html
  <header>
    <h1>Mon super site</h1>
    <nav>
      <h2>Menu de mon site</h2>
      <ul>
        <li><a href="index.html">Index</a></li>
        <li><a href="page2.html">Page 2</a></li>
      </ul>
    </nav>
  </header>
  ```

- Créer la section principale de ton site (regarde la balise sémantique `main` pour englober tout ça) avec un ensemble d'entrées, plats et desserts par exemple. Chacun de ces éléments pouvant être une `section` qui contient des `articles` (l'élément qui contient les plats).

  Par exemple :

  ```html
  <main>
    <section>
      <h1>Entrées</h1>

      <article>
        <h2>Ma super entrée <span>4.5/5</span></h2>
        <img src="photo-de-l-entree" alt="ma super entrée" />
        <p>Description de la super entrée...</p>
      </article>
      <article>
        <h2>Ma super entrée 2<span>4.1/5</span></h2>
        <img src="photo-de-l-entree-2" alt="ma super entrée 2" />
        <p>Description de la super entrée 2...</p>
      </article>
    </section>

    <!-- Idem pour les plats et desserts... -->
    <section></section>
  </main>
  ```

## Documentation

[Mémento des balises HTML](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1608357-memento-des-balises-html)

[Structurer son site avec des balises sémantiques](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/1605881-structurez-votre-page)

![https://user.oc-static.com/files/343001_344000/343677.png](https://user.oc-static.com/files/343001_344000/343677.png)

## Site webs de qualités

- [Openclassroom](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3)
- [Mozilla Doc](https://developer.mozilla.org/fr/docs/Web/HTML)
- Forum StackOverflow
