---
title: "build-100-websites.fun"
date: 2022-07-13T11:44:21+03:00
draft: false
---

Hi there. My name is Andrew and I am building 100 websites. Here are the websites I have built so far.

1. [how-to-host-one-html.page](#how-to-host-one-htmlpage)
   1. [Description](#description)
   2. [Tech stack](#tech-stack)
2. [andrew-quinn.me](#andrew-quinnme)
   1. [Description](#description-1)
   2. [Tech stack](#tech-stack-1)

## [how-to-host-one-html.page](https://how-to-host-one-html.page/)

### Description

The first website I ever made. A one-page document that provides an answer to the question, "I have a page of HTML, now how do I put it on the Internet?"

### Tech stack

- HTML.
- **Version control**: `git` + Github.
- **Hosting**: Netlify.

## [andrew-quinn.me](https://andrew-quinn.me/)

### Description

A semi-professional blog. I don't have a whole lot of content on it yet, mostly because I have no clue what I'm doing or where my career is headed. But I have confidence I'll figure it out in time.

### Tech stack

- Markdown.
- **Frontend**: None. Kind of.
- **Backend**: Again, none.
- **... End?**: Hugo? Honestly, static site generators kind of exist outside of the usual frontend/backend dialectic. I tried to explain it in layman's terms on Reddit here:
  <iframe id="reddit-embed" src="https://www.redditmedia.com/r/learnpython/comments/vrqt0a/can_you_make_websites_with_python/iey5cv9/?depth=1&amp;showmore=false&amp;embed=true&amp;showmedia=false" sandbox="allow-scripts allow-same-origin allow-popups" style="border: none;" scrolling="yes" width="100%" height="300rem"></iframe>

  [Brian Rinaldi](https://css-tricks.com/really-makes-static-site-generator/#aa-the-basics-of-a-static-site-generator) at CSS-Tricks lists the key ingredients of a static site generator, which he learned while building [HarpJS](https://harpjs.com/), as

  > - A **template language**(s) for creating page/post templates
  > - A lightweight **markup language** (typically Markdown) for authoring content
  > - A structure and markup (often YAML) for providing configuration and metadata (e.g. “front matter“)
  > - A set of rules or **structure for organizing and naming files** that are exported/compiled, files that are not and how these files will be handled (e.g. frequently prefacing a file or folder with an underscore means that it is not exported into the final site files or all posts go in a posts folder)
  > - A **means of compiling templates and markup into HTML** (frequently [but not always!] support for CSS or JavaScript preprocessors is also included)
  > - A **local server** for testing.

  Notice what's crucially missing from all that: There's no need to _recieve_ data from the user to one's own user, the traditional function of a backend. So I guess one way to describe static site generators like Hugo is that they're "all frontend".
  
  But this belies the true expressive power of static site generators like Hugo in a post-[Jamstack](https://jamstack.org/) age. With the preponderance of APIs out there already being run by servers big and small, it's entirely possible to avoid writing one's own backend entirely and just let users send whatever data you might need directly into _third party_ APIs - preserving the traditional separation of concerns that makes frontend/backend such an evergreen design decision -- "[separate policy from mechanism; separate interfaces from engines](http://www.catb.org/esr/writings/taoup/html/ch01s06.html#id2877777)" -- but removing the need to actually run and maintain your own backend server.
  
  Or at least, a backend that is actually coupled to the running of the website itself. You can definitely run a "backend" that just scrapes data out of all those third party APIs so you can analyze it from the comfort of your own laptop.
- **Version control**: `git` + Github.
- **Hosting**: Netlify, incidentally themselves the ones who coined the term [Jamstack](https://www.netlify.com/blog/authors/matt-biilmann/).