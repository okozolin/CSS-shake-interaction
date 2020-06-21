#CSS & HTML shake interaction - Flex trick
by: Orit Kozolin - FrontEnd / FullStack Developer Linkedin
<hr>
<strong>Purpose: </strong>

Activate animation where the triggering element should be displayed after the animated element.

<strong>The Problem: </strong>


With pure HTML,CSS the triggering element should be a parent or a sibling preceeding the animated elemnet in the DOM tree, which condredicts the display spec. Checkout the example and code below to see how it's done

<hr>

###Run

Open <strong>index.html</strong> in the browser.

###How to see the effect
Hover over the blue bar, and watch the notification shake. That's the effect.

###The trick
For this to work you need to do 2 steps in your code:

1. HTML - Place the triggering element (the bar) first in the DOM. And, the triggered element (the notification) after. (Siblings HTML elements or Parent and Child)

2. CSS - Flip their display (rendering) using 'flex-direction: reverse-column' (This is the trick!).

That's it , you're done!
