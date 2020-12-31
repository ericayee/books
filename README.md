# Highlights

![Screenshot of the website](assets/images/screenshot.png?raw=true)

A site for my book recommendatiosn and highlights: [ericayee.com/highlights](https://ericayee.com/highlights/), built with Eleventy. Highlights and covers are copyright to their respective authors. Forked from [highlights.melanie-richards.com](highlights.melanie-richards.com).

## To build

1. [Install Node/npm](https://nodejs.org/)
2. Run `npm install`
3. Run `npx @11ty/eleventy --serve`
4. Visit `localhost:8080`

## To deploy to GitHub pages
1. Make sure you have a branch called ```gh-pages```
2. Go into the GitHub settings and enable Github Pages to build from ```gh-pages``` and ```/root``` 

## Commands

| Command                     | Purpose                                |
| ----------------------------| -------------------------------------- |
| npx @11ty/eleventy --serve  | Serve project                          |
| npx gulp sass:watch         | Watch and build sass files locally     |
| npx gulp minify-css         | Compress output CSS file before deploy |
| npx run deploy              | Deploy to GitHub Pages                 |

## Data syntax

### Book front-page matter

```
title: "Book Title"
book: dash-separated
author: first last
kindle: true
date: YYYY-MM-DD
pub: 2020
tags: posts
genres: contemporary romance
review: what I liked about this book
goodreads: https://www.goodreads.com/...
bookshop: https://bookshop.org/...
```

Where "dash-separated" is also the file name for the `_data` file and JPG (cover image).

### Each highlight

```
- text: 
  page: 
  attribution: 
```