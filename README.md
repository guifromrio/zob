# Zero Overhead Blog

A really minimal static blog generator that's about the content and the performance. 

### Why

I want to remove all excuses to having a blog. So I built the simplest blog generator I could. Also, I want to code some deno.

### ~JS~ everything fatigue

I hate file bloat in my repo. I get tired just from thinking of dealing with layers of React and Gatsby and `node_modules`. I just want to convert some markdown into simple, performant static page that focuses brutally on the content - both for myself and for users. 

### The accumulated layers of abstraction hinders first steps

Try explaining to a friend who's curious about programming how your frontend setup works. They probably won't listen long enough to get to the `package.json`, and by `webpack` you've lost them. 
When I was a kid, programming had much a more immediate positive feedback loop. I changed local HTML, reloaded the browser and saw the effects. I got hooked into it - that made me explore further. This is crucial for having more people join the field - making inclusive tools for beginners (and minimalists). I want to build tools that bring me back to that feeling of mesmerizing, iterative evolution. "First, do it". Doing the first thing, taking the first step must be simple. 

### zob is free forever

You are welcome to fork it and do whatever you want. 

# How to zob

```sh
$ deno install --allow-write --allow-read --name zob https://github.com/firstdoit/zob/cli.ts
```

Then, anywhere with a `posts` folder which contains `.md` files with frontmatter like:

```md
---
title: Hello, world!
date: '2021-06-12'
---

Hello, world!
```

Run the `build` command:

```sh
$ zob build
```

This generates a `public/` folder with some HTML and CSS files inside.

Publish those anywhere. I use Vercel.

Enjoy!

# Live Preview

While editing posts, you may take a look at the result with the `live` command:

```sh
$ zob live
```

And going to `http://localhost:8080`. Changes to posts are recompiled immediately. 

# Make it yours

Add an `author.md` with your description.