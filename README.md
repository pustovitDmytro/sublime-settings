# My sublime settings

Windows:
%AppData%\Sublime Text 3\Packages\User

Linux:
~/.config/sublime-text-3/Packages/User

[reference](http://popel-studio.com/blog/article/perenos-nastroek-sublime-text.html)


Color Picker on **Ubuntu 16.04**:

just edit ~/.config/sublime-text-3/Packages/ColorPicker/lib/linux_colorpicker.py,
search this line
```python
if color_sel.run() == getattr(Gtk, 'RESPONSE_OK', Gtk.ResponseType.OK):
```
change to
```python
if color_sel.run() == getattr(Gtk, 'RESPONSE_OK', Gtk.ResponseType):
and save.
```