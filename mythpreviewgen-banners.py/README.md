mythpreviewgen-banners
======================

*Now with Python goodness, this new and improved script should be used instead of [the old one](https://github.com/sammyjayuk/sj-mythtv-scripts/tree/master/mythpreviewgen-banners).*

Until MythTV supports using a banner imagetype widget in the recordings buttonlist, this is a script that, instead of making a framegrab of a recording, will look up the recording’s banner and use that.

My themes [Barry](https://github.com/sammyjayuk/Barry_dev) and [Anita](https://github.com/sammyjayuk/Anita_dev) are best used with this script.

*This script has only been tested on Mac OS X*, but should work just fine on Linux.

Unlike [the old script](https://github.com/sammyjayuk/sj-mythtv-scripts/tree/master/mythpreviewgen-banners), this one should support pretty much any Storage Group configuration. Or rather, it pays no attention to them, instead using the Python bindings to ask MythTV for the files. This has one caveat: if an episode of a series doesn't have season and episode numbers, the Python bindings won't return a file. This doesn't seem to affect films.

Configuration & Installation
----------------------------

I’ll keep it brief.

You’ll need imagemagick installed, so go get that.

You'll also need to make sure that MythTV's Python bindings work properly. If metadata lookup is working, which is needed anyway for there to be any point to this script, then you're almost certainly fine.

That’s almost it, so time for a **big fat warning/disclaimer**:
*This script may result in actual death, as a result of your fiancé/fiancée/husband/wife bludgeoning you to death with a remote control because all your recordings have disappeared. I cannot be held responsible for this (not that you would be in a position to hold anyone anything, since you would be dead), or anything else.*

That said, I have been using this script for several months, and fiancé-remote-control-bludgeoning has yet to occur, at least as a result of this script.

Finally, find `mythpreviewgen` on your system (probably `/usr/bin/mythpreviewgen` on Linux, `/opt/local/bin/mythpreviewgen` for MacPorts), move it aside, and put this script in its place, remembering to check that the executable bit is set appropriately and adjusting the shebang (if necessary) to point to bash.

If you're having trouble finding `mythpreviewgen` on your system, try running `which mythpreviewgen`.

End
---

If you find this script, or any of my other work, useful please consider supporting an LGBT+ charity. If this is objectionable to you politically, please bear in mind that in many places across our world LGBT+ people *literally* fear for their lives.

If you do still feel that you could not support an LGBT+ organisation, instead consider a mental health charity, or a charity for people with disabilities.

Thank you.
