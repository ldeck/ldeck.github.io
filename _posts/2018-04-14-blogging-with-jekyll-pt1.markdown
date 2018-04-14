---
layout: post
title: "Personal Blog with Github Pages and Jekyll themes Pt1."
date: 2018-04-14 11:20:00 +1100
categories: jekyll github general markdown
---
Getting started with [GitHub Pages](https://pages.github.com) is fairly straightforward if all you want is plain text on a white canvas.

To setup a markdown based blog, however, jekyll is a popular option.

## The Good.

Jekyll has promise.

Why give Jekyll a go? My thinking was...

1. It's suggested by GitHub.
1. It has lots of community contributed themes.
1. Both of these should save me time.

The end result is that it's simple to create blog posts: create a **`YYYY-MM-DD-name-of-post.markdown`** file in your `_posts` directory, commit and push.

    ---
    layout: post
    title:  "Welcome to Jekyll!"
    date:   2018-04-14 11:10:16 +1100
    categories: jekyll update
    ---
    Create this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `bundle exec jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

    To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

## The Bad.

The Jekyll docs are verbose from the start.

Too much reading is given to fine-grained options, reading more like man pages, with all the options up front and any examples, if any, buried at the end.

The [Quick Start Guide](https://jekyllrb.com/docs/quickstart/), ironically not linked to from Jekyll's homepage, ends with a section called **Next Steps**:

> Building a Jekyll site with the default theme is just the first step.
> The real magic happens when you start creating blog posts,
> using the front matter to control templates and layouts,
> and taking advantage of all the awesome configuration options Jekyll makes available.

This is exactly what we want to do, but there's no link to the relevant instructions for doing this; the next button takes you instead to `Installation`, which presumably you've already done if you managed to get through the *Quick Start Guide*, right?

## Let's Fix That.

Providing a step-by-step guide beyond generating "Hello, World!" would have been easy. It could go something like this:

Perform the initial steps provided by [GitHub Pages](https://pages.github.com). i.e.,

1. Create a repository called *yourusername*`.github.io` [here](https://github.com/new).
1. Clone your new repository to a local directory as [GitHub describes](https://help.github.com/articles/cloning-a-repository/).
1. Generate a Jekyll blog site (see part 2).
1. Generate and write a blog post (see part 2).
1. Commit and push.

    ```bash
    $ git add --all
    $ git commit -m "My initial blog site"
    $ git push -u origin master
    ```
1. View your handy work at https://*yourusername*.github.io.

Well, stay tuned for part 2 for producing a blog site.
