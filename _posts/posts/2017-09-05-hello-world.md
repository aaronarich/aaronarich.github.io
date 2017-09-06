---
title: Hello World
date: 2017-09-05 00:00:00 Z
categories:
- posts
author: Aaron A. Rich
layout: post
---

Welcome to the latest edition of my site, which just went live over Labor Day weekend! I've been hard at work gathering up projects to showcase, reiterating on layout design, and spending probably the most time deciding which platform/hosting I wanted to use. There's a lot of things to consider when building any website, but it always seems to be a bit more challenging to me when deciding on these things for my personal work.

In the interest of sharing knowledge and process, I want to use this post to give insight into the tools I used to create this website. Enjoy!

### Design

* **[Sketch](https://www.sketchapp.com/) -** hands down one of the best and most streamlined user interface design tools. While I don't coin myself as a product designer, I used Sketch's layout and grid tools to mock-up ideas as they came to mind. I also used their Sketch Cloud feature to share some of my early concepts with friends and get feedback.

* **[Abstract](https://www.goabstract.com/) -** this is a version control tool used in conjunction with Sketch. They launched their product just as I was beginning to learn Sketch, and I found it helpful for syncing my projects across my laptop and desktop. The branching feature was also great for wanting to create one-off explorations.

* **[SkyFonts](https://skyfonts.com/) -** when deciding on typography for my site, I found that it's a bit of a pain to download font-families to my local computer, import them, and then test them out in Sketch. SkyFonts addresses that problem directly by connecting the MacOS Font Book to Google Fonts, and a few other cloud-hosted font services. No more downloading, just pick the fonts you want to try out and they're synced.

### Development

* **[Jekyll](https://jekyllrb.com/) -** I decided to go with Jekyll because I'm familiar with static site generators from my past work. Jekyll is pretty lightweight for building static pages, but it also has a blogging aspect to it (which I hope to utilize frequently). Jekyll not only has an intuitive setup process, but it also integrates directly with several cloud-based CMSs as well as hosting providers... more about that below.

* **[Tachyons CSS Framework](http://tachyons.io/) -** it's so satisfying to design on a grid and have a nice rhythm between text and page elements. I've assembled my own grid layouts in the past, but for this site I wanted to use something more tested and robust. For that, I turned to Tachyons, developed in large part by [Adam Morse](https://github.com/mrmrs). There's also a SASS-specific fork of the project which I used in my Jekyll site. You can find that here on [Github](https://github.com/tachyons-css/tachyons-sass).

* **[Google Fonts, Roboto](https://fonts.google.com/specimen/Roboto) -** I decided to go with one of my favorite sans-serif font family seen on the web today, Roboto. This font was designed by [Christian Robertson](http://christianrobertson.com/) and is served through Google Fonts.

* **[Atom](https://atom.io/) -** I switched from Sublime Text to Atom a couple of years ago. For the most part, the text-editing aspect is largely the same (in my opinion), but the advantages that I've found from using Atom are largely the features and availability of packages built by the community. A few of the packages I use the most are the built in Git client, [Atom-Spotify](https://atom.io/packages/atom-spotify), and Markdown preview pane.

### Hosting & Deployment

* **[Surge](https://surge.sh/) -** early on in the development process, I used Surge as a quick and easy staging server. It's a free service hosted on Digital Ocean that provides quirky one-off URLs (like Heroku) or the ability to use custom domains for the sites you deply. I currently have my DNS pointing [dev.aaronarich.com](dev.aaronarich.com) to Surge for staging projects. The deployment and teardown process is super simple and everything is handled from the CLI.

* **[GitHub Pages](https://pages.github.com/) -** for production, I decided to host this site on GitHub Pages. Since Jekyll was developed at GitHub, Pages can automatically build and deploy my site as I make commits directly to the repository. This is a great solution since static sites have to rebuild each time you make changes. Another great feature of Pages is that they host sites on Fastly's CDN, which helps ensure faster page load times.

* **[Cloudflare](https://www.cloudflare.com/) -** on top of my site being hosted on Fastly's CDN, I've also implemented Cloudflare to sit in front of my site. Cloudflare provides numerous benefits including serving this site over HTTPS, serving it from their 117 global data centers, site cacheing to reduce origin server requests, and optimizing my site's HTML/CSS/JS to reduce page load.  Also, they provide these services as part of their free plan. Thanks to Nate Steiner for his [blog post](https://natesteiner.com/blog/free-static-hosting-with-https/) about setting this up 👍

* **[Siteleaf](https://www.siteleaf.com/) -** as I mentioned above in the Jekyll section, there are a few cloud-based content management systems available for Jekyll. The one I've chosen to go with is Siteleaf. They provide a CMS in the cloud so that my site can be edited from anywhere, not just from my text editor. When you set up a site in Siteleaf, it connects to and syncs with a GitHub repository automatically. This allows me to make changes or write new posts there, and then have them sync as commits to GitHub. Once the commit syncs, GitHub Pages detects the change and automatically rebuilds the site and deploys it.

That pretty much covers it for Version 1.0 now that it's up and running. My goal from here is to keep updating this site with new posts, projects, insights, and even the design itself. I might even add a signup form for getting updates as they roll out, who knows! If you have any questions about anything I mentioned here, feel free to tweet/message me [@aaronarich](https://twitter.com/aaronarich). Thanks for taking the time to read this!
