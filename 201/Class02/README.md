# Introduction to Web Development

This topic matters to me because I want to improve my basics of the 3 languages.

## References

<https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/>
<https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals>
<https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting>
<https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured>
<https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics>
<https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals>
<https://chris.beams.io/posts/git-commit/>

## HTML Basics

Headings should be used in a good order, only 3 at max for navigation ease.

Headings are important for accessibility.

## Advanced HTML

This is how to wrap description list:


        <dl> is how to wrap description list
        item is wrapped in <dt/> and the description is wrapped in <dd>
        <dd> can be used multiple times (multiple definitons etc...)

Use the blockquote element to help put code examples into HTML, and a cite attribute to cite the page its from.

            <q> is used to inline quotations

 Use superscript and subscript to mark up items like dates, formulas, and equations.

            25<sup>th</sup> will make the th go above
            C<sub>8</sub> will make the 8 go below

1. Its to help the code be more readable, these tags are easily identifiable.
2. There are 6 levels of headings.
3. Sup can be used to add the mark up the th on a dates day, and sub can be used to put chemical equations numbers under the letters.
4. Using title in the abbr element lets it have the full word when abbreviating.

## CSS 

To add CSS from an external page, you can add the link element to your code, use rel to classify that its a stylesheet, and then the href would be your style page. Ex..

            <!DOCTYPE html>
        <html lang="en-GB">
         <head>
            <meta charset="utf-8" />
            <title>My CSS experiment</title>
            <link rel="stylesheet" href="styles.css" />
         </head>
         <body>
            <h1>Hello World!</h1>
            <p>This is my first CSS example</p>
         </body>
        </html>

Commenting in CSS is done with /* and ends with *\

Internal style sheet would be like using the external just typing everything in the html document with the style element.

This is bad because when having multiple pages, you have to do this for each html.

Inline styling is bad because its the least efficient. Makes code harder to read.

1. Inline stylesheet, external stylesheet, inline coding
2. Its least efficient, and makes code more difficult to read.
3. h2. Color and padding. Black and 5px.

## JavaScript

// is how you comment in JS

Javascript uses operators like math, just = is assignment, and === is equality. ! and !== is Not and does not equal, these are the most important operators.

### Conditionals

If else statement - if is the test, where it compares something and else is the other statement that is ran if the previous isnt true

### Functions

Alert for example is a function, and is followed by an arguement .

1. String
2. Additon, equality, not operator, divison.
3. Getting the tax of an item so you dont have to do the math

## Conditionals

1. Test and if it evaluates to true.
2. To see if something is true, to do this and if not do this.
3. =, >=, <
4. && stands for and, || stands for OR.

## Things I want to know more about

I want to learn more about how to use conditionals better, and I also want to learn how to use certain functions.
I want to learn many of the different selectors to change things in HTML.



