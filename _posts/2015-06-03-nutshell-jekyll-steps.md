---
layout: post
title: nutshell jekyll steps
categories: []
tags: [jekyll]
published: True

---

### In a nutshell

Using swankyp as github user for examples below...

* Log in to github account where you want new blog
* Fork https://github.com/barryclark/jekyll-now (not https://github.com/barryclark/jekyllnow - that one messed me up for a bit)
* Rename to `swankyp.github.io`
* Note: if committing to more than a single github account, setup ssh config to use appropriate github creds for a given repo. For example, for github account `swankyp` with an email of `swankyp@gmail.com` the settings would be...
  - settings in `~/.ssh/config`

```
Host github.com-swankyp
HostName github.com
User git
PreferredAuthentications publickey
IdentityFile ~/.ssh/swankyp_github
```

  - settings in `thenewrepo/.git/config`. These latter changes can all be done with the git command directly.
    + `git remote set-url origin git@github.com-swankyp:swankyp/swankyp.github.io.git`
    + `git config user.name "swankyp"`
    + `git config user.email "swankyp@gmail.com"`
* upload public key to github account
*


