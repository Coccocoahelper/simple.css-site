---
title: Getting Started | Simple.css {}
header: Getting Started
description: Instructions on how to get started with Simple.css.
permalink: /getting-started
layout: default
---

Ok, so you're starting a new project (or have an existing project), and you want to use Simple.css to theme your site. It's very simple to do and you should be able to set something up that looks like this site in just a few minutes.

There are a number of ways in which you can use Simple.css:

1. Add the minified, CDN hosted version of Simple.css, so you always get the latest updates.  
    1.1 Use NPM's CDN, UNPKG.
2. Install from NPM.
3. Host Simple.css yourself.

## Option 1 - the CDN hosted version

Whenever I push an update to the [Simple.css GitHub repository](https://github.com/kevquirk/simple.css), GitHub automatically minifies the CSS and publishes it to the CDN.

So all you need to do in order to use Simple.css in your project, is add the following line of code to the `<head>` section of your HTML:

```
<link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css">
```

Now, whenever I publish an update to Simple.css, you will automatically receive it.

### Option 1.1 - UNPKG.com (CDN for npm)

Simple.css is also published to [**npm**](https://www.npmjs.com/). Both minified and un-minified versions of the CSS are available NPM's CDN, [**unpkg**](https://unpkg.com/).

So all you need to do in order to use Simple.css in your project, is add the following line of code to the `<head>` section of your HTML:

```
<!-- Minified version -->
<link rel="stylesheet" href="https://unpkg.com/simpledotcss/simple.min.css">

<!-- Un-minified version -->
<link rel="stylesheet" href="https://unpkg.com/simpledotcss/simple.css">
```

## Option 2 - Install from NPM

[NPM](https://www.npmjs.com/) is a package registry installing JavaScript and other frontend packages, for NodeJS and browsers.  If you're using any sort of build process (webpack, gulp, browserify,etc), you can manage simple.css as dependency in your project's `package.json`.

To install with NPM or Yarn

```
$ npm install simpledotcss

# or

$ yarn add simpledotcss
```

For example, using a bundler like **webpack**, you can consume _simple.css_ using an `@import` statement in a CSS file

```
@import url('~simpledotcss/simple.min.css');
```


## Option 3 - self-host Simple.css

Of course, you don't have to use the CDN delivery method. If you prefer, you can host Simple.css yourself; but you won't automatically receive updates to the CSS as it is released. You would need to re-download the source and update your project yourself.

[Download the source files from here](https://github.com/kevquirk/simple.css).

## Adding Simple.css to your project

Here's a simple quick start guide on how to add the CDN hosted version of Simple.css to your project.

### Step 1 - create a HTML file

The first thing you're going to need is a HTML file so you have something to actually format with Simple.css. Fire up your favourite text editor (my favourite is [Atom](https://atom.io)) and paste this basic HTML into it:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My New Website</title>
</head>
<body>
  <header>
    <h1>Hello, world</h1>
    <p>Welcome to my website!</p>
  </header>

  <main>
    <p>This is my new website and it's using Simple.css. It's really cool. If you want to use it too, you can <a href="https://simplecss.org">visit their site</a>.</p>
  </main>

  <footer>
    <p>Jane Smith's website.</p>
  </footer>
</body>
</html>
```

Save this file on your computer somewhere as `index.html`. If you then double-click on that file, it will open in your browser and should look something like this:

![Unformatted HTML example](/assets/images/unformatted-html.png)

Not very nice, I think you will agree. Let's add Simple.css and fix this, shall we?

### Step 2 - add Simple.css

All you need to do to add all the loveliness of Simple.css to your fantastic new site, is add the following line of code to the `<head>` section of your HTML:

```
<link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css">
```
Refresh your browser window and ta da! You now have Simple.css formatting on your site. 🎉

![Simple.css formatted HTML example](/assets/images/simple-css-formatted-html.png)

**That's it. You're done.**

You now have Simple.css formatting your site. All you need to do now is edit the `<header>` and `<footer>` sections to suit your needs. Any content within the main page needs to be added inside the `<main>` tags.

The best part is that because you're using our CDN, whenever we publish updates to the project, you get them automagically!

How easy was that! If you want to learn more about adding more styles elements and what's available with Simple.css, take a look at the [demo page](/demo).
