# Elementary Jekyll Theme 1.0
When I started with the [original project](https://github.com/abhn/Elementary/releases/tag/v0.1) around 2 years ago, my goal was to get rid of all that unnecessary code and progressively add only the most essential bits. 

I feel like the theme is in good enough shape right now that I can call it a v1.0

### Demo
<a href="https://elementary-jekyll.github.io/">https://elementary-jekyll.github.io/</a>

### Features
- Lightweight, <10KB CSS, <3KB (optional) JavaScript + 15KB Open Sans font file + your content
- Highly accessible with semantic HTML
- Structured data ([schema.org](https://schema.org)) pre-added for blog posts
- Dark mode (requires JavaScript for toggling class and saving user preference in cookies)
- Reading progress slider on top (requires JavaScript)
- JavaScript is optional (turn it off in `_config.yml`)
- No request made to any third party
- Any many more...

### Installation
📝 todo

### Customization
📝 todo

### Screenshots
📝 todo

### Performance
📝 todo

### Credits
- Eric S Raymond (http://www.catb.org/~esr/hacker-emblem/glider.png) for the favicon

### Inspiration

I recently read in a blog post that a personal blog has to be fast and lean. There's no reason for a personal blog to be bloated and take 2 seconds to load. That was when I reviewed my own blog code and started analyzing. I discovered that I was loading jQuery just for another jQuery plugin which just helped the images and videos to be mobile responsive. That was some 40KB of overhead, 2 additional requests which could have been prevented with just a `max-width: 100%` attribute to the culprit elements. Similarly, there was Disqus which loaded tonnes of scripts along with its own Google Analytics script. 

I went on stripping weight from the code, and was left with something what you see here. Few extra CSS tweaks and Tadaa!

### License
GNU GENERAL PUBLIC LICENSE Version 3
