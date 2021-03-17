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



[code201Table](201/code201Table.md)

[Back to Homepage](README.md)