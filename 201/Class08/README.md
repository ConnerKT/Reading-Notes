# CSS Layout

This topic is important to me because I want to explore customize my webpage more and learn how to make them more expansive.

## References

<https://web.dev/learn/css/flexbox/>.
<https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox>.

## Flexbox

**Flexbox** is a layout model designed for one-dimensional contnet.

Excels at taking items of different sizez and returning the best layout.

Understanding Flexbox is understanding the concepts of a main axis and a cross axis.

The main axis is the one set by your flex-direction property.

Flex items move as a group on the main axis.

The cross axis runs in the other direction to the main axis.

On the cross axis you can mover items individually or as a group.

To use flexbox you need to declare that you want to use a flex formatting context and not regular block and inline layout.

display:flex.

### Controlling the direction of items

Row: items layout as a row.
row-reverse: lay out as a row from the end of the flex container.
column: the items lay out as a column.
column-reverse: the items lay out as a column from the end of the flex container.

### Writing modes and direction

Items lay out as a row by default.

direction:rtl sets it to right to left.

Languages like japanese are in vertical writing mode.

Flex items behave by default is linked to the writing mode of the document.

Flex-wrap property will wrap everything it can in the container, but nowrap will let it overflow.

The shorthand for flex direction and flex wrap would be flex-flow.

flex-flow: column wrap;

To let items grow but have more space than small ones use flex:auto;

flex-grow: 0 : no grow.
flex-shrink: 1: items can shrink smaller than their flex-basis.
flex-basis: auto: items have a base size of auto.

Items in your flex container can be reordered using the order property.

In ordinal groups.

## Flexbox Questions

1. It provides better alignment.
2. Main axis is your set, and cross axis runs perpendicular to main axis.
3. By using things like row-reverse it puts the order wrong, so it would be different then what certain accessibility options say.
4. Flex box allows you to control more than just the float area, and you can make it more controlled.
5. It helps me be able to set my web pages better,  I can controll the aspect of my elements better.

## Things I want to know more about

I want to learn how to use flex box for buttons.

I want to be able to make my web page more accessible while using flexbox.

