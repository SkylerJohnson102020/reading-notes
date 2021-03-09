# Read 02 Notes

## Chapter 2 in Duckett HTML/CSS pg. 40-61
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






## Chapter 10 in Duckett HTML/CSS pg. 226-245



## Chapter 2 in Duckett JS/JQuery pg. 53-84



## Chapter 4 in Duckett JS/JQuery pg. 145-162




[Back to code 201 Table](code201Table.md)

[Back to Homepage](README.md)