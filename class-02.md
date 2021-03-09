# Read 02 Notes

# Chapter 2 in Duckett HTML/CSS pg. 40-61
- Headings. h1 being the largest, h6 being the smallest.

             <h1> through <h6>

- Paragraphs

                    <p>

- Bold text. Surround a word or section of text that you would like to embolden.

        <p>
        I would like the last word of this sentence to be <b>bold.</b>
        </p>

- Italic text. Surround a word or section of text that you would like to italicize. 

        <p>
        I would like the last word of this sentence to be <i>italicized.</i>
        </p>

- Superscript. The superscript (sup) element's use is for containing characters like suffixes dates and/or math concepts. Like the rd in 3rd or 3 to the n power. Text slightly above the line.

- Subscript. The subscript (sub) element's use is to contain characters like periodic table element. Text slightly below the line. 

        <p>This 3<sup>rd</sup> of July we will have no rain, or H<sub>2</sub>0, in the forecast.
        </p>

        This 3rd of July we will have no rain, or H20, in the forecast.

- White space. There will naturally be white space in between each element. This is line spacing. White space collapsing is if you have too much space in your code but the content is contained in the opening and closing tag, it will still be rendered onto the webpage properly. Also, having separate p tags will trigger a line break. 

        <p>I don't really like white        space anyway!</p>
        <p>I don't      really like white space       anyway!</p>

        I don't really like white space anyway!
        I don't really like white space anyway.

- Line Breaks. Use this tag to cause text following the tag to drop to the next line. 

        <p>I don't <br /> like line breaks <br /> at all!</p>

        I don't
        like line breaks
        at all!

- Horizontal Rule. You can use this to break text that have a separate theme or topic.

        <p>Summer is for backpacking!</p>
        <hr />
        <p>Winter is for skiing!</p>

        Summer is for backpacking!
        --------------------------
        Winter is for skiing!

### Semantic Markup

- The **Strong** element can be used to indicate that this content is very important. 

        <p><strong>Watch Out!</strong> There might be alligators!</p>

        If you see an alligator, keep your distant. <strong>They will attack if provoked!</strong>

     **Watch Out!** There might be alligators!

    If you see an alligator, keep your distant. **They will attack if provoked!**

- The em element can be used to show emphasis on specific words to change the emphasis of a sentence by using italics.

        <p>I <em>don't</em> want a drink.<p>
        <p>I don't <em>want</em> a drink.</p>
        <p>I don't want a <em>drink</em>.

    I _don't_ want a drink.

    I don't _want_ a drink.

    I don't want a _drink_.

- **Quotations**

- Blockquotes. The blockquote element can be used in a situation where you have a quote that will take up a large space or an entire paragraph. This one will generally be indented by the browser.

- The q tag can be used to mark shorter quotes. You can use this one for more inline quotes. Both forms of quotations can cite a url. 

        <blockquote cite="url here">
        <p>Insert your quote here</p>

        <p>As Cookie Monster always says, <q>"C is for Cookie, that's good enough for me!</q></p>

- The abbreviation tag is used when you use and abbreviation or an acronym. 

        <p><abbr title="National Basketball Association">NBA</abbr><p>

        NBA

- The cite tag is used when you want to reference a book, movie, paper, newspaper, or anything else in this category.

        <p><cite>Book title goes here</cite> by xyz author has been published by abc publishing.</p>
        The text inside the cite tag will be in italics.

- The dfn tag defines a term that appears first in a text. Some browsers do not change the look of the text. 

- The address element is used to contain contact information for the author of a particular page.

        <address>
        <p><a href="mailto:BobLoblaw@blah.com">BobLoblaw@blah.com</a></p>
        <p>555 Phony Lane
        </address>

    _BobLoblaw@blah.com_

    555 Phony Lane

- The ins element shows text that has been added, the del element shows text that has been deleted.

        <p>This text was <ins>inserted</ins> while this text was <del>deleted</del>.</p>
        
        The ins will underline the word, the del will cross it off.

- The s element is shows something that is wrong, inaccurate, or has changed. 

        <p>Cookie Monster Puppet</p>
        <p><s>Price was $5,500</s></p>
        <p>Now it is $5</p>

        The second line will be crossed off.






# Chapter 10 in Duckett HTML/CSS pg. 226-245

