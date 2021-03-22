# Chapter 16

            display: block

    Above will turn an image into a block level element.

    For a background image:

            body {
                background-image: url("enter url here");
            }

### The background-repeat allows you to have four values:

repeat - exactly what it does, repeats horizontally and vertically.

repeat-x - horizontal only

repeat-y - vertical only

no-repeat

fixed - a fixed position on page

scroll - the image scrolls

Use the background-position and add value of left top, left center, left bottom, center top, center center, center bottom, right top, right center, and right bottom. Use % to adjust as well.

**Shorthand background**

        main {
            background: blue url("enter here") no-repeat top left;
        }
        
Specify properties in order below:
background-color
background-image
background-repeat
background-attachment
background-position

Rollover - Three different changes to image, standard, when the user hovers over it, and when the user clicks. 

Sprite -  image used for multiple parts of interface. 

CSS3 gradients - for a gradient, you have to specify the two colors that the gradient should set between. you need to use the background-image property and use your -webkit and -moz. See code example on **page 419**.

Contrast background images - If you want your text to appear over an image, generally you will want low contrast applied to your image.

Use a large element (html, body) to apply general properties and give is an id or class of **wrapper**. 

# Chapter 19 Practical Information

Search Engine Optimization (SEO) - The ability to be seen better on a search engine.

Keywords are huge for this.

Having links to and from other sites also improves visibility. 

Seven places where keyeword are located on the page to help users find you.

1. Page Title
2. URL
3. Heading
4. Text
5. Link Text
6. Image alt Text
7. Page description

Make sure your keywords appear in these places, but don't over use the words. The **meta** tag is where you can place information about your page, including keywords. 

Identifying keywords and phrases

1. Brainstorm - come up with a list
2. Organize - categorize them
3. Research - use tools to get suggestions
4. Compare - look at other sites and how they land in a search
5. Refine - choose certain keywords that might work best. If there is one that is very relevant to your page but many others are using, still use it.
6. Map - Choose 3-5 words for each page of your site.

Use analytics to understand how users found you. This can show you things like how many visitors, how they found you, how long they stayed, how many pages they visited, etc. Bounce rate shows you people that left the same page they enetered. This may suggest they were not interested.

File Transfer Protocol (FTP) - transferring your code and images to a hosting company from your computer. 


# Video and Audio APIs (Application Programming Interface)

Follow along with the code examples at: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs

Use the audio and video html elements to set up audio and video in your site.

            <video controls>
                <source src="video1.mp4" type="video/mp4">
                <source src="video2.webm" type="video/webm">
                <p>Browser does not support HTML5 video. Here is a link: <p>
                </video>

Use the _controls_ att. This will set the default video play controls. These controls are different with every browser. Also, broswers tend to not be very keyboard accessible when it comes to play controls, so it might be good to set these in your html, css, and js.

Wrap your entire video player into a div tag as a wrapper.Have multiple versions of the same video so that different browsers will be able to load the video.

_aria-label_ att. provides description of each button

Using CSS - site examples on website. You set stylings for the video player, buttons, fonts, and timer. 

Using JS, you will need to create constants representing all of these items. media, controls, play, stop, rwd, fwd, timerWrapper, timer, and timeBar.

        const play = document.queryselector('.play');

Then use the code below to remove default controls:

        media.removeAttribute('controls');
        controls.style.visibility = 'visible';

Add an event listener for the play/pause button.

        play.addEventListener('click', playPauseVideo);

Then, setup your function: view example on site.

        function playPauseVideo() {
            if(video.paused) {
                play.setAttribute('data-icon', .........
            } else {
                play.setAttribute.......
            }
        }

Note: There is no stop() method. This can be done using pause() and set the currentTime property to 0. 

The play controls in a function need to be set up to where an action needs to be canceled before another activates otherwise our code will break. Example, you have to set up a control to where the play function gets canceled so pause can be activated.

For the timer, you need to create an event listener to update the timer on the video. Again, see example near the end of the web article. 

[code201Table](201/code201Table.md)

[Back to Homepage](README.md)