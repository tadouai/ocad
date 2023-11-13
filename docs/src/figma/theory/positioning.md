# Positionnements

::: tip 🎯 Objectif : Positionner correctement les éléments entre eux au pixel prêt !
![positioning goal preview](../../assets/img/figma/theory/positioning/positioning-goal-preview.png)
:::

## Alignements

### Alignement d'un élément dans un conteneur

Comme nous l'avons déjà vu, Figma permet d'aligner (à gauche, à droite, en haut, en bas, au centre) un élement à l'interieur de son conteneur (`Frame`, `Groupe`, `Section`) :
- directement dans le plan de travail (aides visuelles de Figma)
- à l'aide des boutons d'alignements en haut à droite du `Design panel`

::: details Tutoriel 🎥
![change page background color](../../assets/img/figma/theory/positioning/positioning_alignment_demo.gif)
:::

### Alignement de plusieurs élements

::: tip Sélection en profondeur 💡

Pour sélectionner un élément à l'interieur d'un autre (groupe, frame) : 
- soit double-cliquer jusqu'à atteindre l'élement
- soit maintenir la touche <kbd>Ctrl</kbd> enfoncée puis cliquer sur l'élément

:::

## Espacements

(work in progress)

## Grilles

Les grilles sont des outils de mise en page facilitant le positionnement des différents éléments qui compose nos pages.
Si vous designez pour du format web, elles peuvent être particulièrement utiles pour créer des designs `responsives` mais sont également utiles pour du format tablette ou mobile.

**Les grilles ne sont applicables uniquement sur les `frames`**

Il existe 3 éléments associés aux `layout grid` : les grilles, les colonnes et les lignes.


Pour créer un `layout grid`, commencez par créer ou sélectionner une frame. Depuis cette frame vous pouvez accéder à la section `layout grid` depuis le `panneau de conception`.

Vous pouvez créer 3 layouts différents :
- **les grilles :** statiques, ne dépendent pas de la taille de la frame
- **les colonnes**
- **les lignes**

Il y a 4 types d'alignement de colonnes et de lignes :

- Stretch : la taille des colonnes est automatique pour s'ajuster à la frame
- Center
- Left
- Right 

Il est possible d'ajuster les tailles des colonnes et lignes, mais aussi des `gouttières` et des `marges`.
Une `gouttière` correspond à l'espace entre les lignes ou colonnes.
La `marge` correspond à l'espace aux extrémités des lignes ou colonnes.

INSERER SCREEN SCHEMA

::: details Tutoriel 🎥
<p align="center"><img src="../../assets/img/figma/theory/positioning/layout-grid.gif"></p>
:::