mythpreviewgen-banners
======================

**YOU WILL DEFINITELY NEED TO MODIFY THIS SCRIPT TO SUIT YOUR SYSTEM.** See [Installation](#installation) below.

**This script has only been tested on Mac OS X.** It has not been tested on any other system. Importantly, OS X uses BSD utilities, whereas Linux uses GNU. In this script, I use `head` and `cut`.

Until MythTV supports using a banner imagetype widget in the recordings buttonlist, this is a crappy script that, instead of making a framegrab of a recording, will look up the recording’s banner and use that.

My themes [Barry](https://github.com/sammyjayuk/Barry_dev) and [Anita](https://github.com/sammyjayuk/Anita_dev) are best used with ~~this script~~ *a better implementation of what this script does*, but failing that, you can use this one :P

Configuration & Installation
----------------------------

Still here? I’ll keep it brief, then—you obviously know what you’re doing.

You’ll need imagemagick installed, so go get that.

You’ll also need to make sure you have only one directory specified for each of the Storage Groups. Separate Storage Groups are fine.

Open the script in your favourite text editor, and change the settings at the top of the file to suit your system:

`art_storage` is where MythTV stores the metadata artwork for your recordings.

`pre_storage` is where the generated image should go.

`mysql_username` and `mysql_password` are the user name and password for MySQL. User name is generally "mythtv". You can find the password in the ~/.mythtv/config.xml file.

`mysql_command` is the location of the mysql command line client on your system.

That’s almost it, so time for a **big fat warning/disclaimer**:
*This script may result in actual death, as a result of your fiancé/fiancée/husband/wife bludgeoning you to death with a remote control because all your recordings have disappeared. I cannot be held responsible for this (not that you would be in a position to hold anyone anything, since you would be dead), or anything else.*

That said, I have been using this script for several months, and fiancé-remote-control-bludgeoning has yet to occur, at least as a result of this script.

Finally, find `mythpreviewgen` on your system, move it aside, and put this script in its place, remembering to check that the executable bit is set appropriately and adjusting the shebang (if necessary) to point to bash.

End
---

If you find this script, or any of my other work, useful please consider supporting an LGBT+ charity. If this is objectionable to you politically, please bear in mind that in many places across our world LGBT+ people *literally* fear for their lives.

If you do still feel that you could not support an LGBT+ organisation, instead consider a mental health charity, or a charity for people with disabilities.

Thank you.
