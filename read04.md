# Read 04 Notes HTML

# Duckett Chapter 18
## Who is your site for?
#### Ask Yourself:
- Age range of my target audience
- Average income of visitors
- What part of the country do they live? A different country?
- How often are they on the internet?
- Occupations?
- Level of education of visitors
- Hours of work per week
- What device are they using to access your site?

#### For target companies
- What is the size of the company?
- Position of people within the company who visit the site?
- How large of a budget does this company carry?

#### Why people visit my site?
There are **two basic categories** to keep in mind
1. What is the motivation behind an individual visiting my site?
2. What are the goals of these visitors when visiting the site?

#### What information do my visitors want to see?
- Are they familiar with your brand or do you need to explain yourself?
- Will they know your product or do you need to give an explanation?
- What are the most important features of what you're selling?
- What makes you different from others who offer something similar?
- Are there FAQs about your site from visitors?

Some sites need more updates then others depending on what they're about. Something like a sports website like Bleacher Report will have to update more frequently since many new events happen everyday. A roofing company won't need to update as frequently. One needs to determine how often to update in order to keep people visiting.

## What do I do now?
- Create a site map 
    - A site map is a diagram of the all the pages you are using to       strucutre you site.

- Card Sorting
    - Card sorting is a technique to help you decide what goes where. Essentially creating a map of where everthing is categorically.

- Wireframing
    -This is drawing of how each page should appear. This can even be drawn on a piece of paper. This will help give you a better idea of how each page will look. Consider it like a blueprint. 

- Organization 
    - You will have a lot of information, make sure you think clearly about how you want to organize all of this info in a way to where it appears clear and readable. You can group content blocks together to help accomplish this.

- Distinction
    - Make other parts more distict to either draw attention to or from something.

## Visual Hierarchy
 - Where do you want to visitior to look first when visiting a page? Where does the visitor's attention go first? This refers to the order in which a vistior's eyes see the site. It what order are your items seen? Make sure you use size, color, and style to accomplish this.
    - Size, specifically larger items. Larger items like large text or heading can grab attention.
     - Color - Either foreground and background color can draw attention to something you're wanting to highlight. Brighter sections tend to draw visitors in first.
     - Style - A specific item may blend too well into the page and maybe needs to need more style. An example of this is playing around with fonts when you want something to stand out. 
    
    - Images are huge when it comes to Visual Hierarchy. These often catch the viewer's attention first. 

- Balance - make sure you have balance in your site to make things look even. there are many ways to achieve this through all elements. Nothing specific here, just make sure you keep this mind.

## Grouping and Similaritry
    - Proximity - If items are close together, they are viewed as related.
    - Closure - If we have a more complicated arrangement or shape of items, we will look for single patterns, or look more closely at the content.
    - Continuance - These items appear to have direction, thus also appear related. This can be used to lead a viewer in a direction.
    - White space - less space between related items, more space to separate unrelated items.
    - Color - Color behind related items to further show their relation.
    - Borders - These can be used to groupd items.
    - Consistency -  put text in multiple blocks in the same style but with white space separating them.
    - Headings - Give a paragraph a larger heading to show this distinction

## Navigation
Site navigation gives your viewers a map of where to go. Make sure you are concise, clear, and selective with this. There are three different types of navigation. **Primary** navigation most likely will appear across the top of a page or left or right. **Secondary** navigation might be underneath the primary navigation. **Tertiary** navigation is most often at the bottom of page in the footer. Make sure you offer context, do you navigation names offer intrest, curiosity, or tell a story? Be clear with this. Make sure the links are large enough and visible. Make sure in the **primary** navigation bar that there is a color highlighting, an arrow pointing, or some other way to communicate to the viewer where they are on your page.


Html stands for **Hypertext Markup Language**. Html is the structure of a website. Stictly using html is not very pretty to look at as it is only the structure. All you will see is mainly text and perhaps some photos. CSS is how we stylize our website, but we will get into that later. Html is comprised of a lot of tags. These tags contain an opening and closing tags, attributes, and you include contents as well.

There are many tags that you can use and there are many different types of tags. There are many different types of basic tags, formatting tags, form and input, images, links, frames, lists, tables, and the list goes on from there. First things first, you have to start your file with a DOCTYPE command, and certainly select html.

## Chapter 8 Extra Markup
- If you want to add in a message into the code that the viewer will not see, the contents of the tage should begin with ! and double -- on either side, so:

            <!-- message here -->

These are good as working messages for when you come back to work on your code, you give yourself a little guidance on what to do next.

- ID attribute - Also know as **global attribute**, because this can be used on any element. So:

            <p id="pullquote">

- Class Attribute - a single attribute that can impact multiple elements. "Class"

- Block elements - These elements appear to start on a new line in the page, you will see white spacing. examples include:

            <h1>, <p>, <ul>, and <li>

- Inline elements - these elements appear to continue in the same line or text so the surrounding elements. Examples include:

            <a>, <b>, <em>, and <img>

- Grouping Text and Elements in a Block - this is the **"div"** tag. This tag helps you setup elements in a block-level box. You might use this to contain all elements for your header or use it it contain comments from visiors. 

- Grouping Text and elements inline - the **"span"** tag. You can use this in two way:
1. To contain a chunk of wording where there is no element to help differentiate it from the other text.
2. Use it to a contain multiple inline elements.

This tag will help people control the look of the content in CSS.

- IFRAMES - this tag **"iframe"** can bring a small window of another webpage onto your page. Like when google maps appears on a lot of restaurant listings. Common attributes you can use for this are:

            src= helps direct a certain url into your page to show in the small window
            height= height of frame
            width= width of frame
            scrolling= scrolling is not supported in HTML5. HTML4 or XHTML shows wheter or not the frame will have scroll bars. You can add three values to thi att.
                1. Yes, to show scroll bars
                2. No, to hide them
                3. Auto, to show if needed
            frameborder= not supported in HTML5. Shows in other versions if the frame should have a border or not.
            seamless= this can be applied to an iframe if scrollbars are not necessary. No value is needed to be added to this attribute.

- Information about your pages - the **meta** tag or element is contained inside the head. This will contain info about the webpage. This element tells a search engine information about your website. Things like wheter or not your page is time sensitive or will expire/time out, about your page, and who created it. **No closing tag for this element.** This uses a number of att. to hold info. Most likely you will use name and content atts. So:

            <meta name="value">
            <meta content="value">
            <meta http-equiv="value">

Values include
    - Description - helps search engines know what your page is about
    - keywords - common words a user might use to find your website
    - robots - determines wheter or not a search engine will include your page to it's results
    - author - who wrote the page
    - pragma - this prevents the browser from caching or storing this page locally (to your computer) to save time downloading it on future visits.
    - expires - Since browsers often cache content of the page, the expires value can be applied to indicate when a page should expire and no longer be cached.

- Escape Characters - 


## Here are a few basic tags
    <h1><h2> - main heading
    <title> - use for the title of the page in the tab
    <html> - open and close your document with this 
    <head> - is a container placed between html tags
    <body> - defines the body of the document
    <header> -  define the header of a section
    <nav> - navigation, intended for major block of links
    <img> - image <img src="url here">
    <p> - used for paragraphs, text
    <link> - connect an external link

These are just a few tips on how to get started with HTML

[Back to Homepage](README.md)