CSS applies rules to your html elements by using a selector (ex: p, h1, etc) followed by a declaration (box) using the {} brackets. Selectors indicate what element you want to stylize and the declaration is how the element should be styled. A declaration is made up of two parts, a property (color:, font-family:, etc.) and values (color: yellow;, font-family: Arial;). You can use multiple elements in a CSS rule, so:

            h1, h2, h3 {
                font-family: Arial;
                color: yellow;
                }

The link element can be used in html to tell your browser where to look for the CSS file you are using to style the page. 

        Place the first line of code below in your head element.
        <link href="style.css" type"text/css" rel="stylesheet">

        - href - specifies path to CSS file
        - type - the type of document being linked to.
        - rel - indicates the relationship between the file you are linking to and the html.

You can also include CSS styling in your HTML code by using the style element or tag. You can place CSS rules within this tag directly in your HTML code. This tag should sit inside the head tag or element.

You can select a class in your CSS document by using the class selctor. This is indicated by a . before the selector.
       
        - * is a universal selector and applies to all elements

**You can use one CSS sheet to apply to a website with multiple pages.**



# Chapter 2 in Duckett JS/JQuery pg. 53-84

### Statements

        let today = new Date();
        let hourNow = today.getHours();
        let greeting;

        if (hourNow > 18) {
          greetng = 'Good Evening World!';
        } else if (hourNow > 12) {
          greeting = 'Good Afternoon World!';
        } else if (hourNow > 0) {
          greeting = 'Good Morning World!';
        } else {
          greeting = 'Welcome!';
        }

        document.write('<hjs>' + greeting + '</hjs>');

In the js example above, you will see an example of a varied greeting. The lines beginning with let, greeting, and document are statements. The curly brackets indicate the beginning and end of a code block. The else if lines determines what code will run in this order. 

**Statements** are one to a line, you must have only one statement per line and the statents are, in a nutshell, instructions.

- Each one is a single instruction that the computer will follow. 
- Each one begins on it's own line and will end with a ;
- The ; is important at the end of your code since it will tell the js interpreter that the instruction is complete telling it to go onto the next instruction or step.
- **Code blocks** are statements that are contained with curly brackets. Each code block in the example above only contain one statment, the time. Code blocks are used frequently to contain multiple statements. Also, this makes it much easier to read your own code.
- You can write comments in your code to help better understand what the code is supposed to do.

**Multi-Line comments** - These will encompass more than one line. Open with /*, write your text, then close with */.

**Single-Line comments** - Anything that you type past the // on that particular line will not be processed by the Javascript interpreter. These are used for what this line of code is doing. 

### **Variables**

- Variables are places where pieces of data can be stored temporarily from a script. 
- Once you leave a page, the data will be dropped from the browser memory. 
- The name, variable, is a good label for this idea since the data can change every time you visit the page and the script runs. 
- The variable can be computed or calculated in the interpreter using the data that is temporarily stored in the variable.

            var quantity = 3;

- **In the example above**, we have the keyword, var. (This keyword is used to create a particular variable.) The Javascript interpreter will understand that this keyword will create a variable. 
    - **var is the keyword**

    The variable name is, in this case, quantity. This is also known as an identifier. 
        
    - **The variable name is quantity.**

    _Note: If there is more than one word in your variable name, or identifier, you have to use what is called camelCase where any additional word is started with a capital. So, hourNow, camelCase, etc._

- The equals sign is the assignment operator. This example assigns a value to the variable. The 3 above is the variable value. If there is no value indicated, this variable is undefined.

### JS identifies the differences between strings, numbers, and Booleans, Booleans being true or false values.

 - **Numeric Data** handles numbers. You can only use characters 0-9. No commas are written in your numbers. You can also have negative numbers. Three quarters will be conveyed as 0.75

 - **String data** handles letters and other characters. These can be used for any type of text. Use matching ' or " on either side of your text. 

 - **Booleans** are true of false, on or off. For example, if an item is in stock or not, this is a true or false, yes or no value. 

 ## Six Rules for Naming Variables

1. The name needs to start with a letter, $, or _. Cannot start with a number.
2. The name of the variable can contain letters, $, or _. You cannot use a - or . in the name.
3. You are not allowed to use two things: reserved and keywords. See above for keyword definition. 
4. Variables are case sensitive. So, starting the same word uppercase and lowercase are two different variable names. It's not good methodically to use the same word for two different variables. 
5. Use like variable names for the information you are storing. 
6. Make sure you use camelCase when typing more than one word. 


# Chapter 4 in Duckett JS/JQuery pg. 145-162




[Back to code 201 Table](code201Table.md)

[Back to Homepage](README.md)