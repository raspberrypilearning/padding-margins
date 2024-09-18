Le diagramme ci-dessous montre le **modèle de boîte**. Les concepteurs de sites web utilisent ce modèle pour savoir quelles valeurs ils doivent ajuster pour que leurs marges, remplissages et bordures soient de la bonne taille.

![Un rectangle qui a une étiquette sur chaque côté pour indiquer « top », « right », « bottom » ou « left ». La forme a été divisée en quatre couches. La couche la plus externe est étiquetée « margin », la couche suivante est étiquetée « border », la troisième couche est étiquetée « padding » et la quatrième couche au centre du rectangle n'a pas d'étiquette.](images/box-model.png)

La propriété « margin » est la zone la plus externe de l’élément.

La « border » s’imbrique à l’intérieur de la « margin ».

Le « padding » s'imbrique à l'intérieur de la « border ».

L'espace au centre montre le contenu de l'élément.

Le code ci-dessous montre les paramètres des propriétés « margin » et « padding ».

## --- code ---

language: CSS
filename: style.css
line_numbers: false
line_number_start: 1
line_highlights: 4, 7
----------------------------------------------------------

main {
background: var(--primary); /\* Colore l'arrière-plan _/
color: var(--onprimary); /_ Colore le texte _/
margin: 0 auto; /_ Centre si le navigateur est vraiment large _/
min-width: 25rem; /_ Ne laisse pas le contenu devenir trop étroit _/
max-width: 70rem; /_ Ne laisse pas le contenu devenir trop large _/
padding: 0;
padding-top: 0.5rem; /_ Remplissage en haut _/
margin-bottom: 1em; /_ Espace avant le pied de page \*/
}
\--- /code ---

Tu peux également spécifier le côté du contenu auquel tu souhaites ajouter des marges, des remplissages et des bordures.

## --- code ---

language: CSS
filename: style.css
line_numbers: false
line_number_start: 1
line_highlights: 8-9
---------------------------------------------------------

main {
background: var(--primary); /\* Colore l'arrière-plan _/
color: var(--onprimary); /_ Colore le texte _/
margin: 0 auto; /_ Centre si le navigateur est vraiment large _/
min-width: 25rem; /_ Ne laisse pas le contenu devenir trop étroit _/
max-width: 70rem; /_ Ne laisse pas le contenu devenir trop large _/
padding: 0;
padding-top: 0.5rem; /_ Remplissage en haut _/
margin-bottom: 1em; /_ Espace avant le pied de page \*/
}
\--- /code ---
