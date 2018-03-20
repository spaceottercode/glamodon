# Glam
[Userscript](https://en.wikipedia.org/wiki/Userscript) that adds a new button to your compose box on Mastodon websites<sup>1</sup>. With this new button you can apply filters & stickers to your images and tweak them.

This scripts runs on Firefox with GreaseMonkey or Chrome (natively as an extension).

> 1. This User Script by default, runs on the following sites:
>
>   * mastodon.social
>   * mastodon.art
>   * mstdn.io
> 
>   Add your Mastodon site by adding a new @install line at the top of the script or replacing an existing one


# Install

### Firefox

To run userscripts on Firefox based browsers you will need [Greasemonkey extension](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) plugin. 

Next **[Click here](https://raw.githubusercontent.com/spaceottercode/glamodon/master/glamodon.user.js)** to automatically install the script.

If GreaseMonkey does not detect the userscript, create a `New user script...` in GreaseMonkey, and replace it with the contents of [glamodon.users.js](https://raw.githubusercontent.com/spaceottercode/glamodon/master/glamodon.user.js).

### Chrome

On Chrome, no plugin is needed to run a userscript like this one. Drag the script unto your browser's extension window to install. See Chromes documentation for instructions on accessing the extension window/page.

# Features

* filters
* layer png images ontop of your images<sup>2</sup>
* adjust brightness, contrast, gamma, exposure, and saturation
* rotate and flip your images<sup>3</sup>

Upcoming

* crop
* text
* blur

> 2. Your pngs must be packed into a tar file. tar file must not be compressed. An example is included above: `stickers.tar`. To create a tar file on POSIX operating systems run: `tar cvf fileout.tar image01.png image02.png` ...

> 3. At the moment flips cannot be combined with other flips or rotates.

# TODO/WIP

### filters

- [ ] the ability to add and remove filters
- [ ] the ability to reorder filters
- [ ] document how to make custom filters
- [ ] a filter to add borders/frames
- [ ] vignette

### tools

i.e. utilities. This is where you'll find things like the focal point tool and other tools like rotate (90º)

- [ ] channels
- [ ] colorize
- [ ] blurs
- [ ] text

### misc

- [ ] render to sizes > 640x640
- [ ] as the script reaches maturation, change toot button to a done/ button, processed image is integrated back
into compose text box as usual retaining traditional workflow

# Version

### 0.1

apply one of ~10 filters to a pic and upload. Privacy and text can be set in the main UI (compose message box). Spoiler text has limited support. In this release the processed image can be upto 640x640 but this will be lifted in future releases.

### 0.2

Support for stickers/decals added. To use stickers you will need to create a sticker pack. `stickers.tar` above is an example. A sticker pack is nothing more than a tar file with one or more png file. png files can be any size up to 255x255. They don't all have to be the same size. pngs may use transparent backgrounds. At the moment up to 32 pngs can be included. I might raise it later.

> Do not compress your tar file. tar.gz, tar.bz, etc, files are not supported. Only plain .tar files.

For linux and mac users, you can run the `tar` command in a terminal by navigating to the folder with pngs and running,

~~~
tar cvf tarfile_name.tar *.png 
~~~

That's pretty much it. You can import your stickers with the Add Sticker button.

### 0.3

stickers can now be scaled.

### 0.5

now includes tools for adjusting the brightness & contrast, exposure, gamma, hue & saturation, and the vibrance of an image.

### 0.6

non-compounded rotate and flips added. Focal point tool added. throbber added.
