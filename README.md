# Glam
User-Script that adds image filters, stickers, and image tweaking tools on Mastodon sites<sup>1</sup>

> 1. Stickers and tools will be made available soon.

Runs on Firefox running GreaseMonkey and Chrome (running natively as an extension).

# Install

To run User-Scripts on Firefox based browsers you will need [Greasemonkey extension](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) installed and running. 

Next **[Click here](https://raw.githubusercontent.com/spaceottercode/glamodon/master/glamodon.user.js)** to automatically install the script.

If GreaseMonkey does not detect the User-Script, create a New User Script in GreaseMonkey, and replace the script's text with the contents of [glamodon.users.js](https://raw.githubusercontent.com/spaceottercode/glamodon/master/glamodon.user.js).

On Chrome, no plugin is needed to run a User-Script like this one. Drag the script unto your browser's extension window to install. 


> This User Script by default, runs on the following sites:
>
>   * mastodon.social
>   * mastodon.art
>   * mstdn.io
> 
>   Add your Mastodon site by adding a new @install line at the top of the script or replacing an existing one


# TODO/WIP

### filters

- [ ] the ability to scroll filters left and right
- [ ] the ability to add and remove filters
- [ ] the ability to reorder filters
- [ ] document how to make custom filters
- [ ] the ability to add frame borders

### stickers

- [x] adding stickers is a high priority. ideally should be extensible and distributable. 
  Simplest way atm is to allow any png (of limited size) to be imported as a sticker
- [ ] ability to scale stickers
- [ ] ability to rotate stickers (might be dificult+expensive with a 2D canvas)
- [ ] Of lesser priority but nice to have: animated stickers

### tools

i.e. utilities. This is where you'll find things like the focal point tool and other tools like rotate (90º)

- [ ] focal point
- [ ] rotate CW, CCW, flip
- [ ] brightness & contrast
- [ ] saturation
- [ ] curves, exposure, gamma
- [ ] color tweaks
- [ ] blurs
- [ ] text

### misc

- [ ] render to sizes > 640x640
- [ ] add vertical scroll
- [ ] as the script reaches maturation, change toot button to a done/ button, processed image is integrated back
into compose text box as usual retaining traditional workflow

# Version

### 0.1

apply one of ~10 filters to a pic and upload. Privacy and text can be set in the main UI (compose message box). Spoiler text has limited support. In this release the processed image can be upto 640x640 but this will be lifted in future releases.

### 0.2

Support for stickers/decals added. To use stickers you will need to create a sticker pack (I will be uploading one soon). A sticker pack is nothing more than a tar file with one or more png file. png files can be any size up to 255x255. They don't all have to be the same size. pngs may use transparent backgrounds. At the moment up to 32 pngs can be included. I might raise it later.

> Do not compress your tar file. tar.gz, tar.bz, etc, files are not supported. Only plain .tar files.

For linux and mac users, you can run the `tar` command in a terminal by navigating to the folder with pngs and running,

~~~
tar cvf tarfile_name.tar *.png 
~~~

