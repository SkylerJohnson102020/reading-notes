# Chapter 15

**Block-Level** elements will start on a new line and act as your primary building blocks to shape your page. Ex: h1, p, ul, li.

**Inline elements** the boxes will shape around and between your text. img, b, i. 

Separate your boxes in css using border, margin, padding, background colors, etc. 

**Containing Elements** A block-level element nested inside of another block-level element is known as a parent (containing) element. You can use the div element to separate the child boxes.

**Positioning** In CSS using the _position_ property.

- Normal Flow - Typically if you apply nothing. All of your block-levels will appear on a separate line. They will just drop down vertically one from the next. 

        p {
            positon: static;
        }

- Relative Postioning - This will shift a block-level in relation to where it would be in normal flow. Use position relative, the adjust top, right, bottom, and left. An example would be to shift an a block of text (p) to the right on the screen, I would set left to 75px or maybe as a percentage to indent the paragraph. This positions the text releative to it's parent element.

        p {
            positon: relative;
            top: 25px;
            left: 75px;
        }

- Absolute Positioning - This takes a block-level element out of the flow and does not impact the postion of the other elements. Make sure you apply top, right, bottom, left. This will have a fixed placement on the page and will move with the scrolling of the page. This will have no impact on the other elements' flow.Postion things so you don't have overlap. The CSS below places this element relative to it's parent.

         h1 {
            positon: absolute;
            top: px;
            left: px;
            width: px;
        }
            other elements {
            adjust to not overlap.
            width:
            z-index: (to not overlap)
        }

- Fixed Position - ("sticky header") This keeps an element in the same place even if you scroll. This would me like your main header staying in the middle of your page over text and does not move. Not an ideal placement, but maybe small bits of info or a heading you want the user to continue to see as they scroll.

        h1 {
            positon: fixed;
            width: 100%; 
            set a color, padding, margin
        }

- Floating Elements - Use this to float text left or right of another element. This takes it out of normal flow and allows other block-levels to flow around the floated oject.

- z-index - use this for overlap. An element with a higher number on the z-index will put the appearance over top of an element with a lower z-index value. Basically makes an element more or less transperent. 

        h1 {
            z-index: 8;
            this one is on top
        }

        p{
            z-index: 3;
            this is underneath
        }

- float - This will help you to move a block left or right. If you want text to float around an image, this is what you will use. To float multiple boxes side by side, you will want to use your width property in css. You are taking this out of normal flow and placing it typically on the far left or right of the page. Perhaps an image that you want text to float around an image. If you want an image to be on the right hand side, you would simply do float: right; There are more adjustments afterward, but this is where you start. 

- Using floats for side by side elements. Taking multiple p elements and floating them to be side by side can be tricky, so you will want to work with obviously setting float left or right and then adjusting your height and width of all of your p boxes to be the same. This will help your flow.

- Clearing floats - Is way to tell all of your elements in a parent element not to touch wither the left or right side of each box. 

        clear: left, right, both, or none;

Left will make the left hand side of each box will not touch any others in that box. Same with setting it to right. Both will set it to both sides cannot touch. None, elements can touch.

- You can create multi column layouts with floats. Using width (width of your column), float (to position the columns next to eachother), and margin (gap between columns). You can target each one with a class tag or call them all in one css {}.

Screen sizes - keep this in mind when constructing your data. Phones all the way up to large screens. This impacts how much content a user will see.

Screen resolutions - Number of dots per inch a screen displays.

Page sizes - An interesting concept. This is like see a newspaper that is folded and all you see is the top half of the front page. Think of your webpage in this sense. When a user opens your page, they aren't going to see EVERYTHING right away on your page. You need to grab their attention in the upper portion. Generally, you want to tell your user in a space of about 570-600px what it is you want them to know, and then make it enticing enough for them to want to know more. You can't cram too much and make it looked chaotic, be clear. If you give the user a little bit of what is at the bottom of the page they will want to scroll.

Fix-width layouts - This typoe of design doesn't change in size when a user adjusts the size of the browser window. Measurements are in px. Advantage, this is a very accurate method that allows the designer to have a lot of control over the site. The items will stay the same size depite the size of the window.

Liquid layouts - adjust to the size of the browser window. These use measurements in %. This method can eliminate the potential for large spaces on the page, % fills these gaps. A disadvantage is the use of smaller screens. Content can overflow over other content. For a wide screen, this can result in very long lines of text stretching across the window. 

Layout grids - webs designers use a 960 px grid to superimpose lines on the page to help create a layout. Examples on page 389. 

CSS frameworks - To create a grid, set a class to the container holding the entire content of the page, set the class to container_12. This will set your page to be 960px wide. You can grab a 960gs stylesheet at 960gs.com page 391. Adding _clearfix_ to your class will ensure your browser to the containing box heighth since it contains floating elements only. 

Multiple Style Sheets - You can have your html use one stylesheet linked in the head as usual. Then, you can import other stylesheets by using: @import. Or, you can link each stylesheet into the head of the html. **These imports must happen before any other rules are set, place this at the top.** 

        @import url("colors.css");
        @import url("tailwind.css");

With all stylesheets, if you have multiple rules applied to the same element in different places on different stylesheets, the rules that appear later, or last, will be used over the previous rule(s).

[code201Table](201/code201Table.md)

[Back to Homepage](README.md)