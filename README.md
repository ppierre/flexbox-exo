FlexBox en quelques mots
========================

Mettre l'élément parent (conteneur) en [&#128279;`display:flex;`](https://developer.mozilla.org/fr/docs/Web/CSS/Disposition_flexbox_CSS#Guides) puis trois étapes :

1.  Sur le parent, définir le ou les axes :  
    [&#128279;`flex-flow`](https://developer.mozilla.org/fr/docs/Web/CSS/flex-flow)`: row(-reverse)/column(-reverse) (no)warp(-reverse)`  
    **Travail : [Exo `flex-flow`](exo-1-flex-flow.html)**

2.  Sur chaque élément enfant, définir comment ils adaptent leurs tailles à l'espace disponible :  
    [&#128279;`flex`](https://developer.mozilla.org/fr/docs/Web/CSS/flex)`: auto/initial/none/ {grow} / {grow shrink basis}`  
    **Travail : [Exo `flex: auto...`](exo-2-flex-grow-shrink-basis.html)**

3.  [Sur le parent, définir les alignements](https://developer.mozilla.org/fr/docs/Web/CSS/Disposition_flexbox_CSS/Aligner_des_éléments_dans_un_conteneur_flexible) : `(justify/align)-(content/items) : {alignement}`

    *   `justify` désigne l'axe principale (eg. la ligne)
    *   `align` désigne l'axe orthogonal (par rapport à la ligne)
    *   `content` désigne l'ensemble du contenu, comment il est placé et réparti sur l'axe
    *   `items` désigne le placement (ou agrandissement) individuel de chaque élément par rapport à leurs "ligne/position de base".

    Le vocabulaire d'alignement a été formalisé et unifier dans le [module CSS : box-alignment](https://rachelandrew.co.uk/css/cheatsheets/box-alignment) :

    *   Position : `center / start / end`
    *   Par rapport à la ligne de base du texte : `base-line`
    *   Répartition (du contenu) : `stretch / space-between / space-around / space-evenly`

    **Travail : [Exo alignement](exo-3-alignment.html)**

Autres possibilités de `display:flex;` :
----------------------------------------

*   Les marges peuvent servir à espacer les éléments enfants. Mettre une marge à `auto` va utiliser l'espace libre. Cela peut servir à créer un espace en deux éléments enfants spécifiques.  
    **Travail : [Exo flex et `margin-left:auto;`](exo-4-flex-margin-auto.html)**
*   Changer l'ordre d'affichage avec la propriété `[order: ? ;](https://developer.mozilla.org/fr/docs/Web/CSS/order)`

### Remarques :

*   Si vous donnez des tailles fixes (`px` ou %) à tous les éléments, `display:flex;` présente comme seul intérêt le fait d'être un peu plus simple que les techniques "traditionnelles". Bien employer `display:flex;` : c'est faire des mises ne page qui s'adaptent en fonction de la taille du contenu et de la place disponible. (Voir : [css intrinsic and extrinsic sizing](https://www.smashingmagazine.com/2018/01/understanding-sizing-css-layout/#css-intrinsic-and-extrinsic-sizing) ).
*   Si vous donnez des tailles fixes pour avoir des alignements (verticaux) entre les lignes : c'est que vous devriez utiliser `display:grid;` .

### Autres ressources :

*   **[http://flexboxfroggy.com](http://flexboxfroggy.com) : un jeu où vous aidez Froggy la grenouille et ses amis en écrivant du code CSS!**
*   [https://css-tricks.com/snippets/css/a-guide-to-flexbox/](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
*   [http://tympanus.net/codrops/css\_reference/flexbox/](http://tympanus.net/codrops/css_reference/flexbox/)
*   [http://www.sketchingwithcss.com/samplechapter/cheatsheet.html](http://www.sketchingwithcss.com/samplechapter/cheatsheet.html)