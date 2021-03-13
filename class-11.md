# IMAGES

Controlling the size and alignment of
our images using CSS keeps rules that
affect the presentation of our page in
the CSS and out of the HTML markup.

We can control the size of an
image using the width and
height properties in CSS.

Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
code will often load before the
images, and telling the browser
how much space to leave for an
image allows it to render the rest
of the page without waiting for
the image to download.

![back](data:image/png;base64,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)

Where the <*img>* elements
appear in the HTML, rather
than using width and height
attributes we can use these
names as values for the class
attribute.
In the CSS, we add selectors for
each of the class names, then
use the CSS width and height
properties to control the image
dimensions.


**Background-image**

The background-image
property allows us to place
an image behind any HTML
element.

 **Background-repeat** property can have four values:
 * repeat
 * repeat-x : The image is repeated
horizontally only (as shown in
the first example on the left).
* repeat-y: The image is repeated vertically
only.
* no-repeat: The image is only shown once.
* fixed: The background image stays in
the same position on the page.
* scroll: The background image moves
up and down as the user scrolls
up and down the page.

**Background position**

* left top
* left center
* left bottom
* center top
* center center
* center bottom
* right top
* right center
* right bottom


The properties must be specified
in the following order, but we
can miss any value if we do not
want to specify it :

1: background-color

2: background-image

3: background-repeat

4: background-attachment

5: background-position

CSS3 is going to introduce the
ability to specify a gradient for
the background of a box.

**Contrast of background images**

If we want to overlay text on a background image, the image must be low
contrast in order for the text to be legible.

![image](https://miro.medium.com/max/1808/1*QTWGR0eSThjeeJLuTWVgKA.jpeg)

We can use a background image behind the box
created by any element on a page.

To reduce the number of images our browser has to
load, we can create image sprites.

# Practical Information

Search Engine Optimization (SEO)
SEO is a huge topic and several books have been written on the subject.

**The Basics**

Search engine optimization (or
SEO) is the practice of trying
to help our site appear nearer
the top of search engine results
when people look for the topics
that our website covers.

![on](https://wordstream-files-prod.s3.amazonaws.com/s3fs-public/styles/simple_image/public/images/media/images/on-page-seo-versus-off-page-seo-visual.jpg?N0F5SfUyTfk0gH6KFLhTwBsVFYgN0kmP&itok=gI_4ZOUn)

**On-Page Techniques**

On-page techniques are the
methods we can use on our
web pages to improve their
rating in search engines.

**Off-Page Techniques**

Getting other sites to link to us
is just as important as on-page
techniques. Search engines help
determine how to rank our
site by looking at the number of
other sites that link to ours.

In every page of our website there are seven key places where keywords
(the words people might search on to find our site) can appear in order
to improve its findability.


![seo](https://theweeklytrends.com/wp-content/uploads/2019/10/zz1-14.jpg)

**How to Identify Keywords and Phrases**

1: Brainstorm

2: Organize

3: Research

4: Compare

5: Refine

6: Map

**Google Analytics**

**Signing Up**

The Google Analytics service
relies on us signing up for an
account at:
www.google.com/analytics
The site will give us a piece of
tracking code which we need to
put on every page of our site.


**How it Works**

Every time someone loads a
page of our site, the tracking
code sends data to the Google
servers where it is stored.
Google then provides a webbased
interface that allows us
to see how visitors use our site.

**The Tracking Code**

A tracking code is provided
by Google Analytics for each
website we are tracking. It
should appear just before the
closing <*/head>* tag. The code
does not alter the appearance of
our web pages.


### How Many People Are Coming to Our Site?

**Visits**

This is the number of times
people have come to our site.

**Unique Visits**

This is the total number of
people who have visited our site
over the specified period.


**Page Views**

The total number of pages all
visitors have viewed on our site

**Pages per Visit**

The average number of pages
each visitor has looked at on
our site per visit.


**Average Time on Site**

The average amount of time
each user has spent on the site
per visit.

**Date Selector**

Using the date selector in the top
right hand corner of the site, we
can change the period of time
the reports display.

**Export**

The export link just above the
title that says "visitors overview"
allows us to export the
statistics on this page for other
applications such as Excel.

The content link on the left-hand side allows
us to learn more about what the visitors are
looking at when they come to our site.

![page](https://leadfront.io/wp-content/uploads/2017/12/web-analytics.png)


### Domain Names & Hosting

These sites usually have a form
that allows us to check whether
our preferred domain name is
available, and because millions
of domain names have already
been registered, it might take
us a while to find the one that is
right for our site.

**Disk space**

This refers to the total size of all
of the files that make up our site
(all of the HTML and CSS files,
images and scripts).


**Bandwidth**

This is the amount of data the
hosting company will send to
our site's visitors.

**Backups**

Check whether the hosting
company performs backups on
our site (and how often).

### FTP & Third Party Tools 

To transfer our code and images from our
computer to our hosting company, we use
something known as File Transfer Protocol.

![ftp](https://cdn.educba.com/academy/wp-content/uploads/2019/10/FTP-vs-SFTP.png)

Here is a list of some popular FTP applications:

* FileZilla
* filezilla-project.org
*Windows, Mac, Linux
* FireFTP
* fireftp.mozdev.org
 Windows, Mac, Linux
* CuteFTP
* cuteftp.com
 Windows, Mac
* SmartFTP
* smartftp.com
* WIndows
* Transmit
* panic.com/transmit
* Mac


Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save we writing them from scratch).


### Video and Audio APIs

HTML5 comes with elements for embedding rich media in documents — <*video>* and <*audio>* — which in turn come with their own APIs for controlling playback, seeking, etc.

![video](https://static.freemake.com/blog/wp-content/uploads/2015/06/HTML5-video-tag-sample-code.png)


if we load the HTML you should see a perfectly normal HTML5 video player, with the native controls rendered.

The <*video>* element contains two <*source>* elements so that different formats can be loaded depending on the browser viewing the site.

The controls HTML is probably the most interesting:
We have four <*button>* s — play/pause, stop, rewind, and fast forward.

Each <*button>* has a class name, a data-icon attribute for defining what icon should be shown on each button (we'll show how this works in the below section), and an aria-label attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags. The contents of aria-label attributes are read out by screenreaders when their users focus on the elements that contain them.


We use the ::before selector to display the content before each <*button>* element.
We use the content property to set the content to be displayed in each case to be equal to the contents of the data-icon attribute. In the case of our play button, data-icon contains a capital "P".
We apply the custom web font to our buttons using font-family. In this font, "P" is actually a "play" icon, so therefore the play button has a "play" icon displayed on it.

### How Flash Works

Whether we are creating an
animation or a media player in
Flash, the files we put on our
website are referred to as Flash
movies.

If we want to create our
own Flash movie, we need to
purchase the Flash authoring
environment from Adobe.

![video](https://aleen42.gitbooks.io/wiki/content/Programming/HTML/flash_video_audio/timeline.png)


The most popular way of
adding Flash into a web page
is using JavaScript. There are
several scripts that allow you
to do this without an in-depth
understanding of the JavaScript
language.

The type attribute is used on the
<*script>* element to indicate
that the script inside is written
in JavaScript. The *src* attribute
tells the browser where to find
the script.


