---
layout: post
title: Convert point shapefile to GPX waypoints for use in Garmin GPS
---

The easiest way or one way to this is with [QGIS] (http://www.qgis.org/)

1) Open QGIS

2) Edit the table so that it have the three columns name, cmt, and desc. The name column will be the waypoint id, the two other columns are comments (cmt) and description desc). I have to check which one that is most important.

You can create a string description of multiple columns like this:


![_config.yml]({{ site.baseurl }}/images/2014-08-20/image002.png "Step2")

Thus the table with the three default columns:


![_config.yml]({{ site.baseurl }}/images/2014-08-20/image004.png)

4) The export to GPX using the Layer menu and Save as. Remember to set the coordinate system of the GPS (Check if important, maybe a geograpichal system is needed??). In the Save vector layer as dialog box set CRS=Selected CRS og Browse to the correct system (eg. WGS84 -  ESPG:4326).


![_config.yml]({{ site.baseurl }}/images/2014-08-20/image006.png)

The GPX file should den look like this if opened in a text editor:

![_config.yml]({{ site.baseurl }}/images/2014-08-20/image008.png)

This is a demo of all styled elements in Jekyll Now. 

[View the markdown used to create this post](https://raw.githubusercontent.com/barryclark/www.jekyllnow.com/gh-pages/_posts/2014-6-19-Markdown-Style-Guide.md).

This is a paragraph, it's surrounded by whitespace. Next up are some headers, they're heavily influenced by GitHub's markdown style.

## Header 2 (H1 is reserved for post titles)##

### Header 3

#### Header 4
 
A link to [Jekyll Now](http://github.com/barryclark/jekyll-now/). A big ass literal link <http://github.com/barryclark/jekyll-now/>
  
An image, located within /images

![an image alt text]({{ site.baseurl }}/images/jekyll-logo.png "an image title")

* A bulletted list
- alternative syntax 1
+ alternative syntax 2
  - an indented list item

1. An
2. ordered
3. list

Inline markup styles: 

- _italics_
- **bold**
- `code()` 
 
> Blockquote
>> Nested Blockquote 
 
Syntax highlighting can be used by wrapping your code in a liquid tag like so:

{{ "{% highlight javascript " }}%}  
/* Some pointless Javascript */
var rawr = ["r", "a", "w", "r"];
{{ "{% endhighlight " }}%}  

creates...

{% highlight javascript %}
/* Some pointless Javascript */
var rawr = ["r", "a", "w", "r"];
{% endhighlight %}
 
Use two trailing spaces  
on the right  
to create linebreak tags  
 
Finally, horizontal lines
 
----
****