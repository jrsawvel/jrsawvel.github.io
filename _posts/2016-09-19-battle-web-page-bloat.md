---
layout: boghop
title: Battle Web Page Bloat
subtitle: "We despise having to download megabytes of crapware"
---



<div markdown="1" style="background:#CEE3F6;text-align:center;">
**This page is unfinished,
 and it's currently being edited.**
</div>


In my opinion, showing empathy for web readers means not burdening them with obese article pages that are loaded with unnecessarily huge and maybe irrelevant images, JavaScript, ads, trackers, and unknown objects. Simplifying leads to faster performance and a better reading experience. 

A single web page can be several megabytes in size once everything is downloaded to the user's device. Pounds of cruft can bog down older machines and create a clunky UI/UX.

JavaScript is not the problem. The misuse or overuse of JavaScript is the problem. 

Here are the March 7, 2016 webpagetest.org results for a [Toledo Blade op-ed](http://www.toledoblade.com/Featured-Editorial-Home/2016/03/06/Yes-on-Toledo-tax.html).

First View Fully Loaded:

* Time: 44.201s
* Request: 952
* Bytes In: 5,018 KB
* Cost: $$$$$

A single web page makes 952 requests and ends up being 5 megabytes in size. The op-ed contained a few hundred words of text with no images.

In June 2016, the Toledo Blade introduced a new version of its website, and as of late July 2016, it appears that the Blade has trimmed its pages by more than 50 percent. 

July 2016 webpagetest.org [results](http://www.webpagetest.org/result/160721_M9_1J02/) for the same March 2016 op-ed.

From: Dulles, VA - Chrome - Cable 7/21/2016, 4:50:42 PM

First View Fully Loaded:

* Time: 17.279s
* Requests: 329 
* Bytes In: 2,020 KB
* Cost: $$$$$

The page is still too large, but at least the Blade is trending in a positive direction. Just because our computers of all sizes contain more memory and faster CPUs, that doesn't mean publishers should create sprawling web pages. 

I host some of my websites at Digital Ocean, and I have total access to my own virtual server. For these sites, I use the Nginx web server. 

Here's a [simple HTML page of the same op-ed,](http://testcode.soupmode.com/yes-on-toledo-tax.html) stored on my Digital Ocean server (obvious copyright violation to make a point).

The actual file size of the HTML page is around 8 KB. Nginx compression shrinks the download size of the page to 5 KB.

webpagetest.org [results](http://www.webpagetest.org/result/160721_1C_1M50)

From: Dulles, VA - Chrome - Cable - 7/21/2016, 5:34:39 PM

First View Fully Loaded:

* Time: 0.557s
* Requests: 2
* Bytes In: 5 KB
* Cost: $

Some tests show the download time to be around 0.3 seconds. Even a heavily-trafficked, properly-configured website should be able to serve the text portions of simple, static HTML files in about a second.

Obviously, for-profit publishers want to monetize their websites, which means bombarding users with ads and trackers. It's a conundrum. How can publishers make money from their web content while providing a reader-friendly experience? 

My answer is a paywall. Restaurants and many other businesses do not give away their creations for free. At Etsy, I could pay $15 to $30 for a crocheted beanie, but the Toledo Blade gives away its craft for free.

I feel bad for the writers, editors, and everyone else at newspaper orgs. Their service is needed at the local level. But bloated web design indefensible.

I suppose that I would be the only person willing to pay a hefty annual subscription fee for content that was displayed as simply as the HTML example that I created above. Photos and illustrations are still welcomed. In fact, more images should be posted. But publishers should simplify the delivery container.

A fast, simple delivery mechanism does not improve bad writing. But good writing and important writing can be lost or ignored when the delivery mechanism is an abomination.

Even digital-only media sites that have formed in recent years and never created a print version are designing massively bloated websites.

But I see no improvements in the future by publishers, regarding their reader-hostile web designs. The only change will be that the websites will get worse.

Thanks to poorly-designed, slow websites, we will have more services like Facebook's Instant Articles and Google's Accelerated Mobile Pages because most people read on their phones.

Some day, it may be pointless for news orgs to have their own websites because they will publish their content on other platforms. It's not Facebook's fault. It's the fault of the publishers. And we can't blame the content management systems. Humans make the decisions.

Other people have plenty to say on the subject.


---


* mondaynote.com - [News Sites Are Fatter and Slower Than Ever](https://mondaynote.com/news-sites-are-fatter-and-slower-than-ever-1dc7adebfc90#.3bh7mismx)

> An analysis of download times highlights how **poorly designed news sites are.** That’s more evidence of poor implementation of ads… and a strong case for ad blockers.

> Websites designers live in a bubble, they’re increasingly disconnected from users.

> Today, a news site web page of a consists of a pile of scripts, of requests to multiple hosts in which **relevant content only makes up an insignificant proportion of the freight.**

> Consider the following observations: When I click on a New York Times article page, it takes about 4 minutes to download 2 megabytes of data through… 192 requests, some to Times’ hosts, most to a flurry of others servers hosting scores of scripts. Granted: the most useful part — 1700 words / 10,300 characters article + pictures — will load in less that five seconds.

> But when I go to Wikipedia, a 1900 words story will load in 983 milliseconds, requiring only 168 kilobytes of data through 28 requests.

Unfortunately, "only" 2 megabytes of crud and "only" 192 requests is now considered good for a single web page by today's standards.



---

* businessinsider.com - [Ads on news sites gobble up as much as 79% of users' mobile data](http://www.businessinsider.com/enders-analysis-ad-blocker-study-finds-ads-take-up-79-of-mobile-data-transfer-2016-3)

> "Ads on news sites gobble up as much as 79% of users' mobile data"

> One of the reasons consumers download mobile ad blockers is the impact ads have on their data plans. A report released Wednesday from Enders Analysis appears to back up that claim — at least when it comes to a sample of news websites.

I submitted the above BI article to [WebPageTest.org](http://webpagetest.org).

[results](http://www.webpagetest.org/result/160721_1W_1EQ1/) for First View, Fully Loaded:

* From: Dulles, VA - Chrome - Cable
* 7/21/2016, 2:58:49 PM
* Time = 17.922 seconds
* Requests = 298
* Bytes In = 3,463 KB 


---


* digiday.com [What agencies want from Google's bid to speed up mobile ads](http://digiday.com/agencies/agencies-want-google-amp-ads/)

> Google’s ongoing project to speed up the web with its Accelerated Mobile Pages has focused on how it can speed up page loads for publishers.

> The Catch-22 with digital ads is that as they’ve become richer over the years, they’ve also got heavier and, therefore, slowed page loads — a factor that’s had a fundamental role in the rise of ad blocking. Google sites research showing the average mobile site takes 19 seconds to load.

Web page bloat won't be reduced until people understand the cause of the problem. Note what the writer said about Google's AMP project, *"speed up the web."* That's incorrect.

The horribly slow page load time is not the fault of the mobile web infrastructure, mobile web browsers, nor WiFi and cell connections. It's 100 percent the fault of publishers.

The web is fine. Google is trying to speed up the page load time of web pages, hosted by bloated websites. Google is trying to do the work that publishers should be doing: simplifying a web page. Google is not speeding up the web. Google is trying to improve a reader's user experience because publishers cannot or will not do this.



---


* npr.org - [NPR.org Now Twice as Fast](http://www.npr.org/sections/thisisnpr/2015/10/27/451147757/npr-org-now-twice-as-fast) - Designer News [discussion](https://www.designernews.co/stories/58223-nprorg-now-twice-as-fast)

Designer News comment:

> Main reason it is faster than most news sites, beyond all this excellent work: they not beholden to 3rd-party advertising tech.



---


* opera.com - [New ad blocker - Built into the Opera browser](http://www.opera.com/blogs/desktop/2016/03/native-ad-blocking-feature-opera-for-computers)

> If there were no bloated ads, some top websites would load up to 90% faster.

Proper terminology was used. Websites would load faster not that the web would be faster. Websites are the problem not the web.


---



* digiday.com - [5 ways publishers' tech choices come back to haunt them](http://digiday.com/sponsored/5-ways-publishers-tech-choices-come-back-haunt)

The following admission came from a guest writer who works for an ad company. Will media people comprehend the article?

> Many of these tech “solutions” don’t add real value and instead **clutter up the user experience, slow down pages, and drive people away.** So we – the ad tech community – need to create products that **put the user experience first.**

> I’m not the first to observe that there are way too many pieces of executable code that run on publishers’ pages. Unsurprisingly, these scripts periodically crashed the sites on which they appeared.

> ... we commonly see more than 500 servers called from a single publisher page.  Most [page scripts] do nothing that benefits the publisher. On the contrary, they just leak data at best, and **at worst they reduce the consumer’s privacy and experience.**

> Furthermore, publishers may unwittingly be **violating their visitors’ privacy by allowing scripts to grab or use data without consent.**

> **Page scripts that cause latencies lead to delays in delivering content, turning impatient users away.** The longer the load times, the steeper the “user decay” curve, a term we use to describe the pattern of page abandonment caused by latency.

> Most publishers aren’t intentionally overloading a page with scripts to **create a horrid user experience,** goading their precious audiences into leaving or spurring them to install ad blockers. 

> When publishers can **learn what’s slipping onto their pages** and keep those pages working smoothly, they’ll have the control to **give users the experience they deserve.** 


---


* medium.com/@carsol - [Why you suck, not the mobile web](https://medium.com/@carsol/why-you-suck-not-the-mobile-web-cd1e233749d8#.w1hcurd58)

> The botching of the mobile web experience isn’t the phone broswer, it’s the web developer. Developers need to stop being lazy.


---


* cdixon.org - [The Decline of the Mobile Web](http://www.cdixon.org/2014/04/07/the-decline-of-the-mobile-web/) - and corresponding [Hacker News thread](https://news.ycombinator.com/item?id=7548530)

HN comment:

> Am I in the minority that I don't want an app for every. bloody. webpage. I visit?

Another HN comment:

> I also don't want every mobile webpage I visit to use some slow janky JavaScript framework to emulate native app behavior either because in my experience the user experience for those are universally worse than just trying to be a relatively normal web page (perhaps with some media queries for image sizes, etc) and letting the mobile web browser do its thing.




---


* idlewords.com - October 2015 - [Website Obesity](http://idlewords.com/talks/website_obesity.htm)

> Let me start by saying that beautiful websites come in all sizes and page weights. I love big websites packed with images. I love high-resolution video. 

> I love sprawling Javascript experiments or well-designed web apps.
**This talk isn't about any of those. It's about mostly-text sites that, for unfathomable reasons, are growing bigger with every passing year.**

> Here’s an article on GigaOm from 2012 titled "The Growing Epidemic of Page Bloat". It warns that the average web page is over a megabyte in size. The article itself is 1.8 megabytes long.

> Here's an almost identical article from the same website two years later, called “The Overweight Web". This article warns that average page size is approaching 2 megabytes. That article is 3 megabytes long.

> ... consider this 400-word-long Medium article on bloat, which includes the sentence: "Teams that don’t understand who they’re building for, and why, are prone to make bloated products." The Medium team has somehow made this nugget of thought require 1.2 megabytes.

> That's longer than Crime and Punishment, Dostoyevsky’s psychological thriller about an impoverished student who fills his head with thoughts of Napoleon and talks himself into murdering an elderly money lender.



---


* backchannel.com - [Google Is Going to Speed Up the Web. Is This Good?](https://backchannel.com/google-is-going-to-speed-up-the-web-is-this-good-a92a6043598b)

> “Sluggish” is too tame a word for what we endure now, due to an accumulation of terrible news-industry design and business choices in recent years.

> Before getting into details about what’s happening here, let’s be clear on something. AMP wouldn’t be necessary — assuming it is in the first place — *if the news industry hadn’t so thoroughly poisoned its own nest.*

> Looking for money in a business that grows more financially troubled by the month, media companies have infested articles with garbage code, much of it on behalf of advertising/surveillance companies, to the extent that readers have quite reasonably rebelled.

> We don’t like slow-responding sites, period. On our mobile devices, which are taking over as the way we “consume” information, we despise having to download megabytes of crapware just to read something, because the carriers charge us for the privilege.

> That’s one reason why we use ad blockers. (The other, at least for me, is that we despise being spied on so relentlessly.)

> The news business could have solved this problem without racing into the arms of giant, centralized tech companies. But it didn’t, and here we are.

> What if news sites had just done the right thing in the first place? Or, since they didn’t, *what if they just resolved to build faster pages* — using standard HTML markup and loading components in a non-annoying way — now?



---

* baldurbjarnason.com - [Facebook and the media: 
united, they attack the web](https://www.baldurbjarnason.com/notes/media-websites-vs-facebook)

> The web doesn’t suck. Your websites suck. All of your websites suck.

> You destroy basic usability by hijacking the scrollbar. You take native functionality (scrolling, selection, links, loading) that is fast and efficient and you rewrite it with ‘cutting edge’ javascript toolkits and frameworks so that it is slow and buggy and broken.

> You balloon your websites with megabytes of cruft. You ignore best practices. You take something that works and is complementary to your business and turn it into a liability.

> The lousy performance of your websites becomes a defensive moat around Facebook. The web is capable of impressive performance and offers a dramatically vaster reach and accessibility than anything an app can offer.



---


* daringfireball.net - [The New York Times on Apple's Dominant Position in Podcasting](http://daringfireball.net/linked/2016/05/09/nyt-podcasts)

> JavaScript has brought the web to the brink of ruin, but there’s no JavaScript in podcasting. Just an RSS feed and MP3 files.

I understand what Gruber was saying, but I would qualify it more.

"The **misuse** of JavaScript has brought the web to the brink of ruin."

It's not the usage of JavaScript that's the problem. It's the excessive, unnecessary usage.

Who gets to define the misuse? Does the article page or site function fine without JavaScript? What does a thousand pounds of JavaScript files do for the single article page that's accessed by a browsing-only reader?

For a site that requires the user to login, then I expect the dashboard or admin interface to employ JavaScript in an elegant manner that has been designed and developed by extremely talented people.

In my opinion, that happens when I log into my Digital Ocean account. Their usage of JavaScript is elegant. The JavaScript helps make the experience smooth and easy. The JavaScript is not used to show-off. The JavaScript seems to be a background experience. The experience is smooth and maybe unnoticeable, which is even better. I log in, perform a task or two, and then exit. I'm not looking to be wowed by fancy tech.

Ditto for my FastMail account, which is my favorite email service. In my opinion, FastMail's JavaScript usage is also elegantly used.

For content sites where I don't login, I don't understand the overuse of client-side JavaScript. That's why I surf the web with JavaScript and other things disabled by default, thanks to the NoScript plugin for Firefox.

Using JavaScript for useless extravagance is breaking the web.




---


* Hacker News [discussion](https://news.ycombinator.com/item?id=11798646) about an article titled [The real responsive design challenge? RSS.](https://begriffs.com/posts/2016-05-28-rss-responsive-design.html)

Top-rated HN comment:

> On a more serious note - RSS is the Great Web Leveller. It spites your fancy CSS hacks, it's disgusted by your insane javascript, and it will piss all over your "mobile-optimized" crap. No semantic markup == no party; because markup is for robots, and RSS parsers are very stubborn robots that can see through web-hipster bullshit like Superman through walls.


Another HN comment well down in the thread:

> Regarding reading news on the Kindle: I've noticed that the browser becomes much more responsive (read: usable) if one disables JavaScript altogether. 

> Sure, some websites will break, but most will work well enough to be able to read articles.

> Disabling JavaScript is also my trick for actually being able to browse the internet on a phone these days. In Firefox for Android, you can install a plugin to toggle it on/off for when you need it.

> A bit sad that you have to do this to get at decent experience, but what can you do...

I read many websites with JavaScript disabled within the browser on my desktop and laptop computers. At times, it feels like the latest, greatest CPU is required to read web articles, especially those produced by media orgs. Pages load incredibly fast when javascript is disabled. 

Web pages also load fast when viewing sites with the text-based browser called Links.


---

Speaking of text-based access to websites ...


* daniel.haxx.se - March 20, 2015 - [Curl, 17 Years Old Today](http://daniel.haxx.se/blog/2015/03/20/curl-17-years-old-today) - corresponding Hacker News [discussion](https://news.ycombinator.com/item?id=9236551)

Here are a few HN comments with my emphasis bolded and additions contained within brackets:

> "If it doesn't load through curl, it's broken." --someone 
So, so true. Thanks, curl.

> I wasn't saying not to do the fancy stuff but rather to start with something which degrades well and then **have your JavaScript enhance that basic experience.** 

> I've been using websites since the early 90s and this pro-single-page sentiment [SPA] is getting really tiresome. **You are breaking the web.** You are destroying users' security. Sure, there are **plenty of reasons to use JavaScript, and plenty of places where it's appropriate.** It probably is a good idea for games and so forth. But requiring users to load and execute constantly-changing code from across the web **in order to read a page** or submit a form is in-friggin-sane.

> Some one else pointed out that it'd be nice if browsers offered more support for things that certain types of developers clearly want to do. I completely agree; it'd definitely be nice to take advantage of many of the technologies which currently exist to do more, in a more structured way. **But requiring code execution in order to read data [plain text] is madness.**



---


* 500ish.com - [Drinking the Web Through A Straw](https://500ish.com/drinking-the-web-through-a-straw-75ab685a1763)

> Because on the desktop we’re all used to seeing the absolute worst of the web. That is, ridiculous widgets, awful JavaScript load times, and, of course, ads galore. AMP stripped all of the crud away and just gave me unadulterated content. And gave it to me fast.

> It was such a revelation. I wanted to view all web-based content this way. Not just on mobile, everywhere.

Welcome to the dark side of wanting faster, simpler, browsing-only websites.  As mentioned above, a similar experience can be had by disabling JavaScript within the web browser. Google AMP is needed if the website is poorly designed.



---


* wired.com - [I Turned Off JavaScript for a Whole Week and It Was Glorious](http://www.wired.com/2015/11/i-turned-off-javascript-for-a-whole-week-and-it-was-glorious) - HN [discussion](https://news.ycombinator.com/item?id=10593276)

From the Wired.com article:

> THERE’S ANOTHER WEB out there, a better web hiding just below the surface of the one we surf from our phones and tablets and laptops every day. A web with no ads, no endlessly scrolling pages, and no annoying modal windows begging you to share the site on social media or sign up for a newsletter. 

> The best part is that you don’t need a special browser extension or an invite-only app to access this alternate reality. All you need to do is change one little setting in your browser of choice. Just un-tick the checkbox that enables “JavaScript” and away you go, to **a simpler, cleaner web.**

> **Pages loaded nearly instantly,** my laptop battery lasted longer, and I could browse the web with fewer distractions—all without the sense of guilt that comes with using an ad blocker.



---


* medium.com/@pete - [How many floppy disks do you need to fit an article from The Atlantic?](https://medium.com/@pete/how-many-floppy-disks-do-you-need-to-fit-an-article-from-the-atlantic-8924a9e057ff)

> In case your experience with computers started after 2010, this: [image] … is a 3.5 inch floppy disk. Standard capacity: 1.44MB.

> Today, I tried to read this (really quite good) article from *The Atlantic* on my iPhone 5S. First time around I tried in a webview. Next attempt was in Safari. It crashed both of them.

> Digging for Dinosaurs in My Twenties is a little over 6,200 words and has four images. Saved in rich text format, the words come to 37KB of data, the four images total 346KB (exactly the same images are served to my desktop browser as are to my phone).

> Given all the information so far, guess how many floppy disks it would take to fit an article from The Atlantic?

> **Answer: at least 15**

> “No, no,” I hear you grumble, “37 plus 346 equals 383KB which is a little over one quarter of the 1.44MB capacity of a floppy disk.”

> Well, of course. Unless you include all the other crap that comes with the article.

> By the time Safari had crashed, **I’d logged 21MB of ads, pixels, and associated scripts that had been downloaded onto my phone.** If the main idea was to **heat my phone so my hand could stay warm** against the San Francisco fall, nice job everybody!

> If, on the other hand, the idea was that I could read the article, without **scrolling being deathly sluggish,** and maybe actually make it to the end before it crashed the browser. **Yeah, you failed.**

> ... seriously… does anybody at The Atlantic **read their own content on their own site?** On a phone… just the same as an ever-increasing number of users consume content? Or were they too busy checking it in Instant Articles and Apple News to take a look at their own mobile view?



---

* Hacker News [discussion](https://news.ycombinator.com/item?id=11517491) about the websites listed at [brutalistwebsites.com](http://brutalistwebsites.com)

HN comment:

> Just showed some of these to a generally non-tech-savy friend who said he didn't like them because they looked "too 90s." Personally I love them because **they load fast, are easy to read,** and don't require a knowledge of a bunch of different frameworks to write.


Another HN comment:

> I have been fighting for years to get people used to "90s aesthetics."

> It's even more important for web design. Give me simple HTML with a touch of css, and javascript **only if it's absolutely necessary.** I can think of hardly any websites that I would consider "beautiful" these days for exactly this reason.

> PS: I'm not sure I would classify these sites as brutalist; perhaps 'utilitarian' or 'functional' would be better descriptors.

HN comment:

> You can make something that doesn't require tons of frameworks and loads fast while NOT looking like a relic of the days of Kazaa. The fact that so many developers are too lazy to do so does not mean we should throw the baby out with the bathwater and go back to times new roman black-on-white.

Worthwhile CSS and JavaScript are fine.

HN comment:

> As an overt visual design paradigm, meh. But hallelujah to the idea of a page that just has content, without the trendily de rigeur fucktons of overblown css and pointless javascript that adds 0 and only serves to crash my crappy mobile browser.



<http://thin.npr.org>

thin.npr.org is a better web design than most slick-looking media websites today. Okay, it lacks the viewport to display nicer on a phone, but at least a reader can read the site in landscape mode, and the reader can zoom into the content to enlarge the text size. And the browser back buttons work properly with the site. Links are underlined. 

The NPR thin site supports the open web better than most websites. It uses minimal HTML. The pages are lightweight and fast-loading. A sprite of inline JavaScript exists: 4 lines with two lines being curly braces. No external JavaScript is loaded. No inline nor external CSS is used.

webpagetest.org [results](http://www.webpagetest.org/result/160726_B2_1EBA/) for thin.npr.org article [FBI Investigates Possible Russian Connection To Leaked DNC Emails](http://thin.npr.org/s.php?sId=487480514&rId=1001&x=1) - From: Dulles, VA - Chrome - Cable - 7/26/2016, 4:06:41 PM - First View Fully Loaded:

* 0.258s
* 2 requests
* Bytes In = 4 KB
* Cost = $

Obviously, the web works well. This news story would load fast over a slow internet connection. If the article contained a viewport mention, inside the top of the HTML page, along with a smidgen of CSS, then the page would display better on a phone. But at least a phone user can zoom into the article and/or read the article in landscape mode.


---


* mobiforge.com - April 2016 - [The web is Doom](https://mobiforge.com/research-analysis/the-web-is-doom)
  * Hacker News - [discussion](https://news.ycombinator.com/item?id=11548816)
  * wired.com - [The Average Webpage Is Now the Size of the Original Doom](http://www.wired.com/2016/04/average-webpage-now-size-original-doom/)

From the mobiforge.com article:

> In July 2015, inspired by something Mat Marquis said at TXJS 2015, I suggested that the average web page weight would equal that of the Doom install image in about 7 months time.

> Well, we’ve made it, albeit a bit later than expected.

> Recall that Doom is a multi-level first person shooter that ships with an advanced 3D rendering engine and multiple levels, each comprised of maps, sprites and sound effects. By comparison, 2016’s web struggles to deliver a page of web content in the same size. **If that doesn’t give you pause you’re missing something.** 

From the Wired.com article:

> Today the average webpage is about the same size, data-wise, as the classic computer game Doom, according to software engineer Ronan Cremin.

> A compressed copy of the installer for the shareware version of Doom takes up about 2.39MB of space. Today’s average webpage, meanwhile, requires users to download about 2.3MB worth of data, according to HTTP Archive, a site that tracks website performance and the technologies they use.

> That’s not totally analogous comparison, but it does illustrate the web’s growing obesity problem. our story on giving up JavaScript for a week weighs in at 3MB.

> So how did we get here? As internet connections have gotten faster, publishers and developers worry less about efficiency. 


---

* eev.ee - [Maybe we could tone down the JavaScript](https://eev.ee/blog/2016/03/06/maybe-we-could-tone-down-the-javascript)

> I can almost hear the Hacker News comments now, about what a luddite I am **for not thinking five paragraphs of static text need to be infested with a thousand lines of script.** Well, let me say proactively: fuck all y’all. 

> I think the Web is great, I think interactive dynamic stuff is great, and I think the progress we’ve made in the last decade is great. I also think it’s great that the Web is and always has been inherently customizable by users, and that I can use an extension that lets me decide ahead of time what an arbitrary site can run on my computer.

> I’m not saying that genuine web apps like Google Maps shouldn’t exist. I’m saying that something has gone very wrong when basic features that already work in plain HTML suddenly no longer work without JavaScript. 

> 40MB of JavaScript, in fact, according to about:memory — that’s live data, not download size. That might not sound like a lot (for a page dedicated to showing a 140-character message?), but it’s not uncommon for me to accumulate a dozen open Twitter tabs, and now I have half a gig dedicated solely to, at worst, 6KB of text.

> Maybe one day a year, get your whole dev team to disable JavaScript and try using your site. Commence weeping.

> The web is not a video game console; act accordingly. Keep your stuff modular. Design proactively around likely or common customizations. **Maybe scale it down a bit once you hit 40MB of loaded script per page.**


Sometimes, it's necessary for a web site to function like a native app, but I don't think that includes media websites where the user is only reading the content.

For text-heavy websites, publishers should build websites, instead of trying to build native app sites. If publishers want native app functionality, then they should build a native app. Publishers should quit trying to make websites act like native apps.

When I log into sites that provide functions such as:

* email
* tax preparing
* banking
* publishing
* project management
* survey building

... then I expect a JavaScript-enhanced interface. And when it is done elegantly, the experience is pleasant and satisfactory. I complete the desired tasks, and I move on.

Could those web sites/apps/services function with JavaScript disabled? Possibly, but the experience could be awkward, slower, and error-prone. 

When the necessary JavaScript is used, then it's fine. Elegance over extravagance. The focus should be on utility.


---




* medium.com/@wob - [The sad state of web development](https://medium.com/@wob/the-sad-state-of-web-development-1603a861d29f)

The author expressed strong opinions on many web development areas, including Single Page Applications and React.js.

> "Really all I’m saying is don’t build a SPA. A SPA will lock you into a framework that has the shelf life of a hamster dump. When you think you need a SPA, just stop thinking."

> From what I can tell the background of React is: Facebook couldn’t create a notification indicator on Facebook.com, so they create this over engineered dump pile to solve that problem. Now they can tell you how many unread posts you have while downloading 15 terabytes of Javascript. 

> I have the Chrome plugin that shows when a site uses React. I swear every other website I visit uses React, for the stupidest stuff. So many content sites use React. It’s pitiful.

> Good job Yahoo, you rewrote your shitty mail client in React. Your customers didn’t give a shit. They just want it to work. My poor wife with her shitty Chromebook. She can play Crysis at 60fps, but fuck if she can read her email on Yahoo.

I rarely use my Yahoo email account, and I agree, it's a garbage web app. I started using Yahoo email in 1999, and I would bet that their '99 version would be more useful than their 2016 version. But I don't blame React.js for Yahoo's poor email app design.


---


* joneisen.me - [Great state of web development](http://joneisen.me/2016/01/13/great-state-of-web-development.html)

> The world wants Single Page Apps (SPAs), meaning we have to move huge amounts of logic from the server to the browser. We’ve been doing this for years, but in 2015, we’ve found better ways to build these large sprawling front end apps.

Eewww. Maybe the world wants native apps. Why not simply build native apps?

Are these SPAs used for internal web apps at companies to perform tasks by logged-in users? If so, then okey-dokey.

> ... we’ve found better ways to build these **large sprawling front end apps.**

Great. Saddle users' devices with large, sprawling front-end apps. If these piles of steaming poop are used to display text-based content to non-logged-in users, then why build them?

If the user-experience is improved, then the SPA is a success. If the user-experience is diminished by a bloated, sluggish, clunky web site, then the SPA is a massive failure. Return to 1995 web development and then progressively-enhance with a light touch.


---


* baldurbjarnason.com - [Facebook and the media: 
united, they attack the web](https://www.baldurbjarnason.com/notes/media-websites-vs-facebook)

> The web doesn’t suck. Your websites suck. All of your websites suck. You destroy basic usability by hijacking the scrollbar. You take native functionality (scrolling, selection, links, loading) that is fast and efficient and you rewrite it with ‘cutting edge’ javascript toolkits and frameworks so that it is slow and buggy and broken. 

> You balloon your websites with megabytes of cruft. You ignore best practices. You take something that works and is complementary to your business and turn it into a liability. The lousy performance of your websites becomes a defensive moat around Facebook.

> If your web developers are telling you that a website delivering hypertext and images can’t be just as fast as a native app (albeit behaving in different ways) then you should fire them.

> Peter-Paul Koch, [web browser tester extraordinaire,](http://www.quirksmode.org/mobile/) picks up on the phrase that I highlighted in the John Gruber quote and runs with it.

> > The web definitely has a speed problem **due to over-design** and the junkyard of tools people feel they have to include on every single web page. However, **I don’t agree that the web has an inherent slowness.** The articles for the new Facebook feature will be sent over exactly the same connection as web pages. However, the web versions of the articles have an extra layer of cruft attached to them, and **that’s what makes the web slow to load. The speed problem is not inherent to the web; it’s a consequence of what passes for modern web development.** Remove the cruft and we can compete again.
Tools don’t solve the web’s problems, they ARE the problem by Peter-Paul Koch 

> We continue to have this problem because your web developers are treating the web like an app platform when your very business hinges on it being a quick, lightweight media platform with a worldwide reach.

> The web is capable of impressive performance and offers a dramatically vaster reach and accessibility than anything an app can offer.



---


* blog.chriszacharias.com - 2012 - [Page Weight Matters](http://blog.chriszacharias.com/page-weight-matters) - Hacker News [discussion](https://news.ycombinator.com/item?id=10393930)

HN comment:

> If you have an engineering mind and care about such things - you care about complexity. Even if you don't - **user experience matters to everyone.**

> Have you ever seen something completely insane and everyone around doesn't seem to recognize how awful it really is. That is the web of today. 60-80 requests? 1MB+ single pages?

Man, the olden days of only 1mb web pages. More from the HN commenter:

> Your functionality, I don't care if its Facebook - does not need that much. It is not necessary. When broadband came on the scene, everyone started to ignore it, just like GBs of memory made people forget about conservation.

> The fact that there isn't a daily drumbeat about how bloated, how needlessly complex, how ridicuous most of the world's web appliactions of today really are - baffles me.


But I disagree with this HN comment:

> The real problem of web development is JavaScript. It’s a relic of the past that hasn’t caught up with times and we end up with half-assed hacks that don’t address the real problem. We need something faster and way more elegant.

I'm writing this page from within the JavaScript editor open source code that I borrowed in the summer of 2013 and then hacked to meet my requirements. I have installed versions of this editor in my Junco, Grebe, Scaup, Veery, and Wren web publishing apps. I can use it easily on my phone. I write fast with it. It works for me and my web writing purposes. **For this, I LOVE JavaScript.** 

And "editor" may be an incorrect term to use for "my" writing app. I disabled features that existed in the original code, and I added several new features. The code uses Ajax to send and receive JSON. The JavaScript editor sends markup to the server where the server code converts it into HTML and returns it to the editor. Simple. It's my preferred writing environment for the web.

My Grebe, Scaup, and Veery web publishing apps caches pages and the homepages in Memcached. If the page is not cached, it's pulled from the MySQL or CouchDB database, and then it's cached. Most of the time, browsing-only users receive the cached page. 

My Wren publishing app does not use a database. It creates static HTML pages. I'm using Wren to create this and the other related pages.


---


* wsj.com - [Google Starts Including AMP Content in Mobile Search Results](http://www.wsj.com/articles/google-starts-including-amp-content-in-mobile-search-results-1456326159)

> “We want to make it really easy for publishers of all shapes and sizes to publish AMP-formatted pages, from the New York Post all the way down to people running their own personal blogs,” said Paul Maiorana, vice president of platform services at WordPress.com parent company Automattic.

Why not create simple, fast-loading, reader-friendly pages by default?

> Under the hood, AMP works by simplifying and streamlining the HTML code that powers Web pages to prioritize speed. Google also “caches” pages, or saves copies of them on its own systems, in order to deliver them quicker when users access them. It’s an open-source initiative, meaning anyone is free to use it.

Again, content producers on their own can create simple HTML pages, and they can cache their own content for faster access, thus creating a reader-friendly experience.



---


* filamentgroup.com - [Delivering Responsibly](https://www.filamentgroup.com/lab/delivering-responsibly.html)

> ... page weight does matter. Access can be slow, expensive and prohibitive.

> People have come to learn that web fonts take a long time to load. Boom! Just disable them. And along with custom fonts, there go the icon fonts too, so we need to be thinking about fallback images and text for font icons. Or better yet, use SVG instead.

> Most importantly, if disabling enhancements like JavaScript or ads ends up breaking your site, will people just assume that your site is down? I suspect they will. I would.

> And really who would blame people for reacting to the web this way? Our own practices have set the stage for blockers to become enormously popular.

> And I think reach is the greatest advantage of web technology. If we do our jobs well, our sites can reach folks who access the web under very different circumstances than many of we web designers do day to day.

> Tim Kadlec recently built [What Does My Site Cost .com.](http://whatdoesmysitecost.com/) It’s a website that calculates the real cost of accessing any site on the web using the costs of the cheapest data plans around the world.

> For example, **an article on the Wired site weighs over 11.27 mb.** For some people it costs almost $4 US dollars to visit that page! For many it's at least a dollar.

> Lastly, the tool I’d recommend most is [webpagetest.org](http://webpagetest.org/). It's a website. You can enter a URL, choose a browser/device combination to test, and a region of the world to run the test from, and webpagetest will load your page from there and give you all sorts of information about how it loaded. It’s my favorite tool for development and testing.



---



............................................................................







http://www.niemanlab.org/2016/02/diving-all-in-or-dipping-a-toe-how-publishers-are-approaching-googles-accelerated-mobile-pages-initiative/

> “Mobile web performance is bad — I challenge you find someone who disagrees with that,” Mic’s chief strategy officer Cory Haik told me.

I would vehemently disagree. The mobile web performance is not bad. Your obnoxiously bloated and clunky website is bad. You create a reader-hostile experience and then blame something else.

> “When our pages load too slowly on mobile, as a publisher, we’re losing an audience, and that is painful. So we’ve been excited to build on AMP.”

Cuckoo time.



---

Here's how to speed up an article page:

* use no javascript
* cache the page
* create static HTML


---


Webpagetest.org 

Another testing service:

https://developers.google.com/speed/pagespeed/insights



http://m.toledoblade.com/Featured-Editorial-Home/2016/03/06/Yes-on-Toledo-tax.html

Speed:

Mobile = 33 / 100
Desktop = 64 / 100
I don't understand. The mobile version of the Blade's website is slower on mobile than their desktop version, and the mobile version is faster on desktop than their desktop version. At least according Google's PageSpeed test. Whatever, it's all very slow.


http://toledotalk.com/yes-on-toledo-tax.html

Incredibly boring webpage, but it's the same content.

Speed:

Mobile = 99 / 100
Desktop = 99 / 100
ToledoTalk.com is hosted on a shared server at HE.net, meaning that TT shares a computer that also hosts dozens of other websites. Obviously, I don't have root access. The speed rating would be 100/100 if I could enable compression within the Apache web server.

For my other sites, I host at Digital Ocean, and I have total access to my own virtual server. I use the Nginx web server. That same HTML page does receive a 100/100 score.

At webpagetest.org:

Fully Loaded:

Time: 0.535s
Requests: 2
Bytes in: 14 KB
Apache at HE.net must be adding some additional info because that
boring ass web page is a little over 8,000 bytes in size on the file system, due to the HTML tags and some CSS.

When the version at Digital Ocean is tested, the Bytes In equals 5 KB, due to Nginx compression.


The same op-ed:

5,000 bytes downloaded versus the Blade's version which requires over 5 megabytes to be downloaded.
Fully loading in under a second versus requiring over 40 seconds to load completely.
Making only 2 requests versus over 900 requests!!! (what in the hell is going on there?)
I'm always impressed by consumers' ability to tolerate mediocrity and abuse.



I feel bad for the writers, editors, and everyone else at newspaper orgs. Their service is needed at the local level, in my opinion.

But this kind of web design indefensible, and I would never support it with money.

I have no sympathy for media orgs if their business declines when they abuse web readers like this.

Writers and editors may feel that they cannot do anything about their company's wretched web design, but I disagree because I assume that those people also use the web, and they work at these companies.

Anyway, the keys are no JavaScript, no tracking gobblygook, and no ads. 

I suppose that I would be the only person willing to pay a hefty annual subscription fee for content that was displayed that simply. Photos and illustrations are still welcomed. In fact, more images should be posted. Just greatly simplify the delivery container.

A fast, simple delivery mechanism does not improve bad writing. But good writing, important writing can be lost or ignored when the delivery mechanism is a train wreck.

Even digital-only media sites that formed in recent years and never created a print version are designing massively bloated websites.

But I see no improvements in the future by newspaper/media orgs, regarding their reader-hostile web designs. The only change will be that the websites will get worse.

Thanks to slow websites, we will have more services like Facebook's Instant Articles and Google's Accelerated Mobile Pages because most people read on their phones.

Some day, it may be pointless for news orgs to have their own websites because the media orgs will publish their content on many other platforms. It's not Facebook's fault. It's the fault of the publishers for designing web pages in 2016 that are 5 to 15 megabytes in size.

And if the local, daily newspapers close, I'll get my "news" by overhearing pointless third-hand drivel from people who read Facebook.



---













https://stratechery.com/2015/why-web-pages-suck/ 
https://news.ycombinator.com/item?id=9891927

> John Gruber had strong words about Apple news site iMore:
> > I love iMore. I think they’re the best staff covering Apple today, and their content is great. But count me in with Nick Heer — their website is shit-ass. Rene Ritchie’s response acknowledges the problem, but a web page like that — Rene’s 537-word all-text response — should not weigh 14 MB.1.
It’s not just the download size, long initial page load time, and the ads that cover valuable screen real estate as fixed elements. The fact that these JavaScript trackers hit the network for a full-minute after the page has completed loaded is downright criminal. Advertising should have minimal effect on page load times and device battery life. Advertising should be respectful of the user’s time, attention, and battery life. The industry has gluttonously gone the other way. iMore is not the exception — they’re the norm. 10+ MB page sizes, minute-long network access, third-party networks tracking you across unrelated websites — those things are all par for the course today, even when serving pages to mobile devices. Even on a site like iMore, staffed by good people who truly have deep respect for their readers.








This is hilarious and extremely ironic: http://www.theverge.com/2015/7/20/9002721/the-mobile-web-sucks

> I hate browsing the web on my phone. I do it all the time, of course — we all do. But man, the web browsers on phones are terrible. They are an abomination of bad user experience, poor performance, and overall disdain for the open web that kicked off the modern tech revolution. 


I disagree. The problem is not with the mobile web browsers. The problem is with the WEB SITES.

Web sites are an "abomination of bad user experience, poor performance, and overall disdain for the open web."

And the Verge.com is one example of a web-abusive site. It's home page is horribly slow-loading thanks to way too many useless images and probably javascript. With javascript disabled, the site's home page loads significantly faster.

These bloated websites require users to have brand new computers with the latest, fastest CPUs.


> Mobile Safari on my iPhone 6 Plus is a slow, buggy, crashy affair, starved for the phone's paltry 1GB of memory and unable to rotate from portrait to landscape without suffering an emotional crisis.


I've never had remotely close to those problems in the 12 months that I've been using my iPhone 5C. I'm still using iOS 7.

> Chrome on my various Android devices feels entirely outclassed at times, a country mouse lost in the big city, waiting to be mugged by the first remnant ad with a redirect loop and something to prove.


Um, okay. This person is not a writer.

And I've not had an issues with the Chrome browser on my iPhone. I like the fact that the browser has defaulted to the fast, smooth scroll when viewing websites. Maybe this will be the default for all mobile browsers someday. Then we'll have no need to design a website with the special CSS to make fast, smooth scroll occur. That CSS munges up other functionality within a mobile browser, like having the top and bottom sections of the browser disappear or shrink when scrolling.

Granted, this is only theverge.com, and maybe that's why this article lacks intelligent thinking.


> The overall state of the mobile web is so bad that tech companies have convinced media companies to publish on alternative platforms designed for better performance on phones.


It's not because of poor mobile browsers and poor phone hardware. It's because of horribly designed websites by media orgs. 

So typical. A media company blames someone else.

Way down in that lengthy article, the writer finally states something intelligent.

> Now, I happen to work at a media company, and I happen to run a website that can be bloated and slow. Some of this is our fault: The Verge is ultra-complicated, we have huge images, and we serve ads from our own direct sales and a variety of programmatic networks. Our video player is annoying. 

> We could do a lot of things to make our site load faster, and we're doing them.


Finally, admitting, in a round-about, back-handed way, that it's the media company's fault. And I would say it's 100 percent the media company's fault.

Yet ...


> But we can't fix the performance of Mobile Safari.


The writer or theverge.com should design that article page with bare-minimum html, 1995-style, and then load it as a static page and test the load speed on mobile Safari. 

Add a meta tag with the viewpoint attribute to make the page read better on the phone. And then add a tiny CSS page with a little formatting and maybe a font-family load and a media query. But keep it focused on something useful.

And test that page load time.

Oh, no JavaScript. Don't need it for a user who is only reading the page.

 


Jul 21, 2015 tweet
https://twitter.com/richardpenner/status/623498582805512192

> The Verge article blaming browsers for a shitty mobile web is 6MB and has more than 1,000 javascript errors.

























http://product.voxmedia.com/2015/5/6/8561867/declaring-performance-bankruptcy




http://mattgemmell.com/the-reader-hostile-web/

https://timkadlec.com/2015/05/choosing-performance/


good
http://digiday.com/publishers/gq-reversed-declining-homepage-traffic/
http://digiday.com/publishers/gq-com-cut-page-load-time-80-percent/


shaky
http://digiday.com/publishers/washington-post-cut-page-load-time-85-percent/


reddit : [rise and fall of the gopher protocol](https://www.reddit.com/r/programming/comments/4xd2c7/the_rise_and_fall_of_the_gopher_protocol/)

[#manifesto](/tag-manifesto.html)
