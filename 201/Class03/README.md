# HTML Lists, Control Flow with JS, and the CSS Box Model

This topic is important to me because I want to be able to improve my basics and better my coding skills.

## References

<https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol>.
<https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul>.
<https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model>.
<https://developer.mozilla.org/en-US/docs/Learn/JavaScript>.

## HTML Ordered List and Unordered List

### Ordered List

            <ol> and </ol> are the tags to start and close a ordered list.
            with each item in the list you must contain it in a <li> and </li>.

Attributes that you can apply to the list:
reversed - items in reverse order (high to low).
start - to start counting from the list items.
type - set the numbering type (roman numerals etc).

The usages of Ordered list is usally for steps in something, directions, list of ingredients in decreasing proportion.

### Unordered List

Bullet Points typically.

            <ul> and </ul> are th tags to start and close a Unordered list.
            must contain listed items in <li>.

Attributes that you can apply:
compact - renders the list in a compact style.
type - sets the style of the list.

## Questions for List

1. When you have a group of items that have no numerical or order to them.
2. You use the type attribute.
3. Ordered list for steps and order etc, and unordered list for listing items without order.
4. You can use the type attribute and the start attribute.

## CSS Box Model

Applies to block boxes and defines how the different parts of a box - margin, border, padding, and content - work together to create a box that you can on a page.

Outer display type - It will break onto a new line,the width and height are applied.

Inline display type - It will not break onto a new line, the width and height are not applied.

Margin can pushes other elements away from it, it can overlap.

Padding pushes away from the border, it can not overlap.

## Questions for The Box Model

1. In the story of the box model, theres two characters named margin and padding. Margin is a popular person, who doesn't hesitate to intrude into others lives, and will keep others he doesn't like out, Padding is a quiet kid, who likes to stay in his comfort areas. He doesn't intrude into others personal lives, and only leaves when necessary.
2. Content, Padding, Border, and Margin.

## JavaScript: Arrays, Operators, Expressions, Conditionals, and Loops

### Arrays

Its a method to store data, under a single variable.

list like objects.

If we didn't have arrays, we'd have to store data in every variable.

Examples of arrays:

            const sequence = [1, 1, 2, 3, 5, 8, 13];
            const random = ['tree', 795, [0, 1, 2]];

to check the length of an array:
            sequence.length = 7

you can change the values by specifying the number:

        const shopping = ['bread', 'milk', 'cheese', 'hummus', 'noodles'];
        shopping[0] = 'tahini';
        console.log(shopping);
        // shopping will now return [ "tahini", "milk", "cheese", "hummus", "noodles" ]

An array in an array is called a multidimensional array. to access the array in an array, you have to chain two sets of square brackets together:

            random[2][2]

use the **indexOf** method to find the index of an array.

You can also push items into arrays with **push**.

you can add an item to the start of the array using **unshift()**

**pop()** is used to remove items.

**splice()** is used if you know the index of the item.

### Operators

There are a lot of different operators found here:
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#assignment_operators>.

This is a comprehensive list, I think for now the basics of operators are good.

### Conditionals

<https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals>.

If Statements

Else if statements

comparison operators

### Loops

<https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code>.

while and for loops-

While this condition isnt met do this and this until it is met.

for loops-

for this in this, do this.

## JavaScript Questions

1. Integers, Booleans, Strings, Objects
2. Yes it is, to access this you need to chain two square brackets to access deeper into arrays.
3. +=, -=, *=, /=, %=
4.  You would get 10dog, because its two strings so they combine, but c is false, has no string value so it does nothing.
5. If your varaible equals x, do this for your program, else do this for your program.
6. When you want to loop until a condition is fullfilled, when asking the user for their credit card information.

## Things I want to know more about

I want to learn more deeply about arrays and how they function.

I want to learn more about advanced functions after learning the basics.

How do I get CSS animations through flex box.

