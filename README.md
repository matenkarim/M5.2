# Web Dev Starter Code

## Overview

This project was focusing on how to make HTML websites more accessible for everyone. To run the project, the user can clone the git repository and open it through VSCode. Then, use the Live Preview function to run the website.

## Accessibility Lab Answers

Color
The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors?
    
- The test gave a 2.71:1 ratio. I decided to change it and the new ratio is 6.68:1 which is better.

Semantic HTML
The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.
    
- It starts at the links at the top of the page, then the search query, and jumps down to the audio file and the other links.

Can you update the article text to make it easier for screen reader users to navigate?
    
- Yes, by replacing the `<font>` tags with header tags

The navigation menu part of the site (wrapped in `<div class="nav"></div>`) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.

- It should be a `<nav></nav>`

The Images
The images are currently inaccessible to screen reader users. Can you fix this?

- Yes, by adding alt attributes to explain what the image is.

The Audio Player

- I added a transcript of the audio

The `<audio>` player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio?

- I added an external link to the audio

The Forms
The `<input>` element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers?

- You can add an aria label that will be accessible to screen readers but not sighted users.

The two `<input>` elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this? Note that you'll need to update some of the CSS rule as well.

- Adding label tags will fix this problem


The Show/Hide Comment Control
The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key?

- I added a tab index so the show comments button is keyboard-accessible.

The Table
The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem?

- I added a caption to explain what the table is for. I also added th elements and used the scope feature so I can specify if it is a column or row.


Other Considerations?
Can you list two more ideas for improvements that would make the website more accessible?

- Including roles for the different sections such as nav, main, and footer would help. We could also use focus indicators to show at which part of the website we are currently on.

## Sources and Credits


- WEBAIM: https://webaim.org/resources/contrastchecker/
- ARIA: https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/
- Accessibility: https://developer.mozilla.org/en-US/docs/Learn/Accessibility/CSS_and_JavaScript

