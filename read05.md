# Understanding CSS

CSS applies rules to your html elements by using a selector (ex: p, h1, etc) followed by a declaration (box) using the {} brackets. Selectors indicate what element you want to stylize and the declaration is how the element should be styled. A declaration is made up of two parts, a property (color:, font-family:, etc.) and a values (color: yellow;, font-family: Arial;). You can use multiple elements in a CSS rule, so:

            h1, h2, h3 {
                font-family: Arial;
                color: yellow;}

The link element can be used in html to tell your browaser where to look for the CSS file you are using to style the page. 

        - href - specifies path to CSS file
        - type - the type od document being linked to.
        - rel - indicates the relationship between the file you are linking to and the html.

You can also include CSS styling in you HTML code by using the style element or tag. You can place CSS rules within this tag directly in your CSS code. This tag should sit inside the head tag or element. 

You can select a class in your CSS document by using the class selctor. THis is indicated by a . before the selector.
        - * is a universal selector and applies to all elements

**You can use one CSS sheet to apply to a website with multiple pages.**


## Chapter 11 Color
- You can use the RGB rules using hex codes #ee3e80, rgb(100,100,90), color names
- There are 147 named predetermined colors
- You can adjust colors by changing the hue, saturation (the amount of gray), and brightness (how much black).
- You can use the value to indicate color, background color, and more.
- Contrast - you can use contrast to ensure that your text over the color is readable. The colors can't be so similar that you cannot read the text.
- Opacity refers to the ability to see through a feature on your page and see another feature behind, so the overlap is visible. 
- Lightness - is the amount of white (lightness) or black (darkness) in a color.
- Hue is expressed as an angle, 0 to 360 degrees
- Saturation is expressed as a percentage
- Lightness is expressed with a percentage of 0 being white, 50% being normal, and 100% being black.
- Alpha - expressed between 0 and 1.0. 0.5 is 50% transperancy and 0.75 is 75% transperancy.

[Back to Homepage](README.md)