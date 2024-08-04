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