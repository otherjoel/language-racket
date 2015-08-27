# Racket & Scribble syntax support for Atom

Syntax support for Racket language and the Scribble documentation tool. This fork mainly adds support for [Pollen](http://pollenpub.com) syntax as well.

## Installation

This folder should go in your `~/.atom/packages` folder, which will cause it to be automatically loaded when Atom starts. Files with the extensions `pm`, `pp`, and `ptree` will automatically use the new Pollen syntax definitions.

If Atom is already running when these files are added or changed, you can make this take effect by pressing `CMD+SHIFT+P` and typing `Window: Reload`.

## Pollen support

Since Pollen is based on Scribble, I've added support for Pollen by simply copying `grammars/scribble.cson` and making some simple in-place edits: swapping out `@` for `◊` where appropriate, changing the class names from "scribble" to "pollen", and adding the Pollen file extensions.

I'm new to Atom, so I haven't attempted anything elaborate here. Comments and pull requests welcome.
