# Read 03 Notes Lists, Boxes(Plus Table Row Element), Shorthand CSS, Arrays, Decisions, and Loops.

## Chapter 3 pg 62-73 Lists

### Lists

- 3 types of lists: ol, ul, and dl.

**Ordered Lists**

    <ol>

**Ordered List**: All of the list elements must be contained with the ordered list tag. All items will be numbered in this element.

    <li>

The li tag is used to list individual items.

        <ol>
        <li>Turkey</li>
        <li>Stuffing</li>
        <li>Mashed Potatoes</li>
        <li>Gravy</li>
        </ol>

        1. Turkey  
        2. Stuffing
        3. Mashed Potatoes
        4. Gravy 

**Unordered List** use ul tag.

        <ul>
        <li>Turkey</li>
        <li>Stuffing</li>
        <li>Mashed Potatoes</li>
        <li>Gravy</li>
        </ul>

        - Turkey  
        - Stuffing
        - Mashed Potatoes
        - Gravy 

**Definition Lists** use the dl tag. The dl tag will contain all of the contetn, but there are two other tags that go along with this. The dt tag will contain the term you want to define, the dd tag will contain the definition.

        <dl>
            <dt>Jetboil</dt>
            <dd>A brand of stove used to cook food while hiking or camping. Typically use for backpacking.</dd>
            <dt>Bivy</dt>
            <dd>Short for Bivouac Sacks. This is used for an extra layer against the elements for a sleeping bag.</dd>
            <dt>Mountain House</dt>
            <dd>A brand of freeze dried meals popular among hikers.</dd>
        </dl>

            Jetboil
                A brand of stove used to cook food while hiking or camping. Typically use for backpacking.
            Bivy
                Short for Bivouac Sacks. This is used for an extra layer against the elements for a sleeping bag.
            Mountain House
                A brand of freeze dried meals popular among hikers.

**Nested Lists** You can put an additional list inside the li tags of another list.

        <ul>
            <li>Tent</li>
            <li>Sleeping Bag</li>
            <li>Food</li>
                <ul> 
                    <li>Mountains Houses</li>
                    <li>Granola</li>
                    <li>MTrail Mix</li>
                </ul>
            <li>Sleeping Pad</li>
            <li>Pack</li>
            <li>Water</li>
        </ul>

## Chapter 13 Duckett: Boxes in CSS

A box will fit naturally around the edges of text. To change this, use **box dimensions**: height and width.

        div {
            height: 250px;
            width: 350px;
            background-color: orange;
        }
        p {
            height: 60%;
            width: 60%;
            background-color: tan;
        }

Using % will make your box size relative to the window in the browser. Using ems will base the size of the box off the size of the text contained in that box.

**Limiting Width** this is your min-width, max-width. These are great for limiting how wide or how narrow the text and other contents will expand or shrink the size of the browser. You don't want your text to be so wide or narrow that you page in illegible. 

        td.description {
            min-width: 100px;
            max-width: 275px;
            text-align: left;
            padding: 7px;
            margin: 1px;
        }

        The above example was being applied to a Table Row element. <tr></tr> with the table data cell element <tr></tr> contain within it.

 **Limiting Height** use min-height, max-height. This will limit the height of your box, exactly like width. 

        p {
            min-height: ;
            max-height: ;
        }


**Overflowing Content** This will help prevent your page from looking scrunched or messy. This property will help us let the browser know how to handle our content in a box is too large than the box. We have two options: hidden or scroll. Hidden will hide any content that won't fit. You text may just randomly stop and you will have to enlarge the browser window to see the rest. Scroll gives you the option to scroll through all the text despite the small box.

        p {
           overflow: hidden; 
        }
        p {
            overflow; scroll;
        }

**Border, Margin, and Padding.** You can adjust every box using these main properties. This was covered in 102. 

See [code102 Reading Notes](code102Table.md)

**Border Width** can be fun. Two sides of your box border can have a different thickness, a generic setting, or all four sides. **If all four sides,** your order of border side is always:

## **top, right, bottom, left** 

        p {
            border-width: 1px;
            /* controls thickness on all sides */
        }
        p {
            border-width: thick;
            /* the entire border is given a generic thick setting */
        }
        p {
            border-width: 3px 2px 10px 6px;
            /* each side has a different thickness. */
        }

**Border-styles** There are many different border styles like solid, dotted, dashed, groove, double, outset, inset, ridge or hidden/none. **You can select a different style for each side of the box. Again:**

## **top, right, bottom left**

**Border-color** was covered in code102. See above link to see those notes.

# Shorthand 
### Specify multiple characteristics in one property.

**Border** You can put all properties in one line of code.

        p {
            width: 100px;
            border: 4px ridge darkcyan;
        }

**Border Color** Remember top, right bottom, left

        p {
            border-color: red, salmon, darkblue, black;
        }

**Border** 

        p {
            width: 100px;
            border: 3px inset green;
        }

**Padding** top, right, bottom, left (pg 313)

        p {
            width: 50px;
            border: 2px ridge blue;
            padding: 10px 5px 10px 5px;
            /* or you can use */
            padding: 10px;
            /* this will change all sides to 10px */
        }

**Margin** clockwise: top, right, bottom, left. For margin you can apply just two numbers. The first number will cover top and bottom, the second will cover left and right.

        p {
            width: 150px;
            border: 3px ridge green;
            padding 5px;
        }
        p.example {
            margin: 25px 15px;
            /* or */
            margin: 25px 15px 25px 15px;
        }






# Arrays






[Back to code 201 Table](code201Table.md)

[Back to Homepage](README.md)