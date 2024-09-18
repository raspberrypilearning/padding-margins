Het diagram hieronder toont het **boxmodel**. Webontwerpers gebruiken dit model om te bepalen welke waarden ze moeten aanpassen om hun marges (margins), opvulling (padding) en randen (borders) de juiste grootte te geven.

![Een rechthoek met aan elke kant een label waarop staat 'top', 'right', 'bottom' of 'left'. De vorm is in vier lagen verdeeld. De buitenste laag is gelabeld als 'margin', de volgende laag is gelabeld als 'border', de derde laag is gelabeld als 'padding' en de vierde laag in het midden van de rechthoek heeft geen label.](images/box-model.png)

De eigenschap `margin` is het buitenste gebied van het element.

De `border` bevindt zich in de `margin`.

De `padding` bevindt zich binnen de `border`.

De ruimte in het midden geeft de inhoud van het element weer.

De code hieronder toont de instellingen voor de `margin` en `padding` eigenschappen.

## --- code ---

language: CSS
filename: style.css
line_numbers: false
line_number_start: 1
line_highlights: 4, 7
----------------------------------------------------------

main {
background: var(--primary); /\* Kleur de achtergrond _/
color: var(--onprimary); /_ Kleur de tekst _/
margin: 0 auto; /_ Centreer als de browser echt breed is _/
min-width: 25rem; /_ Laat de inhoud niet te smal worden _/
max-width: 70rem; /_ Laat de inhoud niet te breed worden _/
padding: 0;
padding-top: 0.5rem; /_ Opvulling bovenaan _/
margin-bottom: 1em; /_ Ruimte voor de voettekst \*/
}
\--- /code ---

Je kunt ook aangeven aan welke kant van de inhoud je margins, padding en borders wilt toevoegen.

## --- code ---

language: CSS
filename: style.css
line_numbers: false
line_number_start: 1
line_highlights: 8-9
---------------------------------------------------------

main {
background: var(--primary); /\* Kleur de achtergrond _/
color: var(--onprimary); /_ Kleur de tekst _/
margin: 0 auto; /_ Centreer als de browser echt breed is _/
min-width: 25rem; /_ Laat de inhoud niet te smal worden _/
max-width: 70rem; /_ Laat de inhoud niet te breed worden _/
padding: 0;
padding-top: 0.5rem; /_ Opvulling bovenaan _/
margin-bottom: 1em; /_ Ruimte voor de voettekst \*/
}
\--- /code ---
