# Learn CSS Transforms by Building a Penguin

You can transform HTML elements to create appealing designs that draw your reader's eye. You can use transforms to rotate elements, scale them, and more.

In this course, you'll build a penguin. You'll use CSS transforms to position and resize the parts of your penguin, create a background, and animate your work.

## Step 1

You will be building a happy Flappy Penguin, and further exploring CSS transforms and animations in the process.

Begin with your basic HTML boilerplate. Include the `DOCTYPE` declaration, `html` element with a language set to English, the appropriate `meta` tags, a `head`, `body`, and `title` element. Also, link your stylesheet to the page.

## Step 2

Target the `body` element to set the `background` to a linear gradient angled 45 degrees clockwise, starting at `rgb(118, 201, 255) and ending` at `rgb(247, 255, 222)`.

## Step 3

Normalise your page's sizing, by removing the `body` element's `margin` and `padding`.

## Step 4

Normalise your page, by setting the `width` to `100%`, and `height` to `100vh`.

## Step 5

Remove both the horizontal and vertical scrollbars, using only one property.

>Example Code
>
>```overflow
>overflow: hidden;
>```

## Step 6

Within the `body`, add a `div` with a `class` of `ground`.

## Step 7

Target the `.ground` element, and set its `width` to take up the full width of the viewport. Then, set the `height` to `400px`.

## Step 8

Give the `.ground` element a `background` with a linear gradient angled 90 degrees clockwise, starting at `rgb(88, 175, 236)` and ending at `rgb(182, 255, 255)`.

## Step 9

As the `.ground` element will be third in the stacking context of the page layout, set its `z-index` to `3`, and `position` to `absolute`.

## Step 10

Above the `.ground` element, add a `div` with a `class` of `penguin`. This `div` will contain Flappy Penguin.

## Step 11

Target the `.penguin` element, and set its `width` and `height` to `300px`.

## Step 12

Use the `margin` property to horizontally center the `.penguin` element, and set the `margin-top` to `75px`.

>Example Code
>
>```margin
>margin: auto;
>margin-top: 75px;
>```

## Step 13

To create some scenery in the background, you will add two mountains.

Above the `.penguin` element, add a `div` with a `class` of `left-mountain`.

## Step 14

Target the `.left-mountain` element, and set its `width` and `height` to `300px`. Then, set the background to a linear gradient starting at `rgb(203, 241, 228)` and ending at `rgb(80, 183, 255)`.

## Step 15

To prevent the mountain from pushing the `.ground` element, adjust its `position` to prevent it from taking up space in the page layout.

>Example Code
>
>```position
>position: absolute;
>```

## Step 16

To make the mountain look more like a mountain, you can use the `skew` transform function, which takes two arguments. The first being an angle to shear the x-axis by, and the second being an angle to shear the y-axis by.

Use the `transform` property to skew the mountain by `0deg` in the x-axis and `44deg` in the y-axis.

>Example Code
>
>```transform
>transform: skew(0deg, 44deg);
>```

## Step 17

Set the stack level of the mountain element such that it remains directly behind the `.ground` element.

>Example Code
>
>```z-index
>z-index: 2;
>```

## Step 18

To overlap the mountain and `.ground` elements better, give the mountain a `margin-top` of `100px`, and the `.ground` element a `margin-top` of `-58px`.

## Step 19

To give the effect of a mountain range, add another mountain, by creating a new `div` immediately after `.left-mountain`, and give the new `div` the `class` of `back-mountain`.

## Step 20

Target the `.back-mountain` element, and set its `width` and `height` to `300px`. Then, set the `background` to a linear gradient starting at `rgb(203, 241, 228)` and ending at `rgb(47, 170, 255)`.

## Step 21

Set the `position` property of the `.back-mountain` to prevent it from taking up space in the page layout.

>Example Code
>
>```position
>position: absolute;
>```

## Step 22

Change the stack level of the `.back-mountain` element such that it is directly behind the `.left-mountain` element.

>Example Code
>
>```z-index
>z-index: 1;
>```

## Step 23

Rotate the `.back-mountain` element by `45deg` clockwise. Then, give it a `left` property of `110px`, and a `top` property of `225px`.

>Example Code
>
>```transform
>transform: rotate(45deg);
>```

## Step 24

To finish the background, add a sun, by creating a new `div` element immediately after the `.back-mountain` element, and give it the class of `sun`.

## Step 25

Give the `.sun` element a `width` and `height` of `200px`, and a `background-color` of `yellow`.

## Step 26

Set the `position` property of the sun to prevent it from taking up space in the page layout, and set the `border-radius` such that the sun's shape is a circle.

>Example Code
>
>```position
>position: absolute;
>border-radius: 50%;
>```

## Step 27

Position the sun in the `top` `right` corner of the screen such that `75px` of its top and right edges are off screen.

>Example Code
>
>```top
>top: -75px;
>right: -75px;
>```

## Step 28

Your penguin will consist of two main sections: the head, and the body.

