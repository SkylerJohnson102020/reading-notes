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

**Centering**

Centering a box on a page is simple. Just set the left and right margin to auto. You also need to set a width otherwise the box will span across the entire page.

        <p> {
            left-margin: auto;
            right-margin: auto;
            width: 300px;
            padding:
            border:
        } 
            
You can also use **text-align** for older browsers. Use this and set it to centered. This property will impact child elements as well as the parent so make sure you use a class or id tag in your html. 

**IE6 Model** (Internet Explorer 6) You set the width size of a box, generally you add padding and margin. **However**, IE6 is funky and will include the padding and margin in the width of a box. 

**Display: Inline and Block** You can use the display property to turn a list or some other inline element into a block element. You can also go block to inline. In addition, you can hide something. 

- Inline - turns a block element into inline (not generally used to create block elements.)
- Block - turns inline to block
- none - hides element from page

     <ul>
        <li>Turkey</li>
        <li>Stuffing</li>
        <li class="extra">Mashed Potatoes</li>
        <li>Gravy</li>
    </ul>   

    li {
        display: inline;
        margin-right: 5px;
    }     
    .extra {
        display: none
        visibility:
    }

    Turkey  Stuffing  Gravy

**Hiding Elements: Visibility, hidden or visible**

    - The hidden property will hide element.
    - visible shows the element. 

If the visibility property is set to hidden, a blank space form in it's stead. If you want it visible, set the property to none.

**Border-Image** property does exactly that, applies an image to the border. This property is done in 3 steps.
    
    1. set a url
    2. where to cut image
    3. straight edges are done with these possible values:
        repeat - which does exactly that, repeat it.
        round - this will scale the image so tiles will meet properly.
        stretch - exactly that, stretches the image.

        p {
            - moz-border-image: url("images/dots.gif") 8 8 8 8 round;
            - webkit-border-image: url("images/dots.gif") 8 8 8 8 round;
            border-image: url(images/dots.gif") 8 8 8 8 round; 
        }

**box-shadow** does exactly that, set a shadow that drops back from a box. It must include the **Horizontal and Vertical** offset properties. You also add color. Horizontal, the negative value below places the shadow to the left of box. Vertical, negatives will put shadow at top of box. **Blur distance** will blur shadow, if not present, the shadow will sppear solid. **Spread of Shadow** when applied, a value in the positive will expand, negative will contract on all four sides. 

        p {
            - moz-box-shadow: -3px -3px red;
            - webkit-box-shadow: -3px -3px red;
            box-shadow: -3px -3px red; 
        }

**Border-radius** will round the corners on a box use border-top, -left, -bopttom-, etc. you can set one border-radius to a pixel value. 

**Elliptial Shapes** border-radius for custom shapes. This is a complex application, so refer to **page 322 in the Duckett**. For a circle as a quick example, you set the vertical and horizontal values the same. 


# Arrays

Arrays will store many values rather than just a single. Consider using this when you are using a list or collection of values that are related. You can store anything and they don't need to be the same. So, numbers, strings, and booleans can be mixed together. This example below is called array literal, all in one line. You can also do array constructor, in the second example. The second one creates the new keyword and the Array(). Values are then dropped into the (). 

        let colors;
        colors = ['blue', 'brown', 'yellow', 'custom'];

        let colors = new Array('blue', 
                  'brown', 
                  'yellow', 
                  'custom');

**Values in the Arrays** Applying number, or **index**, to the values, you have to remember that **we start at zero.** So in the second exapmle, blue is 0, brown is 1, yellow is 2, and 3 is custom. It doesn't matter if you use the array literal or constructor methods. 

    let colors = new Array('blue', 
                  'brown', 
                  'yellow', 
                  'custom');

    colors[3] = 'darkcyan';


**if statements**

Below is an example of an if statement. This type of statement will check into a condition (test score >= 75). If this condition returns true, then any of the statements (passed()) that follow in the code block will run. So:

        if (test score >= 75) {
            passed();
        }

Below is an example of an if else statement. This one will also examine a condition. If it returns true, then it will run the first statement, or code block. If it returns as false, the next code block will be run. The (test score >= 75) is the condition.

        if (test score >= 75) {
            passed();
        }
        else {
            not passed();
        }

## Switch Statements

The switch statement will begin with a variable that is called _switch value_. In the example below, each possibility is indicating what could possibly the value for this particular variable including the code that will run if the condition is met. 

        switch (stage) {
            possibility 'One':
              title = 'Stage 1';
              break;

            possibility 'Two';
              title = 'Stage 2'
              break;

            possibility 'Three';
              title = 'Stage 3'
              break;

            default:
              title = 'Testing'
              break;
        }

An if statement will run the entire code and then determine which condition is met. The switch statement will run through and will stop when it reaches 'break' once it finds the match. Switch statements generally run faster than if statements. 

**Type coercion** the conversion of data types to meet complete a particular operation. Example it is better to use === or !== since these two operators will check if there is a strict match. This gives less unintended values.

**Weak typing** JS uses this since the type of data can change.

**Strong =typing** others require definition of what data type the variable is. 

**Falsy values** - values treated as false. Any falsy value can be treated as 0. 

**Truthy** - values treated as true. (pg. 167) Truthy can also be 1. Pretty much everything comes out as a truthy value. Having an object of array in your code is considered truthy.

**Short Circuit** values stop running through the code once a result has been reached. If it is finding a truthy and you have three values 0, 1, 2, it will go through 0 since it's falsy and stop, short-circuit, on 1. You typically want to order your code considering this. For the logical OR operator, put code that will return true or most likely will first. In logical AND, put the false returns first. 


# Loops
    
- for - running code for a specific number of times, like an incorrect password. This one is a counter, meaning it will count your incorrect answers. This will be told by the condition how many times the loop should run. 

- while - a loop where you have no idea how many times it should run. This loop will continue until the condition is met and returns true. 

- do while - the do while loop, closely resembling the while loop, has one difference. it will run statements at a minimum of at least once even if it returncomes backs false.

# Loop Counters

**Statements within the for loop**

- Initialization - we set our variable to 0. Our variable is called i. and it behave as our counter. This is our starting position. Starts at 0.

        ver i = 0;

- Condition - the for loop will run until it hits outour specified number. If we start at 0, the loop will run 5 times, 0, 1, 2 ,3 ,4 ,5, undefined.

        i < 5;

- Update - we add one to our counter after each time the loop runs.

        i++

SO;

        let i;
        for (i = 0; i < 5; i++){
                "code"
        }


[Back to code 201 Table](201/code201Table.md)

[Back to Homepage](README.md)