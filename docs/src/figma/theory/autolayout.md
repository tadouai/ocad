# Autolayout

L'autolayout est une propriété qui peut être ajouté à une `Frame`. Il vous permet de créer des design qui s'adaptent en largeur/hauteur en se rétréssissant/s'agrandissant. Idéal lorsque vous avez besoin d'ajouter des éléments (positionnement automatique), d'adapter des textes plus longs ou maintenir des alignements à mesure que votre design évolue. 

Il existe plusieurs manière d'utiliser l'autolayout : 
- Créer des boutons qui s'étirent en fonction de la taille du texte qu'ils contiennent
- Créer des listes qui s'adaptent lors qu'un élément est ajouté, supprimé ou caché
- Combiner des `Frame` d'autolayouts pour créer des interfaces complètes et responsives

L'autolayout est une fonctionnalité puissante dont nous allons présenter les propriétés.

## Agencement des éléments

### Direction

L'autolayout agence les élements dans la `Frame` les uns à la suite des autres (on parle aussi d'empilement). La direction de l'empilement peut être soit :
- **Vertical** : Ajouter, supprimer, changer l'ordre des éléments le long de l'axe Y.
- **Horizontal** : Ajouter, supprimer, changer l'ordre des éléments le long de l'axe X.
- **Wrap** : Arranger les éléments sur plusieurs lignes et colonnes dans la `Frame`. La taille de la `Frame` va délimiter le moment ou les éléments vont passer à la ligne suivante.

![autolayout direction](../../assets/img/figma/theory/autolayout/autolayout-direction.png)


**Exercice :** Créer un autolayout et changer sa direction ! Pour ce faire : 
- Créer trois cercle de couleurs différente (cf. l'image ci-dessus)
- Sélectionnez les 3 cercles (maintenir <kbd>Shift</kbd> + click, ou bien utiliser la sélection rapide)
- Utiliser le raccourcis <kbd>Shift</kbd> + <kbd>A</kbd> OU cliquer sur le bouton <img style="border: 1px solid #666666; border-radius: 4px;" height="24px" alt="a" src="../../assets/img/figma/theory/autolayout/autolayout-add-button.svg"> dans le `Design panel` à droite (propriété `Autolayout`) pour créer un autolayout.

> **Remarque :** : Vous pouvez voir que vos 3 cercles sont contenu dans une `Frame`, <kbd>Shift</kbd> + <kbd>A</kbd> permet de créer une `Frame` avec un autolayout. On aurait très bien pu d'abord créer une frame, ajouter les 3 cercles à l'intérieur, et ajouter l'autolayout qu'après !

- Changer la direction de votre autolayout (Vertical, Horizontal, Wrap) dans le `Design panel` dans la section `Autolayout`

::: details Tutoriel 🎥
![autolayout direction tuto](../../assets/img/figma/theory/autolayout/autolayout-direction.gif)
:::

### Ordre d'empilement

Avec un `Autolayout`, si les éléments ont un espacement négatif (superposition des éléments), le dernier élément de la `Frame` apparaît au dessus des autres par défaut. Vous pouvez changer l'ordre de l'empilement des éléments en cliquant sur le bouton <img style="border: 1px solid #666666; border-radius: 4px;" height="24px" alt="a" src="../../assets/img/figma/theory/autolayout/autolayout-more-button.svg"> dans la propriété `Autolayout` ➡ `Canvas stacking` :
- **First on top** : le premier élément de l'empilement sera au dessus
- **Last on top** : le dernier élément de l'empilement sera au dessus

::: details Démo 🎥
![autolayout stacking](../../assets/img/figma/theory/autolayout/autolayout-stacking.gif)
:::

> **Remarque :** Vous pouvez changer la place d'un élément dans un autolayout avec les flèches du clavier après l'avoir sélectionner !

**Exercice :** Ajouter / Supprimer / Cacher / Déplacer des éléments dans un autolayout
- Ajouter une couleur de remplissage à votre `Frame`(celle qui contient les trois cercles) avec la propriété `Fill`
- Créer un cercle d'une autre couleur sur le plan de travail (en dehors de votre `Frame`)
- Sélectionner le et glisser le entre deux éléments dans votre `Frame`
- A l'aide des flèches du clavier, changer sa position
- Vous pouvez le supprimer en cliquand sur <kbd>Back</kbd> ou <kbd>Suppr</kbd>
- (<kbd>Ctrl</kbd> + <kbd>Z</kbd> pour annuler) cachez l'élément en cliquant sur <img style="border: 1px solid #666666; border-radius: 4px;" height="24px" alt="a" src="../../assets/img/figma/theory/autolayout/visibility-button.svg"> à droite dans le `Design panel` > propriété `Layer`.

> **Remarque :** La taille de la `Frame`s'adapte à son contenu par défaut
- Vous pouvez faire réapparaître l'élément caché depuis le `Panel des calques` à gauche ou en cliquant sur <img style="border: 1px solid #666666; border-radius: 4px;" height="24px" alt="a" src="../../assets/img/figma/theory/autolayout/visibility-off-button.svg">

::: details Tutoriel 🎥
![autolayout children](../../assets/img/figma/theory/autolayout/autolayout-children.gif)
:::

### Position absolue

La position absolue (Absolut position) exclue un élément de l'empilement de l'autolayout tout en le gardant dans la `Frame`. L'élément et se qui l'entour s'ignorent l'un l'autre même si on les redimensionne ou change leur position.

Un peut comme en CSS (<code>position: absolute;</code>), un élément en position absolue peut être placé précisément où vous voulez relativement au conteneur parent (la `Frame`).

Les éléments en position absolue sont gérés comme dans des `Frame` classiques (sans autolayout) : vous pouvez leur appliquer des contraintes pour déterminer leur comportoment lors du redimensionnement de la `Frame` parent.

Pour activer la position absolue d'un élément, sélectionnez un enfant d'une `Frame` avec `Autolayout` et cliquez sur <img style="border: 1px solid #666666; border-radius: 4px;" height="24px" alt="a" src="../../assets/img/figma/theory/autolayout/absolute-button.svg">

::: details Démo 🎥
![absolute position](../../assets/img/figma/theory/autolayout/absolute-position.gif)
:::

## Espacements

<img style="border: 1px solid #666666; border-radius: 4px;" height="24px" alt="a" src="../../assets/img/figma/theory/autolayout/spacing-button.svg">

::: details Démo 🎥
![autolayout spacing](../../assets/img/figma/theory/autolayout/autolayout-spacing.gif)
:::