# Read 04 notes Links

**Links** You can create a tag using the a tag, or anchor element. Makes it a clickable link.

        <a href="url here">Website Title</a>

Generally you create a list comprised of of links, primarily for a links page or your nav bar. Usually in a ul.

**For an email**

    <a href="mailto:skyler@blah.com">Email Skyler</a>

**target** is an attribute used to open your link in a new window. To do this, set the value of target to _blank.

        <a href="url here" target="_blank">Website Title</a>

**Linking to spots on the same page** in the case that your page is long, you can add a list of links to jump to different portions of the page using the id att.
    
    <h1 id="top">Title</h1>
    <a href="#1st drop">1st drop</a>
    <a href="#2nd drop">2nd drop</a>
    <a href="#3rd drop">3rd drop</a>

    <h2 id="1st drop">1st drop</h2>
        some text here
        jjhdhsjkhfkashfjk
        asfhasjkhaklhfk
    <h2 id="2nd drop">2nd drop</h2>
        slkfasklfnsaklf
        ldknkssklsfkl
        slkdlksjkldsnfk
    <h2 id="3rd drop">3rd drop</h2>
        flashfljashfaljkh
        asklfhjalksfhslka
        aslkjfhakjfal
    <p><h2 href="#top">To Top</h2>


# Chapter 15

**Blocks** We have covered this subject multiple times, but here is a summary.  

**Block-Level** elements will start on a new line and act as your primary building blocks to shape your page. Ex: h1, p, ul, li.

**Inline elements** the boxes will shape around and between your text. img, b, i. 

Separate your boxes in css using border, margin, padding, background colors, etc. 

**Containing Elements** A block-level element nested inside of another block-level element is known as a parent (containing) element. You can use the div element to separate the child boxes.

**Positioning** In CSS using the _position_ property.

- Normal Flow - Typically if you apply nothing. All of your block-levels will appear on a separate line. They will just drop down vertically one from the next. 

        p {
            positon: static;
        }

- Relative Postioning - This will shift a block-level in relation to where it would be in normal flow. Use position relative, the adjust top, right, bottom, and left. 

        p {
            positon: relative;
            top: 25px;
            left: 75px;
        }

- Absolute Positioning - This takes a block-level element out of the flow and does not impact the postion of the other elements. It is like it isn't on the page. Make sure you apply top, right, bottom, left. Postion things so you don't have overlap.

         h1 {
            positon: absolute;
            top: px;
            eft: px;
            width: ox;
        }
            other elements {
            adjust to not overlap.
            width:
        }

- Fixed Position - keeps an element in the same place even if you scroll. This would me like your main header staying at the top despite where you scroll. 

        h1 {
            positon: fixed;
            width: 100%; 
            set a color, padding, margin
        }

- z-index - use this for overlap. An element with a higher number on the z-index will put the appearance over top of an element with a lower z-index value. 

        h1 {
            z-index: 8;
            this one is on top
        }

        p{
            z-index: 3;
            this is underneath
        }

- float - This will help you to move a block left or right. If you want text to float around an image, this is what you will use. To float multiple boxes side by side, you will want to use your width property in css. 

- clearing floats




[Back to code 201 Table](code201Table.md)

[Back to Homepage](README.md)