# CSS Animations

This topic is important to me because I've been interested in CSS animations for so long since my first project, so I'm glad I can put it to practice.

## References

CSS Transformations <http://learn.shayhowe.com/advanced-html-css/css-transforms/>.

CSS Transitions and Animations <http://learn.shayhowe.com/advanced-html-css/transitions-animations/>.

8 Ways to upgrade your page <http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users>.

MISC:
CSS Bounce Animation<http://codepen.io/dp_lewis/pen/gCfBv>.

Button Animations<http://codepen.io/retyui/pen/ByoaXV>.

Keyframing<http://codepen.io/akshaychauhan/pen/oAfae>.

404<http://codepen.io/kieranfivestars/pen/MYdQxX>.

## CSS Transform

**Tranform** is a property that came with CSS3 that allows us to choose two dimensional or three dimensional transform of our elements.

    -webkit-transform: scale(1.5);
        -moz-transform: scale(1.5);
        -o-transform: scale(1.5);
            transform: scale(1.5);

(Those are vendor prefixes that are added to sites so multiple browsers can be supported).

The **transform** property takes a bunch of different values.
**Rotate** lets you rotate from 0-360 degrees.
Using a negative value will rotate it counterclockwise.

    .box-1 {
    transform: rotate(20deg);
    }
    .box-2 {
    transform: rotate(-55deg);
    }

Its possible to only scale the height or width of an element using **scaleX and ScaleY values**.

The **Translate** value works liek relative positioning, pushing and pulling an element in different directions.

You can use it similar to transform, but specifying if you want it to translateX, and translateY.

**2D skew** is used to distory elements on the horiontal axis, vertical axis, or both. Similar to scale and translate values.

Using **skewX** distorts the element on the horizontal axis.

Using **skewY** distorts an element on the vertical axis.

    .box-1 {
    transform: skewX(5deg);
    }
    .box-2 {
    transform: skewY(-20deg);
    }
    .box-3 {
    transform: skew(5deg, -20deg);
    }

The last box is an example of using both horizonal and vertical!

Combining transforms is pretty simple, you just put them both on the same property.

    .box-1 {
    transform: rotate(25deg) scale(.75);
    }
    .box-2 {
    transform: skew(10deg, 20deg) translateX(20px);
    }

Behind every transform, there is a matrix that defines its behavior. Using rotate, scale, translate, and skew provides ways to establish the matrix.

**Tranform Origin** lets you manipulate an items origin which is both 50% on horizonal and vertical.

In order for three-dimensional transforms to work the elements need a **perspective** from which to transform. 

Using 3D transformations we can manipulate elements on the z axis, giving us control of depth as well as length and width.

To rotate an element, we can use rotateX,Y,or Z to rotate it in the transform values.

    .box-1 {
    transform: perspective(200px) rotateX(45deg);
    }
    .box-2 {
    transform: perspective(200px) rotateY(45deg);
    }
    .box-3 {
    transform: perspective(200px) rotateZ(45deg);
    }

You can also scale the Z axis on scale.
example: scaleZ(value)

Using translateZ lets you translate on the z axis.

There is no 3D skew.

Backface Visibility lets you hide the element whenever it is facing away from the screen.

### CSS Transforms

1. Lets you transform your items so they look different.
2. I would do it for animated backgrounds, or uniquely placed items.

## CSS Transitions and Animations

**Transitions** provide a change from one state to another.

Different styles must be identified.
:hover, :focus, :active, :target.

    .box {
    background: #2db34a;
    transition-property: background;
    transition-duration: 1s;
    transition-timing-function: linear;
    }
    .box:hover {
    background: #ff7b29;
    }

The **transition-property** property determines exactly what properties will be altered in conjunction with the other transitional properties.

Duration - Sets the duration of the transition.

To set multiple points at which an element should undergo a transition, use the **@keyframe** rule.

It includes the animation name, any animation breakpoints, and its properties.

### CSS Transitions and animations questions

1. Provides a change from one state to another.

2. Animation allows oyu to change the properties of an element over a duration and transtion defines how an element changes over a specific duration.

## CSS3 Transitions

(The code examples on this site are broken).

1. To add a better experience to your web pages to make it more personalized.

2. It fits because I want to make sites that contain good features that feel smooth and unique.

## Things I want to know more about

I want to know more about looping css animations to make interesting designs.
 I want to know more about keyframing.


### Psychological Safety Questions

1. Dependability, structure, and psychological safety.
2. In college I had a group where I did english work, and we would share our work without being ashamed or worried about being judged. It was nice to show your work to get feedback and it was friendly to make friends as well.
3. It produces great work places where people can collaborate and bring great project ideas to board without being scared of being judged.
