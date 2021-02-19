# CH16: Controllig Img size 
* You can specify the dimensions of images using CSS. This is very helpful when you use the same sized images on several pages of your site.
* You can control the size of an image using the width and height properties in CSS, just like you can for any other box.
* First you need to determine the sizes of images that will be used commonly throughout the site, then give each size a name
* Where the``` <img>``` elements appear in the HTML, rather than using width and height attributes you can use these names as values for the class attribute.

**HTML** ``<img src="images/magnolia-small.jpg"class="small" alt="Magnolia" />``

* In the CSS, you add selectors for each of the class names, then use the CSS width and height properties to control the image dimensions.
**CSS** ``img.small {``

``width: 100px;``

``height: 100px;}``

## Aligning images using css 

* Images can be aligned both horizontally and vertically using CSS.

* you can use the class names are used in addition to classes that indicate the size of the image like 
**HTML** ``p><img src="images/magnolia-medium.jpg" alt="Magnolia" class="align-right medium" />``

**CSS**
``img.align-left {``

``float: left;}``

## Centering images using css 

* By default, images are inline elements (flow within the surrounding text)
* to center an image turned into a blocklevel element ``{disply:block}``
* On the **containing element**, you can use the **text-align** property with a value of center.
* On the **image** itself, you can use the use the margin property and set the values of the left and right margins to auto

``img.align-center {``

``display: block;``

``margin: 0px auto;}``


## Background Images

* You can use a background image behind the box created by any element on a page, The background-image property allows you to place an image behind any HTML element, you sellect it

``body {``

``background-image: url("images/pattern.gif");}``

## Repeating Images

* Background images can appear just once or be repeated across the background of the box.

``body {``

``background-image: url("images/header.gif");``

``background-repeat: value;}``

**Value become as**

1. repeat :The background image is repeated both horizontally and vertically
2. repeat-x :The image is repeated horizontally only (as shown in the first example on the left).
3. repeat-y :The image is repeated vertically only.
4. no-repeat :The image is only shown once.
5. fixed :The background image stays in the same position on the page.
6. scroll : The background image moves up and down as the user scrolls up and down the page.

## Background Position

value:(left top ,left center ,left bottom ,center top ,center center ,center bottom ,right top ,right center ,right bottom)

``{background-position: 50% 50%;}``




**You can create image rollover effects by moving the background position of an image.**

**To reduce the number of images your browser has to load, you can create image sprites.**


# CH19: Practical Information

* Search engine optimization (SEO) helps visitors find your sites when using search engines.

* In every page of your website there are seven key places where keywords (the words people might search on to find your site) can appear in order to improve its findability.
1. Page Title
2. URL / Web Address
3. Headings
4. Text
5. Link Text
6. Image Alt Text
7. Page Descriptions

* **six steps** that will help you identify the right keywords and phrases for your site:
1. **Brainstorm** : List down the words that someone might type into Google to find your site. Be sure to include the various topics, products or services your site is about.
2. **Organize** Group the keywords into separate lists for the different sections or categories of your website.
3. **Research** There are several tools that let you enter your keywords and then they will suggest additional keywords you might like to consider, such as:`` adwords.google.co.uk/ select/KeywordToolExternal`` ``www.wordtracker.com`` ``www.keyworddiscovery.com``
4. **Compare** 
5. **Refine**
6. **Map**

* Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.
* To put your site on the web, you will need to obtain a domain name and web hosting.
**DOMAIN NAMES** Your domain name is your web address (e.g. google.com or bbc.co.uk). There are many websites that allow you to register domain names. Usually you will have to pay an annual fee to keep that domain name

* So that other people can see your site, you will need to upload it to a web server. Web servers are special computers that are constantly connected to the Internet. They are specially set up to serve web pages when they are requested

**WEB HOSTING** There are lots of different types of hosting like (Disk space/ Bandwidth/ Backups)



* FTP programs allow you to transfer files from your local computer to your web server.
* Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).


# CH9: Flash, video and audio

**Flash** has been a very popular tool for creating animations, and later for playing audio and video in websites

* Whether you are creating an animation or a media player in Flash, the files you put on your website are referred to as Flash movie
* When you create a Flash file in the Flash authoring environment, it is saved with the .fla file extension. In order to use this file on a web page it has to be saved in a different format known as SWF. (It has the .swf file extension.)


# HTML5 video and audio
The ``<video>`` and ``<audio``> elements allow us to embed video and audio into web pages

``<video controls>``

  ``<source src="rabbit320.mp4" type="video/mp4">``

  ``<source src="rabbit320.webm" type="video/webm">``

``</video>``

## The HTMLMediaElement API
Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example ``HTMLMediaElement.play()``, ``HTMLMediaElement.pause()`` etc.

