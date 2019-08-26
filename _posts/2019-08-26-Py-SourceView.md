---
title: Python 3 - GObject - GTKSource
author: Acry
layout: post
---

## Source View

The Sourceview is an alternative Textview - it is specialised to view and edit source-code. One _really_ should have used [Gtk.Textview](https://github.com/Acry/PyGObject-GTK/blob/master/Gtk/Text/Notes.md) before using GtkSource.View in code.

The main problem is that Sourceview's [GObject Introspection](https://gi.readthedocs.io/en/latest/#gobject-introspection) is not working fully, yet.

Sometimes a bit of hacking and fiddling is needed to reach a goal. For now, after wrestling a bit with the bindings and jumping through some loops, I am quite satisfied with my code.


<video src="assets/vids/sourceview.mp4" width="806" height="498" controls preload></video>

[Check the README's and the code.](https://github.com/Acry/PyGObject-GTK/tree/master/GtkSource/4)


## Background

I have been using [Pygments](http://pygments.org/) as highlighter, which is working quite well under GTK. Currently working on a Snippet-Manager, cause I am tired that every IDE provides its own. And as usual import and exports across IDE-Snippets is a pain.