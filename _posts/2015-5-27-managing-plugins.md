---
layout: post
title: Managing Plugins
tags: [audio]
---

[insert a graphic here - maybe of a folder with shortcuts to the actual directories]

## Getting organized

Plugins can seem mystical - they just show up in your various apps, some as VST, some as AU (mac) or AAX (Pro Tools). In the end, they are just files that can be moved, deleted and managed. Here are the paths (mac specific) and file extensions for each type.

* VST `/Library/Audio/Plug-Ins/VST`, extension `.vst`
* VST3 `/Library/Audio/Plug-Ins/VST3, extension `.vst3`
* Audio Unit `/Library/Audio/Plug-Ins/Components`, extension `.component`
* AAX `/Library/Application Support/Avid/Audio/Plug-Ins`, extension `.aax`

To really take control of your plugins, you will want to get your hands dirty. Create a "shortcut" directory with symbolic links for quick access (you can use this zipped folder).

<!--more-->
## Things to do

* Pruning Extras. Remove plugins that you don't want to show up in your apps. For example, I removed the AU versions of plugins which also have a VST version (I use VST when I can - and no reason to clutter selection lists with duplicate AU plugins). Rather then deleting them, I moved them to a backup folder.
* Removing non-authorized plugins.
* Troubleshooting. If a plugin isn't showing up in an application (but you successfully ran the isntaller), search to ensure the plugin is actually in the corresponding folder. There can be slight variations in name, but in general, the naming is self explanatory. If it isn't there, that points to a problem with the installation. If it is there, that points to a problem with the plugin (or the host app).


### Last Points

* For VST/VST3, some developers create a subdirectory (e.g. `/Library/Audio/Plug-Ins/VST/Softube`) for their plugins.
* Waves plugins are different. Waves places a single "waveshell" (e.g. `WaveShell-VST 9.3.vst`) plugin in each of these directories. The waveshell accesses an external directory with all of the Waves plugins. The individual plugins are located in `/Applications/Waves/Plug-Ins V9`. To remove a Waves plugin, remove it from this directory.
* Universal Audio plugins are a PITA. The UA installer loads every single UA plugin (both VST and AU), even if you don't have a license. I promise if you don't remove the ones that are not authorized, you will continually select them and be prompted with a license dialog - very frustrating (and there are a bazillion, so they just clutter up the plugin drop downs). For VST, UA sticks all of their plugs in the `Powered Plug-Ins` subdirectory (the mono plugs are another subdirectory down `Powered Plug-Ins/mono`). For AU, the plugs are all listed individually.
*

### More Tips?

This is only a scratch on the surface. I will update this post with any additional tips that you'all post in the discussion below.