Within `.penguin`, add two new `div` elements. The first with a `class` of `penguin-head`, and the second with a `class` of `penguin-body`.

## Step 29

Change the stack level of the `.penguin` element such that it appears in front of the `.ground` element, and give it a `position` of `relative`.

>Example Code
>
>```z-index
>z-index: 4;
>position: relative;
>```

## Step 30

Target the `.penguin-head` element, and give it a `width` `half of its parent's`, and a `height` of `45%`. Then, set the `background` to a linear gradient at `45deg` starting at `gray`, and ending at `rgb(239, 240, 228)`.

## Step 31

*Most* penguins do not have a square head.

Give the penguin a slightly oval head by setting the radius of the top corners to `70%` and the radius of the bottom corners to `65%`.

>Example Code
>
>```radius
>border-radius: 70% 70% 65% 65%;
>```

## Step 32

Target the `.penguin-body` element, and give it a `width` of `53%`, and a `height` of `45%`. Then, set the `background` to a linear gradient at `45deg`, `rgb(134, 133, 133)` from `0%`, `rgb(234, 231, 231)` from `25%`, and `white` from `67%`.

>Example Code
>
>```background
>background: linear-gradient(45deg, rgb(134, 133, 133) 0%, rgb(234, 231, 231) 25%, white 67%);
>```

## Step 33

Another interesting fact about penguins is that they do not have square bodies.

Use the `border-radius` property with a value of `80% 80% 100% 100%`, to give the penguin a slightly rounded body.

## Step 34

Target all descendent elements of the `.penguin` element, and give them a `position` of `absolute`.

>Example Code
>
>```penguin
>.penguin * {
>    position: absolute;
>}
>```

## Step 35

Position the `.penguin-head` element `10%` from the `top`, and `25%` from the `left` of its parent.

## Step 36

Position the `.penguin-body` element `40%` from the `top`, and `23.5%` from the `left` of its parent.

## Step 37

Change the stack level of the `.penguin-head` element such that it appears in front of the `.penguin-body` element.

>Example Code
>
>```z-index
>z-index: 1;
>```

## Step 38

To give the penguin body a crest, create a pseudo-element that is the first child of the `.penguin-body` element. Set the `content` property of the pseudo-element to an empty string.

>Example Code
>
>```pseudo
>.penguin-body::before {
>    content: "";
>}
>```

## Step 39

`Position` the pseudo-element relative to its closest positioned ancestor.

>Example Code
>
>```position
>position: absolute;
>```

## Step 40

Give the pseudo-element a `width` `half that of its parent`, a `height` of `45%`, and a `background-color` of `gray`.

## Step 41

Position the pseudo-element `10%` from the `top` and `25%` from the `left` of its parent.

## Step 42

Round off the crest, by giving the pseudo-element bottom corners a radius of `100%`, leaving the top corners at `0%`.

>Example Code
>
>```radius
>border-radius: 0% 0% 100% 100%;
>```

## Step 43

Increase the pseudo-element's transparency by `30%`.

>Example Code
>
>```opacity
>opacity: 70%;
>```

## Step 44

Start the penguin's face, by adding two `div` elements within `.penguin-head,` and giving them both a `class` of `face`.

## Step 45

Give the `.face` elements a `width` of `60%`, a `height` of `70%`, and a `background-color` of `white`.

## Step 46

Make the `top` corners of the `.face` elements have a radius of `70%`, and the `bottom` corners have a radius of `60%`.

>Example Code
>
>```radius
>border-radius: 70% 70% 60% 60%;
>```

## Step 47

Position the `.face` elements so that they are `15%` from the `top`.

## Step 48

Currently, the two `.face` elements are on top of each other.

Fix this, by adding a `class` of `left` to the first `.face` element, and a `class` of `right` to the second `.face` element.

## Step 49

Target the `.face` element with the `left` class, and position it `5%` left of its parent.

>Example Code
>.face.left {
>    left: 5%;
>}
>```

## Step 50

Target the `.face` element with the `right` class, and position it `5%` right of its parent.

>Example Code
>.face.right {
>    right: 5%;
>}
>```

## Step 51

Below the `.face.right` element, add a `div` element with a `class` of `chin`.

## Step 52

Target the `.chin` element, and give it a `width` of `90%`, `height` of `70%`, and `background-color` of `white`.

## Step 53

Position the `.chin` element such that it is `25%` from the top, and `5%` from the left of its parent. Then, give the top corners a radius of `70%`, and the bottom corners a radius of `100%`.

>Example Code
>
>```radius
>border-radius: 70% 70% 100% 100%;
>top: 25%;
>left: 5%;
>```

## Step 54

So far, the `.face` and `.chin` elements have the same `background-color`.

Create a custom CSS property called `--penguin-face`, and set it to `white`.

>Example Code
>
>```root
>:root {
>    --penguin-face: white;
>}
>```

## Step 55

Where relevant, `replace property values` with your `--penguin-face` `variable`.

Note: Change the existing `background-color` under `.face`, `.chin`

>Example Code
>
>```var
>background-color: var(--penguin-face);
>```