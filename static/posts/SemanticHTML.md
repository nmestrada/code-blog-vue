---
title: Semantic HTML
---
## What is Semantic HTML?
Semantic HTML is not something I was taught in coding bootcamp, I learned the basics of HTML. Mostly that a webpage is comprised of a <header>, <body>, <footer> and a bunch of div's right? Well, that's not the whole picture. See HTML5 introduced other tags that can be used to create a better picture of what we see in our html files. There are <section>, <article>, <aside>, <nav> among many other tags to help describe our html. 

A lot of times as a beginner dev, and I'm still learning, I would create what we know as a *div soup*. Div soup is when you add divs into your html without consideration for what they could be. Maybe you have div with a class ".nav" but that could be better written as nav instead. Things like that. 

## Why Semantic HTML?
From a general sense of my research using semantic HTML is very useful. 
1. Accessibillity: Users that use a screen reader will have a better time on your page 
2. SEO: Web crawlers for search engines like Google will better parse your page
3. Readability: let's not create a div soup and organize your html better. Clean code is always fun isn't it!

## Semantic HTML with React
# JSX
Well, I use React and how does this fit into my projects? For one thing React uses JSX. Which is a mixture of XML and HTML. Fun right? Yeah! Instead of wrapping components in a div, use React Fragments to wrap your components if they are a plain div with no attributes. 
# refs

