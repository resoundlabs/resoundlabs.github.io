---
layout: post
title: Maschine - creating custom graphics for plugins and sound libraries
date: 2015-5-27
---

![image](https://cloud.githubusercontent.com/assets/12622205/7867376/b853ba3c-0543-11e5-8da0-5f74aa944266.png)

By default, 3rd party plugins all share a boring graphic that doesn't provide any visual cue to tell them apart. But, that can be changed!

<!--more-->

Here are the steps at a high level
1. load up a plugin and right-click to Save As and save it to the User Library
2. when browsing, it will now show up in User Library sorted by developer (with boring graphic)
3. create a directory with the developers name in `/`
4. this will be the contents of the directory (the easiest way to begin is to copy the contents from one of the existing directories - or use this template) ![image](https://cloud.githubusercontent.com/assets/12622205/7874330/1b59f51e-057c-11e5-8eb5-bf75f78db1ab.png)
5. replace the contents of each file with new custom graphics
6. start (or restart) Maschine

### Last points
Extra special bonus points from us all if someone can figure out how to do this for groups. This only applies to plugins and samples at this point. Custom groups saved in the User area all share the same Maschine top level image.
This tutorial only covers Mac. If someone will doublecheck the specific paths for Windows and post details in the comments below, I will update the article.
### Example
![image](https://cloud.githubusercontent.com/assets/12622205/7833384/645af84c-0434-11e5-87d2-05b5fe292cf9.png)
