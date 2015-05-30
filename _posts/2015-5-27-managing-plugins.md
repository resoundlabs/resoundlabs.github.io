---
layout: post
title: Managing Plugins
---

## Getting organized

Plugins can seem mystical - they just show up in your various apps, some as VST, some as AU and in Pro Tools, you have AAX. In the end, they are just files that can be moved, deleted and managed. Here are the paths.

* VST `/Library/Audio/Plug-Ins/VST`
* VST3 `/Library/Audio/Plug-Ins/VST3`
* Audio Unit `/Library/Audio/Plug-Ins/Components`
* AAX `/Library/Application Support/Avid/Audio/Plug-Ins`

To really take control of your plugins, you will want to get your hands dirty. Create a "shortcut" directory with symbolic links for quick access.

<!--more-->

* Troubleshooting. Check and see if a plugin is on your system. If it isn't showing up in your app and you think it should be, double-check and see if its in the directory. There can be slight variations in name, but in general, its easy to figure out what is what. An example of this... in the directory the manufacturers name might be prepended to the plugin name, while it might not display that way in an app.
* Organization. Remove plugins that you don't want to show up in your apps. For example, I removed the AU versions of plugins that I have a VST for as well (I use VST when I can - and no reason to clutter the list with AU plugs I won't ever use).

### Waves

Waves plugins are different. Waves places a single plugin in each of these directories, the "waveshell," which references an external directory with all of the Waves plugins. The individual plugins are located in `/Applications/Waves/Plug-Ins V9`.

### Universal Audio

UA plugs are a PITA. The UA installation loads every single UA plugin (both VST and AU), even if you don't have a license. I promise if you don't remove the ones you don't have, you will continually select one and be prompted with a license dialog - very frustrating (and there are a bazillion, so they just clutter up the plugin drop downs). For VST, UA sticks all of their plugs in a subdirectory (further, all of the mono plugs are in yet another subdirectory). For AU, the plugs are all listed individually.

### Misc additional notes
http://www.native-instruments.com/forum/threads/share-your-plugins-for-maschine-2-0-browser-heres-mine.210958/

