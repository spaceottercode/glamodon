# Glamodon
User-Script that adds image filters, stickers, and image tweaking tools on Mastodon sites<sup>1</sup>

> 1. Stickers and tools will be made available soon.

Tested on Firefox running GreaseMonkey. Not tested on Chrome (running natively as an extension).

# Install

To run User-Scripts on Firefox based browsers you will need [Greasemonkey extension](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) installed and running. 

Next **[Click here](https://raw.githubusercontent.com/spaceottercode/glamodon/master/glamodon.user.js)** to automatically install the script.

If GreaseMonkey does not detect the User-Script, create a New User Script in GreaseMonkey, and replace the script's text with the contents of [glamodon.users.js](https://raw.githubusercontent.com/spaceottercode/glamodon/master/glamodon.user.js).

> Not tested on Chrome: No plugin is needed to run a User-Script in Chrome. Drag the script unto your browser's extension window to install. 


> This User Script by default, runs on the following sites:
>
>   * mastodon.social
>   * mastodon.art
>   * mstdn.io
> 
>   Add your Mastodon site by adding a new @match line at the top of the script or replacing an existing one


# TODO/WIP

### filters

* the ability to scroll filters left and right
* the ability to add and remove filters
* the ability to reorder filters
* document how to make custom filters
* frames

### stickers

* adding stickers is a high priority. ideally should be extensible and distributable. 
  Simplest way is to allow any png (of limited size) to be imported as a sticker 
* Of lesser priority but nice to have, animated stickers

### tools

This is where you'll find things like the focal point tool and other tools like rotate (90º)

* focal point
* rotate CW, CCW, flip
* brightness & contrast
* saturation
* curves, exposure, gamma
* color
* blurs
* text

# Version

### 0.1

apply one of ~10 filters to a pic and upload. Privacy and text can be set in the main UI (compose message box). Spoiler text has limited support. In this release the processed image can be upto 640x640 but this will be lifted.


