---
layout: post
title: "Personal Blog with Github Pages and Jekyll themes Pt2."
date: 2018-04-25 14:05:00 +1100
categories: jekyll github general markdown
---
In [Part 1]({% post_url 2018-04-14-blogging-with-jekyll-pt1 %}) I said that blogging with [GitHub Pages](https://pages.github.com) and [Jekyll](https://jekyllrb.com/) is a popular choice but it could be much simpler.

[GitHub Pages](https://pages.github.com) instructions, disappointingly, left us with an `index.html` file simply containing the text `Hello, World`. As an advanced option that would be great, but but I'd hoped for a markdown-based blog site out of the box.

## Jekyll's Prerequisites ##

As it turns out Jekyll's [Quickstart Guide](https://jekyllrb.com/docs/quickstart/) assumes you have a ruby development environment already.

See my [Ruby development environment quickstart guide]({% post_url 2018-04-25-ruby-development-environment-quickstart %}) to fulfil that requirement for macOS.

Jekyll's [installation](https://jekyllrb.com/docs/installation/) documentation is otherwise helpful for various platforms.

## Installing Jekyll ##

As Jekyll's [installation](https://jekyllrb.com/docs/installation/) documentation suggests we install both `bundler` to manage plugins and themes along with jekyll itself.

    gem install bundler jekyll

In part 3, we'll use look at theming jekyll.

You can also now refer again to Jekyll's [quickstart guide](https://jekyllrb.com/docs/quickstart/), it's basic [usage](https://jekyllrb.com/docs/usage/) and various [docs](https://jekyllrb.com/docs/home/).
