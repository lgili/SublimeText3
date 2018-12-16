# Sublime Text 3 Setup
My setup is based on [Ijy](https://gist.github.com/ijy/7399688) config.
 
## Install Package Control
https://gist.github.com/ijy/7399688
Install [Package Control](https://sublime.wbond.net/installation) for easy package management. 

1. Open the console with `` Ctrl+` ``
2. Paste in the following:

````
import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 
````

From here on out, use [Package Control](https://sublime.wbond.net/browse) to install **everything**. `CTRL`+`Shift`+`P`, then type `Install package` to get a list of installable packages you can livesearch through. Watch the Status Bar for installation progress.

## Add Some Style

Install [Material Theme](https://packagecontrol.io/packages/Material%20Theme) for some UI customisations. You'll need to restart Sublime after installation for the changes to take effect.


## Add Some Useful Packages

All installed with Package Manager. `CRTL`+`Shift`+`P` and type `install package`. Then start typing the name of the extension you want to install.

### General 


- [SideBarEnhancements](https://github.com/titoBouzout/SideBarEnhancements/tree/st3) Provides enhancements to the operations on Sidebar of Files and Folders.
- [SublimeCodeIntel](https://sublime.wbond.net/packages/SublimeCodeIntel) - Full-featured code intelligence and smart autocomplete engine.
- [AdvancedNewFile](https://sublime.wbond.net/packages/AdvancedNewFile) - Fast file creation within a project.
- [Nettuts+ Fetch](https://sublime.wbond.net/packages/Nettuts%2B%20Fetch) - Fetch the latest version of remote files and zip packages.
- [Gist](https://sublime.wbond.net/packages/Gist) - Gist management.Create, read, update, and delete gists from within Sublime. 
- [ApplySyntax](Provides a real-time Word Count and character count in the status-bar) - Better syntax detection.
- [Alignment](https://sublime.wbond.net/packages/Alignment) - Easy alignment of multiple selections and multi-line selections.
- [DocBlockr](https://sublime.wbond.net/packages/DocBlockr) - Simplifies writing DocBlock comments in Javascript, PHP, CoffeeScript, Actionscript, C & C++.

### HTML, CSS & JS
- [Emmet](https://sublime.wbond.net/packages/Emmet) - (Formerly Zen Coding) For lightning fast coding.
- [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter3#sublimelinter3) - Coming soon. Code linting & hinting for HTML/CSS/JS.
- [Sass](https://sublime.wbond.net/packages/Sass) - Adds syntax highlighting and tab/code completion for Sass and SCSS files. Also features Emmet shortcuts for many CSS properties.

### Git
- [GitGutter](https://github.com/jisaacks/GitGutter) tracks line changes in the gutter.
- [Modific](https://sublime.wbond.net/packages/Modific) - Highlight lines changed since the last commit.

### Markdown
- [MarkdownEditing](https://sublime.wbond.net/packages/MarkdownEditing) - Better Markdown editing from within Sublime.
- [Markdown Preview](https://sublime.wbond.net/packages/Markdown%20Preview) - Preview and build your markdown files quickly in your web browser from sublime text 2/3.
- [SmartMarkdown](https://sublime.wbond.net/packages/SmartMarkdown) - Some useful shortcuts for working with Markdown in Sublime. Brings better integration with Pandoc.
- [WordCount](https://sublime.wbond.net/packages/WordCount) - Provides a real-time Word Count and character count in the status-bar.

### Laravel 

- [Laravel 4 Facades](https://sublime.wbond.net/packages/Laravel%204%20Facades) - Easy access to the Laravel 4 Facades.

### ExpressionEngine

- [ExpressionEngine Add-on Builder](https://sublime.wbond.net/packages/ExpressionEngine%20Add-On%20Builder) - *(Waiting on ST3 support)* - Quick scaffold for EE addon development.

### Apache Conf

- [ApacheConf](https://sublime.wbond.net/packages/ApacheConf.tmLanguage) - For editing .htaccess and .conf files.

## Add Some Colour

- [Dayle Rees Color Schemes](https://github.com/daylerees/colour-schemes) - A collection of high quality colour schemes.
- [Github Color Theme](https://sublime.wbond.net/packages/Github%20Color%20Theme) - Simple github colour scheme.
- [Solarized Toggle](https://sublime.wbond.net/packages/Solarized%20Toggle) - A very simple plugin that lets you toggle between the dark and light default Solarized colour schemes.

## Settings - User

Accessible via: `SublimeText` &rarr; `Preferences` &rarr; `Settings – User`, or with `⌘`+`,'.'

This is a JSON file of custom user configuration settings. Kept in alphabetical order for easy reference.

**Note:** *As a JSON file no comments can be included. Any you add will be stripped out on saving.*

```json
{
"always_show_minimap_viewport": true,
"auto_find_in_selection": true,
"bold_folder_labels": false,
"caret_style": "wide",
"close_windows_when_empty": false,
"color_scheme": "Packages/Material Theme/schemes/Material-Theme.tmTheme",
"copy_with_empty_selection": false,
"create_window_at_startup": false,
"detect_indentation": true,
"dictionary": "Packages/Language - English/en_GB.dic",
"drag_text": false,
"file_exclude_patterns":
[
    ".DS_Store"
],
"folder_exclude_patterns":
[
    ".bundle",
    ".git",
    ".hg",
    ".sass-cache",
    ".svn",
    "bin",
    "CVS",
    "tmp"
],
"font_options":
[
    "subpixel_antialias"
],
"font_face": "Monaco",
"font_size": 10,
"highlight_line": true,
"highlight_modified_tabs": true,
"ignored_packages":
[
    "Vintage"
],
"indent_guide_options":
[
    "draw_normal",
    "draw_active"
],
"line_padding_bottom": 3,
"line_padding_top": 3,
"match_brackets_angle": true,
"material_theme_accent_orange": true,
"material_theme_compact_sidebar": true,
"material_theme_panel_separator": true,
"material_theme_small_tab": true,
"overlay_scroll_bars": "enabled",
"theme": "Material-Theme.sublime-theme",
"trim_trailing_white_space_on_save": true,
"word_wrap": true
}
```

A complete list of Settings can be referenced in `SublimeText` &rarr; `Preferences` &rarr; `Settings – Default`. 

Override any which aren't to your taste.

## Key Bindings - User

Accessible via: `SublimeText` &rarr; `Preferences` &rarr; `Key Bindings – User`. 

Key bindings are the productivity engine which allow you to become one with your text editor. I try to stick with all the defaults to make for an easy install and less chance of potential future clashes. The following are a few small edits I make along with some package specific controls:

```
[
    // Reveal the currently open file in the sidebar
    { "keys": ["ctrl+super+r"], "command": "reveal_in_side_bar" },

    // AdvancedNewFile
    { "keys": ["ctrl+alt+n"], "command": "advanced_new_file_new" },

    // Create a new snippet [Jeffrey Way]
    { "keys": ["alt+super+n"], "command": "new_snippet" },

    // Open iTerm
    { "keys": ["ctrl+alt+t"], "command": "open_terminal" },

    // Select (or type) the syntax to apply to the current view.
    { "keys": ["ctrl+shift+y"], "command": "show_overlay", "args": {"overlay": "command_palette", "text": "Set Syntax: "} },

    // swap the keybindings for paste and paste_and_indent
    { "keys": ["super+v"], "command": "paste_and_indent" },
    { "keys": ["super+shift+v"], "command": "paste" },

    // [HTMLPrettify] Format your HTML, CSS, and JS
    { "keys": ["super+shift+h"], "command": "htmlprettify" },

    // Close tag
    { "keys": ["super+."], "command": "close_tag" },

    // Alignment
    { "keys": ["super+shift+a"], "command": "alignment" },

    // Wrap selection in tag
    {
        "keys"      :   ["alt+shift+t"],
        "command"   :   "insert_snippet",
        "args": {
            "contents": "<${1:p}>${0:$SELECTION}</${1}>"
        }
    },

]
```

More info on Key Bindings can be found in the [unofficial docs](http://docs.sublimetext.info/en/latest/reference/key_bindings.html).

## Sublime from the Command Line

Sublime Text includes a command line tool which you just need to symlink up so that it's in your PATH file. In Sublime Text 3 simply copy this into a terminal session:

    ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" ~/bin/subl

Then you can open files in Sublime Text from the command line with:

    subl my_file.txt

Replacing `my_file.text` with the name of the file or folder you wish to open in Sublime Text.

## Sublime Text Dropbox Sync

If you switch between Macs at home and work then syncing via Dropbox is a huge time saver. To do this you only need to symlink your `Packages` and `Installed Packages` directories to a location in your Dropbox. Then symlink on the device your setting up to sync with those folders on Dropbox.

**Always make sure you backup your `Packages` and `Installed Packages` folders first - just in case anything goes wrong.**

So, once I have Sublime Text 3 installed on my MacBook Pro, I just need to create a symlink for both my `Packages` and `Installed Packages` directories in my Dropbox folder:

    ln -s ~/Library/Application\ Support/Sublime\ Text\ 3/Packages ~/Dropbox/Sync/Sublime\ Text\ 3/Packages

    ln -s ~/Library/Application\ Support/Sublime\ Text\ 3/Installed\ Packages ~/Dropbox/Sync/Sublime\ Text\ 3/Installed\ Packages

Then on my MacBook Air I just need to install Sublime Text 3 (basic install with none of the above) and tell it to look in Dropbox for the Package information:

    ln -s ~/Dropbox/Sync/Sublime\ Text\ 3/Packages ~/Library/Application\ Support/Sublime\ Text\ 3/Packages

    ln -s ~/Dropbox/Sync/Sublime\ Text\ 3/Installed\ Packages ~/Library/Application\ Support/Sublime\ Text\ 3/Installed\ Packages

Now whenever you tweak any settings or install any new packages the changes will be applied to all shared computers.

## Useful Shortcuts

Follow my other gist for useful Sublime Text shortcuts (on a Mac). Commit these to muscle memory and you'll amaze and scare your friends and colleagues with your crazy text editor wizardry. 

## Learn the Basics

Make sure you get familiar with the extremely useful _[Find in Files](http://www.macdrifter.com/2012/07/a-couple-of-sublime-text-tips.html)_ feature along with _[Fuzzy searches](http://docs.sublimetext.info/en/latest/file_management/file_management.html)_.

