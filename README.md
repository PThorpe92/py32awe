# py3status to awesomewm
A module for converting [i3status](https://i3wm.org/docs/i3status.html)/[py3status](https://github.com/ultrabug/py3status) json output
to awesomewm widgets, with colorization & clickibility.

This is a module that takes an [awful.widget.layoutbox](https://awesomewm.org/doc/api/classes/awful.widget.layoutbox.html) and
populates it with [awful.widget.textbox](https://awesomewm.org/doc/api/classes/wibox.widget.textbox.html)s for each module,
and updates them when py3status spits out an update. It also
attaches button handlers that pass commands to py3-cmd.

Note:
I wrote this for py3status, but it should work for i3status.
Not tested, and you'll have to put output_format = json in
the config file.
