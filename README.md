# What is this? 
This is my (kng's) personal configuration for the tools I use, right now that is mostly Tmux and Vim. 

These configs are portable between systems, as I tend to live in Vim or Tmux rather than a particular OS. I may end up with an emacs config as well (for writing markdown).

You are free to use these with attribution if you are doing so in a public forum. 

I have made these configs so I can be efficient in any terminal using just the keyboard and with minimal hand movements, the Tmux config allows quick resizing and making of new panels and windows. If you have acpi it will show your laptops battery. I live in Tmux so these are minimal but good.

The vim config is more complicated and more of a work-in-progress. I use it for Rust and C (mostly N64 stuff). It has code-completion if you have nodejs and tags. It should auto install and configure itself but often you'll have to tweak it a bit and restart Vim a few times. The only real command you need to remember is ToggleTagbar as that is what brings up the tagbar (I don't have it on by default usually). 

I prefer light-themes but I switched to Solarized and Dark plays more nicely with default cursor highlighting. 

I don't have nerdfonts or any fancy themes, they're too much work. Half the time I'm just in a bare zsh session because I keep breaking my Thinkpad and the battery is too far gone to run a window manager. You will have to bring your own paint if you want a pretty system.

Here is an overview of the tmux config shortcuts, which you can also get in your terminal by going 'cat tmux_hints' in the project directory. Essentially it revolves around using alt (or option on Mac) and a combination of I-O-P-[ keys as up-down-left-rigth arrow keys, ; and ' for panel splits and a combination of the n key and spacebar for window hopping/management - with the Shift key acting as an 'alternate' command in the grouping (i.e. Alt+[ jumps left, but Alt+Shift+[ resizes left, Alt+' splits the panel vertically, Alt+Shift+' kills the active panel):
```
################|####################################
       Shortcut | Binding
################|####################################
       Prefixes | 
================|====================================
Ctrl + B        | prefix 
Alt + `         | prefix2
=====================================================
       Panel... |
================|====================================
                | Management
----------------|------------------------------------
Alt + '         | Split Panel Vertically
Alt + ;         | Split Panel Horizontally
Alt + Shift + o | Resize Panel Up
Alt + Shift + p | Resize Panel Down
Alt + Shift + [ | Resize Panel Left
Alt + Shift + ] | Resize Panel Right
Alt + Shift + ' | Kill Panel
----------------|------------------------------------
                | Navigation
----------------|------------------------------------
Alt + o         | Select panel above active panel
Alt + p         | Select panel below active panel
Alt + [         | Select panel left of active panel
Alt + ]         | Select panel right of active panel
================|====================================
      Window... |
================|====================================
                | Management
----------------|------------------------------------
Alt + n         | New Window
Alt + N         | Kill Window
----------------|------------------------------------
                | Navigation
----------------|------------------------------------
Alt + Space     | Next Window
Ctrl + Space    | Previous Window
################|###################(End-of-File)####
```
