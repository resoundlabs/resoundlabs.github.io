---
layout: post
title: Managing Plugins
---

# Getting organized

Plugins can seem mystical - they just show up in your various apps, some as VST, some as AU and in Pro Tools, you have AAX. They become less mystical when you track down the location of the plugins in the file system. Here are the paths.

* VST `/Library/blah`
* Audio Unit `/Library/blah`
* AAC `/blah`

To really take control of your plugins, you will want to get your hands dirty. I created a "shortcut" directory with symbolic links to each directory above. Accessing these directories allows you to do many things.

<!--more-->

* For troubleshooting, look and see if a plugin is on your system. If it isn't showing up in your app and you think it should be, double-check and see if its in the directory. There can be slight variations in name, but in general, its easy to figure out what is what. An example of this... in the directory the manufacturers name might be prepended to the plugin name, while it might not display that way in an app.
* Remove plugins that you don't want to show up in your apps. For example, I removed the AU versions of plugins that I have a VST for as well (I use VST when I can - and no reason to clutter the list with AU plugs I won't ever use). 

### Waves

Waves plugins are different. Waves places a single plugin in each of these directories, the "waveshell," which references an external directory with all of the Waves plugins. 

### Universal Audio

UA is a PITA. The UA installation puts every single UA plugin in the directories (both VST and AU) even if you don't have a license. I promise if you don't remove the ones you don't have, you will continually select one and be prompted with a license dialog - very frustrating (and there are a bazillion, so they just clutter up the plugin drop downs). For VST, UA sticks all of their plugs in a subdirectory (further, all of the mono plugs are in yet another subdirectory). For AU, the plugs are all listed individually. 

### Misc additional notes

