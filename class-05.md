# Images in Html

There are many reasons why we might
want to add an image to a web page: we
might want to include a logo, photograph,
illustration, diagram, or chart.

A picture can say a thousand words.

Images should:
* Be relevant
* Convey information
* Convey the right mood
* Be instantly recognisable
* Fit the color palette

If we are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.

To add an image into the page
we need to use an <*img>*
element.

<*img src="url of image" alt="description of image" title="title
attribute" />*

*src*
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on our
own site.

*height*
This specifies the height of the
image in pixels.

*width*
This specifies the width of the
image in pixels.

**Where an image is placed ?**
* before a paragraph
* inside the start of a
paragraph
* in the middle of a
paragraph

There are three rules to remember when we
are creating images:

* Save images in
the right format
* Save images at
the right size
* Use the correct
resolution


**Image Formats**
* JPEG
* GIF

Tools to Edit
& Save Images ,
We can change many thing on image:

* Image Dimensions
* Cropping Images
* Image Resolution

Images often come with
captions. HTML5 has introduced
a new <*figure>* element to
contain images and their caption
so that the two are associated.

The <*figcaption>* element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.

![image](https://www.naukrinama.com/stressbuster/wp-content/uploads/2019/04/4-2.png)

TL;DR
Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

Almost all forms of data that we see on the internet — text, image, video etc, are compressed to reduce the size of data and ensure faster transmission.

Compression can be of two types :
* lossless 
* lossy. 

In lossless compression, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression.

Lossy compression algorithms always have a superior compression ratio (the ratio of size of compressed image to original image)

* JPEG is a lossy compression
* PNG is a lossless compression
* GIF is a lossless

![lossy](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/f3d84205-58e9-4190-9268-b57b8a89be02/image2-speed-up-your-website-webp.png)

**Transparency**

* JPEG images don’t support transparency
* PNG images support transparency
* GIF images support transparency by declaring a single colour in the colour palette as transparent


Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. 

Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. 

Use GIF format for images that contain animations.

## Color

The color property allows we
to specify the color of text inside
an element. 

We can specify any
color in CSS in one of three ways:

* RGB values
* Hex codes
* Color names


JPEG images can support around 16 million colours.

PNG images mainly have two modes, PNG8 and PNG24. PNG8 can support upto 256 colours where as PNG24 can handle upto 16 million colours like a JPEG image.

GIF images are limited to 256 colours.

CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.

Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color we want, we can use a color picker.

It is important to ensure that there is enough contrastbetween any text and the background color (otherwise people will not be able to read our content).

![color](https://lh3.googleusercontent.com/proxy/QgUozxHQ5awuzCIr-7K3sIq-6xab1YQaS0PKfkp6pL8eeNa1JNnXNEF9b636uPCB47B78u69XoehrwyPQlZp73Xqs6NOLrY2lNd-iJSfHAoDkahVRq-9ZQ7E_t1VEj0G4EiPH_9KBRHfIOCDllTjTLkjzLEakXYjhHXhMmAo61Z7JdioPbv7MCRNrtCX4w)

CSS3 introduces the opacity
property which allows us to
specify the opacity of an element
and any of its child elements.

The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.

![hsl](https://cdn.educba.com/academy/wp-content/uploads/2019/11/Types-of-the-Color-Name-in-HTML.png)

### Text

The formatting of our text can have a significant effecton how readable our pages are.

![text](https://www.shillingtoneducation.com/content-blog/uploads/2019/09/Typography_Anatomy.jpg)

When we choosing
a typeface, it
is important to
understand that a
browser will usually
only display it if it's
installed on that
user's computer.

The font-family property
allows us to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.

The font-size property enables
us to specify a size for the
font. There are several ways to
specify the size of a font.

**Type Scales**
* Pixels
* Percentages
* Ems : Ems allow us to change the size
of text relative to the size of the
text in the parent element

The font-weight property
allows us to create bold text.
There are two values that this
property commonly takes:
* normal
* bold

If we want to create italic text,
we can use the font-style
property. There are three values
this property can take:
* normal
* oblique
* italic


The text-transform property
is used to change the case of
text giving it one of the following
values:
* uppercase
* lowercase
* capitalize

The text-align property allows
us to control the alignment of
text.

The text-indent property
allows us to indent the first
line of text within an element.

**:link**
This allows us to set styles
for links that have not yet been
visited.

**:visited**
This allows us to set styles for
links that have been clicked on.