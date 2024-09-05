The diagram below shows the **box model**. Web designers use this model to see which values they need to adjust to make their margins, padding, and borders the right size.

![A rectangle that has a label on each side to state 'top', 'right', 'bottom', or 'left'. The shape has been divided into four layers. The outermost layer is labelled 'margin', the next layer is labelled 'border', the third layer is labelled 'padding', and the fourth layer in the centre of the rectangle has no label.](images/box-model.png)

The `margin` property is the outermost area of the element.

The `border` nests inside the `margin`.

The `padding` nests inside the `border`.

The space in the centre shows the content within the element.

The code below shows the settings for the `margin` and `padding` properties.

## --- code ---

language: CSS
filename: style.css
line_numbers: false
line_number_start: 1
line_highlights: 4, 7
----------------------------------------------------------

main {
background: var(--primary); /\* Colour the background _/
color: var(--onprimary); /_ Colour the text _/
margin: 0 auto; /_ Centre if the browser is really wide _/
min-width: 25rem; /_ Don't let the content get too narrow _/
max-width: 70rem; /_  Don't let the content get too wide _/
padding: 0;
padding-top: 0.5rem; /_ Padding at the top _/
margin-bottom: 1em; /_ Gap before the footer \*/
}
\--- /code ---

You can also specify which side of the content you wish to add margins, padding, and borders to.

## --- code ---

language: CSS
filename: style.css
line_numbers: false
line_number_start: 1
line_highlights: 8-9
---------------------------------------------------------

main {
background: var(--primary); /\* Colour the background _/
color: var(--onprimary); /_ Colour the text _/
margin: 0 auto; /_ Centre if the browser is really wide _/
min-width: 25rem; /_ Don't let the content get too narrow _/
max-width: 70rem; /_  Don't let the content get too wide _/
padding: 0;
padding-top: 0.5rem; /_ Padding at the top _/
margin-bottom: 1em; /_ Gap before the footer \*/
}
\--- /code ---
