---
layout: post
title: "Ruby development environment quickstart guide"
date: 2018-04-25 12:00:00 +1100
categories: ruby development
---
Sandboxing ruby projects from external changes is imho the sensible choice.

This is true, of course, for any development environment. It's quite frustrating to come back to a project after some time and find it broken because it depended on a particular system configuration that just worked at the time.

One of the underlying remedies for ruby is to use a [ruby version manager](https://blog.metova.com/choosing-a-ruby-version-management-tool) like [rbenv](https://github.com/rbenv/rbenv). So on macOS the following will do the trick.

### Step 1. Install rbenv with ruby-build ###

    brew install rbenv

### Step 2. Initialise your shell with rbenv ###

I use [bash-it](https://github.com/Bash-it/bash-it), thus

    bash-it enable plugin rbenv

But, it is otherwise achieved via rbenv:

    # Run this and follow the instructions to set up rbenv integration with your shell
    rbenv init

### Step 3. Verify rbenv is setup ###

    # assume we've opened a new terminal
    curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash

### Step 4. Install recent ruby ###

Now install a ruby version via rbenv.

    # list the most recent stable version:
    rbenv install -l | grep -E '^\s*[0-9\.]+$' | tail -n 1

    # install that ruby version globally. e.g.,
    rbenv install 2.5.1
    rbenv global 2.5.1

### Step 5. Project initialisation ###

    # init project dir and cd into it
    mkdir my-new-project
    cd $_

    # init .ruby-version
    rbenv local 2.5.1

An alternative / complementary solution, I use [direnv](https://direnv.net). See [direnv's ruby wiki page](https://github.com/direnv/direnv/wiki/Ruby) for further tips.
