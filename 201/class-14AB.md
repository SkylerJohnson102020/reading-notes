# CSS Tranitions and Transforms
###Read14 A & B

What is interesting about the first article is that there was no evidence to suggest that any particular make up of people or process of carrying out the group worked best. They just seemed to work. The thing that researchers concluded was that the key to improving the teams at Google was to understand and influence the group norms. What distinguished the teams that worked well and the ones that didn't was the way people treated one another. In teams that functioned well togehter, two things occured. Members took the same amount of time to speak speaking equal amount of time. Leadership would also shift depending on the task on some teams. A team with no personal connections or even simple friendly exchanges is set up to not work well. Humans need to have psychological safety and comfort. By opening up just a little, it helps us to start breaking through to that safe feeling in the team. Sharing personal feelings, experiences, or a simple laugh can do wonders.

## CSS Transforms

https://learn.shayhowe.com/advanced-html-css/css-transforms/

The _transform_ property offers a lot of techniques. Two dimensional and three dimensional settings. 

Transform Syntax - 
    article {
        -webkit-tranform: scale(0.0);
        - -moz-transform: scale(0.0);
        -o-transform: scale(1.0);
        transform: (1.25);
    }

The prefixes above help to cover broswer support.

2D Transforms
They work on x and y axes/horizontal and vertical.

_rotate_ has the ability to rotate an object 360 degrees. They can take a positive or negative number.

        .square1 {
            transform: rotate(10deg);

        }

2D Scale - _scale_ value has the ability to make an element appear smaller or larger. Default is 1, more will enlarge, less will shrink.

        .square1 {
            transform: scale(.75);

        }
        .square2 {
            transform: scale(1.25);

        }

You can also change the height (scaleY) and width(scaleX) of an element. shorthand to include both values.

2D translate - the translate value moves an element without disrupting the normal flow of elements. Similar to releative positioning.You can also use scaleX and Y on this.

2D skew - Distort and element my skewing. Distorts the vertical and/or horizontal axis. Set values to positive or negative deg.


Combining Transfroms - You will have to use the shorthand version if combing multiple values. You cannot have multiple transform declarations since the last one listed will overwrite the others. Include them in one declaration.

        .square1 {
            transform: rotate(10deg) scale(.50) skew(15deg, 25deg) translateY(5px);

        }

Transform Origin - Default is in the exact center of an element. You can change this using the _transform-origin property. Can accept 1 or 2 values. 

Perspective - You need this for **3D** transforms. Use the _perspective_ value within your _transform_ property. Use px for this value. Perspective Depth Value is a length measurement. Setting it to _none_ will turn off perspective. The perspective appears deeper/farther when the value is high, not as far when the value is low. Perspective origin is a value applied to the transform property, use _perspective-origin_. This is just like transform origin. 

## 3D Transforms 

3D Rotate - We give an objext an x,y, and z axis. So, use rotateX, rotateY, rotateZ for example. 

3D Scale - 

3D translate - translateZ for example.

3D skew - 

Shorthand 3D Transforms - Look at article for reference.

Transform Style - _transform-style_ property with the _preserve-3d value will help transform a child element nested within a parent.

Backface Visibility - This flips the element which makes it look like it's facing away from the screen. Use the _backface-visibilty_ property. Setting this to hidden will hide the element.

## CSS Transitions and Animations

https://learn.shayhowe.com/advanced-html-css/transitions-animations/

You will be using the transition property for this. Pseudo classes include :hover, :target, :active, :focus. Four total transition properties:

1. transition-property
2. transition-duration - time it takes to make the full transition. Value in seconds or milliseconds. Use commas to separate multiple values.
3. transition-timing-function - The transitional speed movement, how fast it will move. Keyword values include linear, ease-in, ease-out, and ease-in-out. Linear is constant speed, ease-in starts slow then speeds up, ease-out is the opposite, ease-in-out slows at both ends of the transition. **cubic bexeir curve** more in article. use commas to separate values.
4. transition-delay - This sets a delay on the transition. Seconds or milliseconds.
5. shorthand transitions - you can put all properties on one line with values with separting with commas.

Use your vendor prefixes to ensure that all browsers will be able to support this. Essential, repeat the same properties each time using: -webkit-, -moz-, and -o- before each transition declaration.

**Transitional Property**

The _transition-property_ determines what will be impacted. The background in the example below will be the only value impacted by duration and linear.

        .square1 {
            background: red;
            border-radius: 4px
            transition-property: background, border-radius;
            transition-duration: 2s;
            transition-timing-function: linear;
        }
            .square1:hover {
            background: blue;
            border-radius: 45%;
        }

**Not all properties can have a transition property,** 

**List of popular transition properties in the article.**

Transitional buttons bring a nice touch to a website. See article for code example.

### Animations

Use the @keyframes rule for this. These must be vendor prefixed. Many of the same or similar properties exist in this conept. Animation-name, -duration, -timing-function, -delay, -iteration-count, -direction, -fill-mode,


## 8 simple css transitions

https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users

1. Fade-in
2. Change color
3. Grow and shrink
4. Rotate
5. Square to circle
6. 3D shadow
7. Swing - (a lot of code....)
8. Inset border


### Other CSS resources

Animated Buttons - https://codepen.io/retyui/pen/ByoaXV

CSS animations, @keyframes - https://codepen.io/akshaychauhan/pen/oAfae

404 animation - https://codepen.io/kieranfivestars/pen/MYdQxX

Bounce Animation - https://codepen.io/dp_lewis/pen/gCfBv

[code201Table](./201/code201Table.md)

[Back to Homepage](README.md)