# The ‘Zine
# tl;dr
The ‘Zine is an online magazine started and run by Meghna Gulati, that seeks to provide a platform for the stories and thoughts of the Indian youth. I was responsible with designing and developing the [initial version of the site](http://zine-old.prabhav.xyz), back in 2013. Two years after the initial launch, I was contacted again for a redesign. My job was mainly to do 3 things: *revamping the whole content structure of the magazine*, *crafting a new visual aesthetic*, and *coding the whole site with a CMS-backed infrastructure*. So yeah, I was pretty much turning the whole magazine over on its head.

# Problems with earlier design:
## 1. Content Structure 
#### aka *Column-Columnists? Articles-Writers?*

When it was launched, the site was made to follow a traditional magazine content format based on columns - a writer was given a particular topic to write on, and they publish subsequent issues of the same in a quarterly fashion.

> For instance, one of the columnists, Rahat Chawla, maintained a column on food reviews. So every quarter, he would review a restaurant and write about it. Screenshots from issues 3, 4, and 5.  

![](The%20%E2%80%98Zine/Screenshot%202017-02-16%2014.27.35.png)
![](The%20%E2%80%98Zine/Screenshot%202017-02-16%2014.28.57.png)
![](The%20%E2%80%98Zine/Screenshot%202017-02-16%2014.29.15.png)



### Main problems with this model:

* [maybe a bulb icon for these bullets] Writers complained of being bored—and sometimes out of content for a scheduled issue release [insert screenshot example]
* As a result, readers reported that writers sometimes went out of their content zone and sometimes the content overlapped with other columns [insert screenshot example]

## 2. Publication Schedule & Content Management System
The site followed a quarterly publication schedule, like a magazine has issues. So, every 3 months we had to get together all the articles and code it all out. What made it even harder was the fact that since the first version was  build in a rush, the infrastructure wasn’t based on a Content Management System. 

* Since the site was updated only every 3 months, the time between the issue releases was a very heavy lull for the traffic. Traffic on the site sharply dropped after almost 2-3 weeks of the release, and users even reduced engagement on the social media profiles—primarily because of the lack of fresh content.
* The lack of a content management system of course made the issue update season ever harder. The backend was based on Liquid-based template system that ran on [Mixture](http://mixture.io)—which ran without a client-accessible editor. 

## 3. Layout and Aesthetics
### *It just doesn’t look and feel like an online magazine.*

* The look of the old site made it look more like a marketing site, and not a publication—for which the site should be as content-centric as possible.

![](The%20%E2%80%98Zine/Screenshot%202017-02-16%2022.51.44.png)

* Navigating through the content wasn’t convenient for the reader/user too, as instead of the title/subtitle/banner image, the previous site went with a traditional magazine-style *Contents* page system.

<a href='The%20%E2%80%98Zine/contents%20scroll.mov'>contents%20scroll.mov</a>

* Also, the client also reported that the visual aesthetic of the site didn’t reflect the desired *editorial look and feel*, and looked a bit more “playful” and “chirpy” that needed.

## 4. Article Structure
* There wasn’t a **tags** or **categories** system to index and sort articles by similar content.
* The client wanted to separate the normal articles with articles about the magazine itself, like the editorials. In the original site, there was a homogenous flavor to all the articles, and there was no way to visually or functionally separate article *for* the magazine and articles *about* the magazine.
* The client reported that the articles required some visuals or a banner image attached to them to give a visual context of the article.
* The client also demanded a share button to *facebook* and *twitter* as a means to share the articles quickly on social media networks.

# The Redesign
![](The%20%E2%80%98Zine/Screenshot%202017-02-19%2008.55.35.png)

## 1. Content Strategy and Information Architecture
To combat the various problems the client and the readers experienced because of the traditional *quarterly, column-based* publication system, I decided to *completely revamp* how the magazine functioned. 

* **From Columns to No-Columns**: We decided to move from a column-based system (where every writer sticks with their own theme), to a more free-flowing blog/article system. This gave the writers the flexibility they demanded to flex their writing muscles in every direction—and since there were no set columns, overlapping of content themes was not only unproblematic, but also beneficial. 

## 2. Publication Schedule and Content Management System
* **From Quarterly to Anytime**: From a quarter-based publication schedule that only encouraged sporadic traffic, we developed a more regular and flexible publication (blog-style) schedule:
* **Staff Flexibility**: In addition to encourage a more flexible and open writer-base, when writers wanted to leave, if hurt the magazine less—and as a result, the content stream was kept fresh and diverse. 
* **From Static to Siteleaf (and Jekyll)**: From a partially hard-coded codebase, I moved the content and code to a automated content-management system. Instead of involving me in the update process, editors and writers could publish article themselves easily. The back-end is now based on Jekyll (for increased portability and hosting-ease) and the build system was moved from (the deprecated) liquid-based [Mixture](http://mixture.io) to [Grunt](http://gruntjs.com/) .

![](The%20%E2%80%98Zine/Screenshot%202017-02-19%2008.37.43.png)

![](The%20%E2%80%98Zine/Screenshot%202017-02-19%2015.56.45.png)
![](The%20%E2%80%98Zine/Screenshot%202017-02-19%2015.57.36.png)


## Layout and Aesthetics
- **Content-centric Design**: Rather than self-advertisement and calls-to-action being in the focus, it was a dire need for the website to accurately depict what was at its heart: *the articles* and the content.
- From having to access a flat list of articles, the readers could now browse through nugget-sized article modules and even browse by category.
- As pushed-for by the client and to match with the magazine’s tone, I went with a more subtle, less bright, and less colorful aesthetic. Here are some early prototypes and comps I made as drafts:

![](The%20%E2%80%98Zine/zine%20-%20archivo%20narrow.png)

![](The%20%E2%80%98Zine/zine%20-%20topics.png)
![](The%20%E2%80%98Zine/zine%20mockup.png)
![](The%20%E2%80%98Zine/zine%20-%20masonry%20bare.png)

![](The%20%E2%80%98Zine/zine%20-%20bare%20home.png)
![](The%20%E2%80%98Zine/Screenshot%202015-06-30%2013.57.00.png)
![](The%20%E2%80%98Zine/Screenshot%202015-07-02%2017.43.05.png)


![](The%20%E2%80%98Zine/Screenshot%202015-09-03%2016.35.47.png)
![](The%20%E2%80%98Zine/zine%20-%20article%20meta.png)
![](The%20%E2%80%98Zine/Screenshot%202017-02-19%2016.31.56.png)
![](The%20%E2%80%98Zine/Screenshot%202017-02-19%2016.39.36.png)

## 4. Article Structure
- I Introduced **categories** to mark the articles into the six streams of content the magazine published.

![](The%20%E2%80%98Zine/tags.png)

- I Introduced a **blog** section to publish articles about announcing meet-ups, sharing progress, and in general publishing content *about* the magazine itself.
- Solving the problems listed earlier, a banner image to each article and social share buttons on the article pages were also added.



 #work/case-study