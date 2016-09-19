---
layout: post
title: John R. Sawvel
subtitle: Fan of the open web
---



<div style="text-align:center;" class="largescreens greylinks" markdown="1">
[Projects](/me2.html#projects) - [Experience](/me2.html#experience) - [Making](/me2.html#making) - [Other](/me2.html#other-interests) - [Manifesto](/me2.html#manifesto)
</div>


I enjoy making things, such as web apps, food, art, crafts, and essays.

I like to use computer programming languages, combined with other technologies to build tools. My projects require knowledge across the full stack. I strive to keep my apps simple and useful.

My favorite web programs to build and use include:

* [message boards](http://toledotalk.com)
* [wikis](http://jothut.com/cgi-bin/junco.pl/blogpost/36298/19May2014/Junco-Readmemd) - [also at TT](http://toledotalk.com/cgi-bin/tt.pl/article/16/Lewiki_Home)
* [blogs](http://maketoledo.com)
* [image uploaders](http://waxwing.soupmode.com)
* [a private, web-based messaging app](https://soupmode.com) 

My goal is to make it easy to publish content to the web. 


### Projects

Information can also be found at these pages:

* [Project descriptions](https://github.com/jrsawvel/Code-Description)
* [Screenshots](https://github.com/jrsawvel/Code-Description/tree/master/screenshots)

ToledoTalk.com and JotHut.com are hosted at HE.net on shared servers where each server hosts dozens of websites, owned by others. The sites use the Apache web server. 

I'm using Amazon Web Services to manage BogHop.com. I bought the domain name through AWS, and I used Route 53 to manage DNS. For the server, I created an EC2 instance. The site uses the Nginx web server.

All of my other projects are hosted on a Digital Ocean virtual server Droplet. For these sites, I also use the Nginx web server.

I use Linux servers at all three hosting providers.



<p markdown="1" style="clear:both;padding-top:2em;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/8/7441/27652053586_1511cbbaef_q.jpg" />[Baby University](http://babyutoledo.com) is a non-profit that helps families in South Toledo prepare their children for school. I [built](https://github.com/jrsawvel/Grebe-BabyU) its website, using a customized version of my [Grebe](https://github.com/jrsawvel/Grebe) app. I also use Grebe to manage my blog sites [MakeToledo.com](http://maketoledo.com) and [ToledoWinter.com](http://toledowinter.com). Grebe uses a REST API. I created "client" versions in [Node.js](http://nodejs.soupmode.com) and [Perl](http://grebe.soupmode.com). Grebe uses MySQL, and optionally, the homepage stream of posts, and each post that was created and updated gets stored in Memcached to speed up access.</p>


<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/8/7286/27651709046_962c32f5df_m.jpg" />[ToledoWeather.info](http://toledoweather.info) reads XMl, JSON, and HTML files from the National Weather Service. [The program](https://github.com/jrsawvel/ToledoWX) also access JSON data from [Forecast.io](http://forecast.io), using [their simple API](https://developer.forecast.io/). My phone contains the [Yo](https://www.justyo.co/) app. I receive notifications on my phone, regarding heavy precipitation, by [combining](https://github.com/jrsawvel/ForecastIO-Plus-Yo/blob/master/forecastio-plus-yo.pl) Forecast.io data with the [Yo API](http://docs.justyo.co/). My [ForecastIO](https://github.com/jrsawvel/Perl-ForecastIO) and [Yo](https://github.com/jrsawvel/Yo-Perl) modules assist. [jQuery mobile](https://jquerymobile.com) displays the info.</p>


<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/6/5689/22331643762_9e5fb3c18f_q.jpg" />[Soupmode.com](https://soupmode.com) is a private, web-based messaging app that I use mainly to communicate with family members. Soupmode uses SSL. Each year, I acquire a new free certificate from [StartSSL.com](https://www.startssl.com). Soupmode was built with my [Kinglet](https://github.com/jrsawvel/Kinglet) code, which uses a REST API. The app is part microblog, part e-mail, and part message board. Messages can be sent and received to users who have agreed to be on each others' approved list. A user can reject another user's request to be added to the approved list. [Soupmode Help page](https://soupmode.com/article/help).</p>


<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/6/5829/22157056568_29459619bc_q.jpg" />[Waxwing](https://github.com/jrsawvel/Waxwing) is an image uploadin  website that offers a stream view of posts with tagging and searching. I wanted a simple way to upload photos from phone and desktop/laptop where I can then embed the photos within a blog post. Client-side JavaScript reduces the image size to a max of 640 pixels on either the width and/or the length, depending upon which one is the longest. The resolution is reduced some. The images are stored on the server's file system. Other info related to the image post is stored in CouchDB. Hashtag search exists, using a view that's added to CouchDB. Elasticsearch provides the string searching. I use Waxwing at <http://waxwing.soupmode.com>. Another Waxwing install is attached to Soupmode for private usage.</p>


<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/8/7435/28059292941_7ce24e75ff_q.jpg" />[Scaup](https://github.com/jrsawvel/Scaup) is a small, single-user web publishing app. Posts are displayed in a stream views by updated date. Long posts are automatically truncated for the stream views. When logged-in, a small text area box exists at the top of the site to allow fast posting of articles, notes, and links. This was my first attempt at using a NoSQL database. Scaup uses CouchDB. For string searches, it uses Elasticsearch. Post pages and the homepage are cached with Memcached. A test site exists at <http://scaup.soupmode.com>. I use Scaup to store my crochet notes at <http://crochet.soupmode.com>.</p>



<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/6/5773/22345023035_12ffe69937_q.jpg" /> **Veery** is similar to Scaup. It's a single-user web publishing app where the home page is a stream view of articles and notes, sorted by updated date. It also uses Memcached. Like some of my other projects, Veery uses a no-password login mechanism. Only an email address is submitted, and if it matches the author's info stored on the server, then a login link is emailed. The author only needs to click the link to activate a login session. Instead of remembering yet another password, the author can focus on securing the email account. Veery also relies on CouchDB and Elasticsearch. But Veery differs from Scaup by containing an [API](https://github.com/jrsawvel/Veery-API-Perl). Veery client versions exist in [Perl](https://github.com/jrsawvel/Veery-Client-Perl) and [NodeJS](https://github.com/jrsawvel/Veery-Client-NodeJS). Test sites: [Perl client](http://veeryclientperl.soupmode.com), [Node.js client](http://veeryclientnodejs.soupmode.com), and [API endpoint](http://veeryapiperl.soupmode.com/api/v1).




<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/8/7397/27612350631_a79de945a5_q.jpg" /> [Wren](https://github.com/jrsawvel/Wren) is a lightweight, web publishing app that does not use a database. It stores markup in plain text files, and it creates static HTML pages. At the moment, it's a single-user tool. Wren is [API-based](https://github.com/jrsawvel/Wren/blob/master/docs/wren-api.md), using REST and JSON. Most of my web publishing apps support Textile and Markdown/MultiMarkdown, but Wren only supports Markdown. From the summer of 2014 to May 2016, [birdbrainsbrewing.com](http://birdbrainsbrewing.com) was powered by my Grebe code, but in May 2016, I converted the site to use Wren. I also use Wren at [wren.soupmode.com](http://wren.soupmode.com), [boghop.com](http://boghop.com), <a href="gopher://boghop.com">gopher://boghop.com</a>, and [zwdqwr2p2xwkpbyv.onion](http://zwdqwr2p2xwkpbyv.onion). The .onion site runs on my home Linux computer, and I'm using it to test Tor. I created the gopher site to test the gopher protocol. To view the onion and gopher sites, special browser clients are required.



<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/8/7661/27076320183_a81166eab9_q.jpg" /> [Article Preview](https://github.com/jrsawvel/Article-Preview) is a quick way to test the format of single web pages. The test site exists [article.soupmode.com](http://article.soupmode.com), and [here's sample markup](https://github.com/jrsawvel/Article-Preview#sample-markup) to try. Using a browser, markup is submitted and formatted html is returned. It supports Markdown, MultiMarkdown, Textile, and HTML. Numerous custom formatting commands exist too. It also contains a [one-command API](https://github.com/jrsawvel/Article-Preview#api-and-json) where JSON is submitted that contains the markup, and then JSON is returned, which contains the formatted post, along with other information, such as word count, reading time, etc. I created this simple tool to test my [ramblings about article page design.](https://github.com/jrsawvel/Article-Designs)




<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/6/5789/22331644482_b3e0b1e89e_q.jpg" /> **Parula** is the name of the code that powers my small, local message board [ToledoTalk.com](http://toledotalk.com), but I do not have the code committed to GitHub. I bought the domain name in September 2001. In the fall of 2002, I started building [the first version of TT](http://www.toledotalk.com/cgi-bin/topics.pl), which was patterned after MetaFilter.com in look and functionality. TT launched in January 2003. In 2005, I created the Parula code, which was/is wiki-based. I wanted a wiki to run alongside the message board. Parula supports Textile. (I've been writing in Textile since 2005, but I also like Markdown.) I liked the Parula code better than the original TT code, and in August 2007, I switched the main site to be powered by Parula.  Over the years since, I have continued to make small changes, but TT is still powered by the Parula code from 2005. 



<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/8/7475/28405781546_d97c6dcdfb_q.jpg" /> Last decade on the ToledoTalk.com server, I created a few [map mashups](http://toledotalk.com/cgi-bin/tt.pl/article/2114/Lewiki_Mashups) that combined data with Google maps. I built [my first map mashup](http://www.toledotalk.com/cgi-bin/comments.pl/21/1376) in 2005 that mapped Lucas County registered sex offenders, using data from the sheriff's department. I maintained this mapping project for a few years, but it became too much of a legal hassle, even though I didn't do anything wrong. I've disabled viewing of that map app. The others don't display content anymore because of tech changes by Google.




<p markdown="1" style="clear:both;padding-bottom:2em;"><img class="largescreens" style="float:left;padding-right:20px;width:100px;height:100px"  src="https://c2.staticflickr.com/6/5740/22319004206_d8d5623a12_q.jpg" /> [JavaScript Editor](https://github.com/jrsawvel/Code-Description/tree/master/screenshots#javascript-editor) -  My Junco, Grebe, Scaup, Veery, and Wren web publishing apps have the option to use a simple, JavaScript-based "editor" for creating and updating posts. In 2013, I started with this person's code [borgar.github.io/textile-js](http://borgar.github.io/textile-js). It's a live-preview editor that supports Textile, but didn't like the flashing of the formatted text in the right window pane. I modified the original code a lot to support my needs. I removed the live-preview, since my web apps also support Markdown and my own custom commands. I prefer to let the server code do all of the formatting. My version  accesses the API code in my apps. Using REST and JSON, the editor sends markup to the server, and it receives HTML. Other functions that I added include a single-screen view to create a larger writing area, keyboard shortcuts, and auto-save. 

--(My preferred writing environment is to use Textile or Markdown with my version of this JavaScript editor, along with one of my web publishing apps. For example, I created this page using Wren, Markdown, and the modified JavaScript editor.)--



### Experience

#### Recent

* Linux
* Nginx
* MySQL
* CouchDB
* Eleasticsearch
* Memcached
* Redis
* Perl
* HTML::Template
* NodeJS
* Express
* Handlebars
* JavaScript
* jQuery
* minified.js
* CSS
* HTML
* MailGun
* APIs
* JSON
* REST
* Textile
* Markdown/MultiMarkdown
* Responsive Web Design
* Progressive Enhancement
* Droplet hosting at Digital Ocean
* using SSL for one site



#### Past

In the past, I worked as a computer systems administer and programmer at a market research company where I managed Unix and Vax/VMS systems, and I created utilities and web apps. I have older experience with programming languages, such as C, Java, TCL, shell, and DCL. My web projects used Microsoft and Oracle databases.

From late-May 2008 to mid-November 2012, I worked in the education area at the Black Swamp Bird Observatory, which is a tiny non-profit, located along Lake Erie about 30 minutes east of Toledo. I created and maintained the website for the Ohio Young Birders Club. I wrote content, and I edited content, created by students and adults. The site that I created has been replaced, and unfortunately, the content is gone too. [Sample page from Archive.org - Feb 2012](http://web.archive.org/web/20120224135234/http://www.ohioyoungbirders.org/) --(not mobile-friendly)--




### Making

I believe that each person should have at least one hobby that involves building or making something.

* [My crochet notes](http://crochet.soupmode.com) - Crocheting has become one of my favorite activities. It's easy, tactile, relaxing, and portable. I can make useful items, such as [hats](http://crochet.soupmode.com/tag/beanie) and [scarves](http://crochet.soupmode.com/scarves-that-i-crocheted-in-20142015), or I can make silly things, such as [snowflakes](http://crochet.soupmode.com/my-first-snowflake) and hyperbolic geometry-related [structures](http://crochet.soupmode.com/crochet-and-hyperbolic-geometry).

* [Making naturally-leavened sourdough bread](http://boghop.com/baking-naturallyleavened-sourdough-bread.html) - This might be my favorite food because of its taste, versatility, and simplicity. I "hatched" my starter in January 2010 at a Zingerman's bread baking class in Ann Arbor. [#bread links and notes](http://jothut.com/cgi-bin/junco.pl/tag/bread)

* [Brewing beer](http://birdbrainsbrewing.com/) - This is a shared hobby with my wife that has taken a hit due to time constraints. Hopefully, we return to this tasty activity soon.

* [Maintaining a backyard garden](http://jothut.com/cgi-bin/junco.pl/tag/garden)

* [Roasting coffee beans](http://boghop.com/roasting-coffee-beans-at-home.html) - I even roasted decaffeinated coffee beans, which turned out shockingly well. This was the first time that I have enjoyed decaf coffee.

* [Making pizza](http://boghop.com/making-pizza.html) - My favorite pizzas remain the ones that I make at home, especially when I use toppings that were made by my wife.

* [#watercolor links and notes](http://jothut.com/cgi-bin/junco.pl/tag/watercolor) - My sketches are weak, therefore they remain private. But it's fun. I like to slow down and observe. For portability, I use a very small watercolor set with a few paints and a waterbrush.



### Other interests

My other interests include [weather](http://toledoweather.info), especially [winter weather](http://toledowinter.com), fishing, and [birdwatching](http://jothut.com/cgi-bin/junco.pl/tag/bird) or [observing nature](http://jothut.com/cgi-bin/junco.pl/tag/nature).

I monitor changes in [media](http://jothut.com/cgi-bin/junco.pl/tag/media) and [digital design](http://jothut.com/cgi-bin/junco.pl/tag/design). I'm interested in how information is created, consumed, and shared.


### Manifesto

Since at least the beginning of 2014, I've become somewhat obsessed with simplifying the design for the single web page article, to make it load faster and to make it easier to read, especially on phones. Web page bloat has become a major irritant, in my opinion.

Here's my manifesto for lightweight web pages. If this doesn't qualify as a manifesto, then it's a screed. It's definitely a frustration for the way that some publishers treat the web.


* [Intro](http://boghop.com/manifesto-for-lightweight-web-pages.html)
* [Design By Writing](http://boghop.com/design-by-writing.html)
* [Create a Comfortable Reading Experience](http://boghop.com/create-a-comfortable-reading-experience.html)
* [Battle Page Bloat](http://boghop.com/battle-web-page-bloat.html)

