# Normalisation des styles


## Remise à zéro

Bootstrap inclus dans son code source, une version de [`normalize.cs`](http://necolas.github.io/normalize.css/) de Nicolas Gallagher et Jonathan Neal.

Cela permettra à vos productions d'être interpretées de façon identique, quelque soit le navigateur. En effet, chaque navigateur possède un jeu de règles appliquées par défaut. Or celles-ci ne sont pas standardisées ; d'où quelques surprises.

[`reset.css`](http://meyerweb.com/erc/tools/css/reset/) d'Eric Meyer n'a probablement pas été choisi car il induit une certaine complexification des règles de cascade.
`normalise.css` ne modifie pas l'ensemble de tous les éléments HTML.

> **Quote** Normalize.css permet aux navigateurs de restituer tous les éléments de façon cohérente et en accord avec les standards modernes. Il ne cible que les styles qui ont besoin d'être normalisés.

> _traduit du site normalize.css_

[Voici une ressource](http://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css) vous permettant d'appréhender les détails qui rendent `normalize.cs` plus intéressante.


## Styles globaux

- Les valeurs de `margin` ont été supprimées.
- `background-color`est défnii sur la valeur `whie`
- Bootstrap utilise des hauteurs de chasse normalisées (via des variables LESS `@font-size-base`, `@line-height-base`).
- Tous les liens utilise la variable `@linkColor` et seul la pseudo-classe `:hover` affiche un soulignement.

> **Hint** Le fichier `variables.less` défini les valeurs globales d'affichage.

## Conteneur principal

> **Warning** Bootstrap a besoin que vous encapsuliez tous votre contenu dans un élément ayant la classe `container` ou `container-fluid`.

```html
<div class="container">
	<!-- Votre Code -->
</div>
```

