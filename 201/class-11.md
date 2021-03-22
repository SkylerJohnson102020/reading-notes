# Chapter 16

            display: block

    Above will turn an image into a block level element.

    For a background image:

            body {
                background-image: url("enter url here");
            }

### The background-repeat allows you to have four values:

repeat - exactly what it does, repeats horizontally and vertically.

repeat-x - horizontal only

repeat-y - vertical only

no-repeat

fixed - a fixed position on page

scroll - the image scrolls

Use the background-position and add value of left top, left center, left bottom, center top, center center, center bottom, right top, right center, and right bottom. Use % to adjust as well.

**Shorthand background**

        main {
            background: blue url("enter here") no-repeat top left;
        }
        
Specify properties in order below:
background-color
background-image
background-repeat
background-attachment
background-position

Rollover - Three different changes to image, standard, when the user hovers over it, and when the user clicks. 

Sprite -  image used for multiple parts of interface. 

CSS3 gradients - for a gradient, you have to specify the two colors that the gradient should set between. you need to use the background-image property and use your -webkit and -moz. See code example on **page 419**.

Contrast background images - If you want your text to appear over an image, generally you will want low contrast applied to your image.

Use a large element (html, body) to apply general properties and give is an id or class of **wrapper**. 


[code201Table](201/code201Table.md)

[Back to Homepage](README.md)