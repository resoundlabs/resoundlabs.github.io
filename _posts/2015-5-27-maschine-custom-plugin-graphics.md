---
layout: post
title: Maschine - custom graphics for plugins and sound libraries
tags: [machine, audio]
---

![image](https://cloud.githubusercontent.com/assets/12622205/7875201/e52c1858-0587-11e5-802b-960ef8b17cf6.png)

By default, 3rd party plugins all share a boring graphic that does not provide any visual cue to tell them apart. But, that can be changed!

## High level steps

1. In the Maschine software, load up a 3rd party plugin, right-click and "Save As" to the User Library ([more on this](maschine-a-better-way-to-browse)). This applies to both Instruments and Effects.
2. Now, when browsing ![image](https://cloud.githubusercontent.com/assets/12622205/7878108/57e5ceba-05b1-11e5-82f1-afe27d9e9688.png) the User section, the plugin will show up, as well as the developer (with boring graphic)
3. Create a directory with the developer's name (exactly as it is displayed in Browse) in `/Users/Shared/NI Resources/image` <br>[e.g. `/Users/Shared/NI Resources/image/Camel Audio`]
4. Copy the contents of another directory in `/image` to the new directory to use as a template (or use this [template](/files/template.zip))
6. Change the prefix of the file ending in `.meta` to match the directory name [e.g. `Camel Audio.meta`]. The contents of the directory should resemble this (again with Camel Audio as an example developer) <br>![image](https://cloud.githubusercontent.com/assets/12622205/7874330/1b59f51e-057c-11e5-8eb5-bf75f78db1ab.png)
5. Replace the contents of each `.png` file with new custom graphics
6. Start (or restart) Maschine

<!--more-->

### Ok, the details for the specific files

* `plugin_name.meta` file name needs to match developer name exactly - see example above (it is not necessary to edit the contents)
* `MST_artwork.png` graphic on Studio's right screen
* `MST_logo.png` graphic on Studio's left screen
* `VB_logo.png` graphic on the left side of Browser section in software
* `VB_artwork.png` graphic on right side of Broswer section in software
* `MST_plugin.png` works only with NI plugs (editing will have no effect)
* `OSO_logo.png` no idea what this is for

### Specifics on creating the graphics

The graphics need to be `.png` files of specific sizes. There are tons of ways to accomplish this. Personally, I open each "template" png file in Photoshop, paste in a screen capture (creating a new top layer). Then select, resize, add text, clip, etc as needed. When it looks good, flatten the layers and save... done.

### Last points

* I have doublechecked and capitalization is not important for either the directory or the `.mst` file. `Camel Audio` and `camel audio` both work. Spacing **is** important - `CamelAudio` will not work.
* Special characters in the developer's name will screw things up. For example, `audio.de` or `Universal Audio, ` will not work. The developer name is derived from the plugin, so no way to change it.
* This tutorial only covers Mac. If someone will doublecheck the specific paths for Windows and post details in the comments below, I will update the article.
* It is possible to change the background color of the images on the controller and in the softare. Here is an example...
* How to change the color in `color.db` - that's another [tutorial](/maschine-plugin-color-backgrounds)
* A creative tip - if you set the background image of `MST_artwork.png` with the background color defined in `color.db`, the image looks like it has a transparent background.
* You can change the graphics for Maschine's own logo as well
* Note: there is a single pixel black line between the right side of `MST_logo.png` and the list of plugins. The lighter the colors in your graphic, the more it will show up.
* This same technique can be applied to User sample libraries
* **Extra special bonus points** from us all if someone can figure out how to do this for User groups! This only applies to plugins and samples at this point. Custom groups saved in the User area all share the same Maschine top level image.

### Links
I did not come up with this - I figured it out from other postings (don't remember which one specifically to give credit). Here are a handful

* [Maschine Masters - youtube](https://www.youtube.com/watch?v=2S0lLtAWho8)
* [Maschine Masters - youtube (covers Windows)](https://www.youtube.com/watch?v=gIS2sJ_Rsy8)
* [VIP Sound Labs - youtube](https://www.youtube.com/watch?v=gsrV3cC9XpY)
* [NI Maschine Forum thread](https://www.native-instruments.com/forum/threads/tutorial-how-to-create-custom-images-for-kits-in-maschine-studio-and-2-0-software.210960/)
