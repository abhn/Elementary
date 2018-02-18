# Elementary Jekyll Theme

Elementary is a zero Javascript and minimal CSS ultra lightweight Jekyll theme for those of you who love simplicity, yet don't want to compromise on mobile responsiveness, readability and asthetics. Elementary is mobile first, content first and is aimed towards content heavy blogs.

The theme is highly customizable, takes less than 100 miliseconds to load, weighs less than 10K gzip'd and looks great on mobile. As vanilla as a website can get, this theme reminds the visitor of the pre 2000s era Internet, yet is backed by the modern CSS flexbox layout and has a sticky footer made with the same.

<img src="https://github.com/abhn/Elementary/blob/master/tmp/multi-display.png?raw=true">

### Demo
Find it here: 

### Features
- Ultra lightweight, ~6-9KB gzip'd, load times consistently less than 100 milliseconds (as tested on my personal blog with Cloudflare)
- Mobile responsive, high accessibility
- No JS required, makes use of HTML5 and CSS3 semantics
- Theme itself makes a single http request
- Content focussed, great for text heavy personal blogs with focus on blog material
- Homepage is the archive page
- Sticky footer (is it 2018 yet? ;)

### Installation
- If this is your first Jekyll blog, follow this <a href="https://jekyllrb.com/docs/installation/">helpful guide</a> to set up Jekyll
- Fork this repository, rename the fork as `your-username.github.io`. Your blog should immediately be live on `https://your-username.github.io`
- Clone your fork
- Delete everything in `_posts` directory. Delete the `tmp` directory
- Open `_config.yml` and set the variables
- Run `jekyll serve` and your blog should be live on `http://localhost:4000`. Make changes, test them locally, commit your changes and push to your fork. Your changes should be live in a couple of seconds

### Screenshots

<div>
    <img src="https://github.com/abhn/Elementary/blob/master/tmp/desktop.png?raw=true">
    <p>Desktop Homepage</p>
    <h3/>
    <img src="https://github.com/abhn/Elementary/blob/master/tmp/desktop-post-top.png?raw=true">
    <p>Desktop Post Top</p>
    <h3/>    
    <img src="https://github.com/abhn/Elementary/blob/master/tmp/desktop-post-bottom.png?raw=true">
    <p>Desktop Post Bottom</p>
    <h3/>    
    <img src="https://github.com/abhn/Elementary/blob/master/tmp/mobile-360px.png?raw=true">
    <p>Mobile 360px Home</p>
    <h3/>    
    <img src="https://github.com/abhn/Elementary/blob/master/tmp/mobile-page-top.png?raw=true">
    <p>Mobile Page Top</p>
    <h3/>    
    <img src="https://github.com/abhn/Elementary/blob/master/tmp/mobile-post-footer.png?raw=true">    
    <p>Mobile Page Bottom</p>
    <h3/>    
</div>

### Customization
- `_/layouts/default.html` Default page with head and footer section
    - `_/layout/post.html` - Page for `layout: post`, inherits `default`
    - `_/layout/page.html` - Page for `layout: page`, inherits `default`

### Credits
- Eric S Raymond (http://www.catb.org/~esr/hacker-emblem/glider.png) for the favicon

### Inspiration
<p>
I recently read in a blog post that a personal blog has to be fast and lean. There's no reason for a personal blog to be bloated and take 2 seconds to load. That was when I reviewed my own blog code and started analyzing. I discovered that I was loading jQuery just for another jQuery plugin which just helped the images and videos to be mobile responsive. That was some 40KB of overhead, 2 additional requests which could have been prevented with just a `max-width: 100%` attribute to the culprit elements. Similarly, there was Disqus which loaded tonnes of scripts along with its own Google Analytics script. 
</p>
<p>
I went on stripping weight from the code, and was left with something what you see here. Few extra CSS tweaks and Tadaa!
</p>

### License
GNU GENERAL PUBLIC LICENSE Version 3