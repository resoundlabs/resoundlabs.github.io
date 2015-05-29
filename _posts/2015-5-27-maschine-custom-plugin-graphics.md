---
layout: post
title: Custom graphics for plugins and sound libraries
tags: machine
---

![image](https://cloud.githubusercontent.com/assets/12622205/7875201/e52c1858-0587-11e5-802b-960ef8b17cf6.png)

By default, 3rd party plugins all share a boring graphic that doesn't provide any visual cue to tell them apart. But, that can be changed!

<!--more-->

## High level steps

1. Load up 3rd party plugin, right-click and "Save As" to the User Library
2. Now, when browsing, it will now show up in User Library sorted by developer (with boring graphic)
3. Create a directory with the developer's name (as it shows up in Browser) in `/Users/Shared/NI Resources/image` [e.g. `/Users/Shared/NI Resources/image/Camel Audio`]
4. Copy the contents of another directory in `/image` to use as a template (or use this template)
6. Change the prefix of the file ending in `.meta` to match the directory name [e.g. `Camel Audio.meta`]. Now the contents of the directory should look like this ![image](https://cloud.githubusercontent.com/assets/12622205/7874330/1b59f51e-057c-11e5-8eb5-bf75f78db1ab.png)
5. Replace the contents of each `.png` file with new custom graphics
6. Start (or restart) Maschine

### Ok, dive into the details

* `MST_artwork.png` big picture on the right screen
* `MST_logo.png` logo on the left screen
* `MST_plugin.png` works only with NI plugs - editing will have no effect
* `OSO_logo.png` no idea
* `VB_artwork.png` text on the right side of software
* `VB_logo.png` logo on the left side of software
* `prism.meta` only requirement is correct name (appears to ignore `setting insde`)

### Specifics on creating the graphics

The graphics need to be `.png` files of specific sizes. There are tons of ways to accomplish this. Personally, I open each "template" png file in Photoshop, paste in a screen capture (creating a new top layer). Then select, resize, add text, clip, etc as needed. When it looks good, flatten the layers and save... done.

### Last points
I have doublechecked and capitalization is not important. `Camel Audio` and `camel audio` both work. Spacing is important - `CamelAudio` will not work.
**Extra special bonus points** from us all if someone can figure out how to do this for groups. This only applies to plugins and samples at this point. Custom groups saved in the User area all share the same Maschine top level image.
This tutorial only covers Mac. If someone will doublecheck the specific paths for Windows and post details in the comments below, I will update the article.
### Example
![image](https://cloud.githubusercontent.com/assets/12622205/7833384/645af84c-0434-11e5-87d2-05b5fe292cf9.png)
