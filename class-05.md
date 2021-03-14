# Read 05 Images, Color, and Text.

# Chapter 5 Duckett Images

- Adding images:

        <img src="url or file name" alt="A description of the image that is seen by users if they cannot see the image." title="A descripton of the image that will be seen by the user in the browser when they hover over the image."/>

- Height and Width can be added into the html code.

        <img src="url or file name" alt="A description of the image." wigth="400" height="200"/>

- Be mindful of where you place images in your html code in relation to other elements. Inside an element will include the image in text or heading amongst the text in the same box.

- align - This attribute is mainly used in older code. This is not used in HTML5 where you align images in CSS. This is if you want your image to appear on the left or the right of your text. Also use top, middle, or bottom to align images vertically. 

        <img src="url or file name" alt="A description of the image." align="left" or "right"/>

### Three Rules:

1. Make sure you pick the correct format: jpeg, gif, or png.

2. Make sure you set the height and width on your website to the same height and width as the file otherwise it can distort or stretch. 

3. Use px when setting the measurements on your images. 

- jpeg - Make sure to use this format when using images that contain a lot of color. This is the best format for photos of outdoor scenery.

- gif or png - Use this format when using images that have few colors or images with a large area of one color. 

- **Reducing image size** - this is good if you need an image that is 400 pixels by 200 pixels. You can reduce it 50% to 200 by 100. 

- **Increasing image sixe** - you cannot increase of your photo too much otherwise this will hinder the quality greatly. You may only want to use this for small adjustments. 

- **Changing Shape** - You can also crop an image without losing quality but you will lose part of the image. 

- **Measuring and Resolution** - Make sure to save images at 300 DPI (dots per inch) to make sure the images are sharp. 

- **Vector Images** - These images are not dependent on resolution. Examples are logos, graphs, diagrams, etc. These are created with a grid and placing points on that grid and connecting between points, kind of like connect the dots. Once you close an area, you can fill in this area with color. These images are great due to the fact that you can increase and decrease the size without impacting the quality. 

- **Animated Gifs** - We all know what these are, but a few points to consider. These are used for simple illustrations, not for showing sharp images. These combine several images together to show animation. The more images included in the file, the bigger it becomes, icreasing the time for downloading. Make sure these are simple. 

- **Transperency** - Adding a quality to be able to see through the image. Tranperency works for gifs if the edge of the image are straight. PNGs allow for more options like diagonal, rounded, semi-opaque, and a drop- shadow. 

- **The figure element** can be used to contain images with a caption. The figcaption element is used to add the caption.

        <figure>
            <img src="url of file name" alt="" title="" width="" etc./>
            <br />
            <figcation>Put your caption about the image within this element.</figcaption>
        </figure>


# Chapter 11 Color  

- You can use the RGB rules using hex codes #ee3e80, rgb(100,100,90), color names
- There are 147 named predetermined colors
- You can adjust colors by changing the hue, saturation (the amount of gray), and brightness (how much black).
- You can use the value to indicate color, background color, and more.
- Contrast - you can use contrast to ensure that your text over the color is readable. The colors can't be so similar that you cannot read the text.
- Opacity refers to the ability to see through a feature on your page and see another feature behind, so the overlap is visible. You use the rgba format, so four numbers. This is expressed from a 0.0 to 1.0 scale. 0.0 being 0%, 1.0 being 100%.

### hsl, hsla

- h - Hue is expressed as an angle, 0 to 360 degrees, appears as a wheel. This can help you see more choices.
- s - Saturation is expressed as a percentage 0%-100% and refers to the amount of gray in a color.
- l - Lightness - is the amount of white (lightness) or black (darkness) in a color. Lightness is expressed with a percentage of 0 being white, 50% being normal, and 100% being black.
- a - Alpha is expressed in 0.0 - 1.0 scale and refer to transperency. 

# Chapter 12 Text Duckett



[code201Table](code201Table.md)

[Back to Homepage](README.md)