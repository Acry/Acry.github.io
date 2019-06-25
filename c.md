---
title: SDL2-C
layout: page
icon: fa-code
order: 2
---

My efforts to make coding with pure C and SDL2 more clear and fun.


A Collection of SDL2 C Tutorials and Demos, SDL2 with OpenGL / ~~Vulkan~~ and other APIs. Procedural ~~Sounds~~ and Graphics, plus GLSL Shaders for Game-Programming and general purpose. All done in pure C.

___

<p align="center">
Why C?<br>
Cause C is seeing!  =)
</p>


### Foreword

Feel free to [contact me](/jekyll-theme-prologue/#contact) for criticism, Demo Requests or whatever!
Oh, you can use the code as you wish, but don't blame me!
*Happy hacking!*


### Coverage

I am trying to cover the [SDL2-API](https://wiki.libsdl.org/APIByCategory) as needed, OpenGL, Vulkan and a couple of other common API's like curl or jannson, tho this is pure C and mainly Linux orientated, doesn't mean I don't cross-compile for Windows or Android. If you need a german translation I could make that happen. SDL-Audio Series and Joystick/Gamecontroller Series are nearly finished, just polishing it. At the same time I am building up my [C-Snippets](https://gist.github.com/Acry/554e04bab3a2669a5ba2ecd4d673e875), but I am pretty behind on that. [SDL_net 2.0](https://www.libsdl.org/projects/SDL_net/) isn't covered yet.


#### Procedurale Sound Annotation

I spent quite some time on that topic and decided that it's not worth going further.
The Hardware isn't there yet. The focus of the past few decades was to improve GPU's.
Common audio chips are simpler than ever, if one compares the complexity of a GPU and an audio chip it is clear that the audio chip doesn't reveals a lot functionality.


### Requirements
You should have a working C-Environment and [SDL2 Development Libs](https://www.libsdl.org/download-2.0.php) installed; preferable some of the extensions to SDL, like [Mixer](https://www.libsdl.org/projects/SDL_mixer/), [Image](https://www.libsdl.org/projects/SDL_image/) and [TTF](https://www.libsdl.org/projects/SDL_ttf/).

If you struggle with getting things up and running, refer to one of those pages:
[Will Usher](https://www.willusher.io/sdl2%20tutorials/2013/08/15/lesson-0-setting-up-sdl) or
[Lazy Foo](http://lazyfoo.net/tutorials/SDL/01_hello_SDL/index.php).
**For Mac OS**: Setting Up An SDL2 Project [in Xcode 9](http://matthewstyles.com/set-up-an-sdl2-project-in-xcode/) or [without Xcode](https://medium.com/@edkins.sarah/set-up-sdl2-on-your-mac-without-xcode-6b0c33b723f7).
And if you wish to use **SDL2 with CMake**: [Trenki's Dev Blog](https://trenki2.github.io/blog/2017/06/02/using-sdl2-with-cmake/)


### Entry Level
[SDL2-Surfaces](https://github.com/Acry/SDL2-Surfaces)
<video src="assets/vids/surfaces.mp4" poster="assets/ss/surfaces.jpg" width="320" height="200" controls preload></video>
This is a set of small introductory programs.
It's about the window, the window icon, a custom cursor, surfaces,
Pixel Manipulation and how to save a screenshot.

#### SDL-Renderer
An Introduction to the Rendering Subsystem.
[SDL2-Renderer](https://github.com/Acry/SDL2-Renderer)
Create a texture from surface, render it flipped, mirrored and rotated.
Take Screenshot with RenderReadPixels.
Render and animate a colorful gradient like a new shadertoy one.
Shows a bit how glsl works and why we want shaders.

#### SDL-Timers

[SDL2-Timer-01](https://github.com/Acry/SDL2-Timer-01)
Records the duration how long left MouseButton is pressed.

[SDL2-Timer-02](https://github.com/Acry/SDL2-Timer-02)
Program quits after a certain amount of time.

#### Put it together
[SDL2-SpriteAnim](https://github.com/Acry/SDL2-Anim01)
<video src="assets/vids/sprite_animation.mp4" poster="assets/ss/sprite_animation.jpg" width="320" height="200" controls preload></video>
Create Spritesheet from gif and render it timed.

[SDL2-GUI-Button](https://github.com/Acry/SDL2-GUI-Button)
Responsive Button.

[SDL2-Mousegrab](https://github.com/Acry/SDL2-Mousegrab)
<video src="assets/vids/mouse_grab.mp4" poster="assets/ss/mouse_grab.jpg" width="320" height="200" controls preload></video>
Let rect follow the mouse.

[SDL2-Slider](https://github.com/Acry/SDL2-Slider)
<video src="assets/vids/slider.mp4" poster="assets/ss/slider.jpg" width="320" height="200" controls preload></video>
It is a follow up from Mousegrab. Shows how to make a Slider.

#### Drag and Drop
[SDL2-DnD](https://github.com/Acry/SDL2-DnD)
Drag and Drop. Receiving Text and Files via SDL_DropEvent.

#### Audio
[Play music with SDL2](https://github.com/Acry/SDL2-Mixer-play_music_mp3)
Use of SDL-Mixer for Music.

[SDL2-Mixer-play_mp3](https://github.com/Acry/SDL2-Mixer-play_mp3)
Use of SDL-Mixer for Sound.

### Put it together
[SDL2_simple_music_player](https://github.com/Acry/SDL2_simple_music_player)
Use of SDL-Mixer and GUI-Elements.

[SDL2-Parallax-02](https://github.com/Acry/SDL2-Parallax-02)
<video src="assets/vids/parallax.mp4" poster="assets/ss/parallax.jpg" width="400" height="225" controls preload></video>
Rapid Parallax implementation with 6 Layers.

[SDL2-Titlebar](https://github.com/Acry/SDL2-Titlebar)
Roll your own titlebar.

#### Fonts
[SDL2-TTF](https://github.com/Acry/SDL2-TTF)
<video src="assets/vids/ttf.mp4" poster="assets/ss/ttf.jpg" width="468" height="197" controls preload></video>
This is a series about the SDL-Extension SDL_ttf 2.0

#### Procedural/algorithmic Textures
[SDL2-Textures](https://github.com/Acry/SDL2-Textures)

#### (Game-)Physics
[SDL2-Game-Physics](https://github.com/Acry/SDL2-Physics)
This is a series about physics - SI-Units, Velocity, Acceleration, Gravity, Friction etc.

#### Artificial intelligence (AI)
[SDL2-Game-AI](https://github.com/Acry/AI)

#### Curves
[SDL2-Curves](https://github.com/Acry/SDL2-Curves)
<video src="assets/vids/casteljau.mp4" poster="assets/ss/casteljau.jpg" width="320" height="200" controls preload></video>
How to apply De Casteljau's algorithm on a quadratic Bézier curve.

#### More Textures
[SDL2-create_tex_part_of_win](https://github.com/Acry/SDL2-create_tex_part_of_win)
Re-Render a part of the screen using SetRenderTarget and SDL_TEXTUREACCESS_TARGET.

[SDL2-TextureColorMod](https://github.com/Acry/SDL2-TextureColorMod)
<video src="assets/vids/colormod.mp4" poster="assets/ss/colormod.jpg" width="320" height="200" controls preload></video>
This small demo shows how to use [TextureColorMod](https://wiki.libsdl.org/SDL_GetTextureColorMod?action=fullsearch&context=180&value=TextureColorMod&titlesearch=Titles).

#### A simple Game
[Pong](https://github.com/Acry/SDL2-Pong)
<video src="assets/vids/pong.mp4" poster="assets/ss/pong.jpg" width="320" height="200" controls preload></video>
My scaleable Pong implementation. You can take over two player control anytime, the AI will take over if you go afk. A [mingw](http://www.mingw.org) Windows 64 build is in the Makefile.

### Intermediate
*You need to fully understand pointers, [dynamic memory allocation](https://github.com/Acry/STD-C) and [bit operations](https://github.com/Acry/C-Bits).*

#### Strings/Input/Text
[SDL2-Text](https://github.com/Acry/SDL2-Text)
<video src="assets/vids/text.mp4" poster="assets/ss/text.jpg" width="425" height="217" controls preload></video>
This is a small SDL2 text API demo

#### A GIF-Viewer
[SDL2-Gif](https://github.com/Acry/SDL2-GifViewer)
<video src="assets/vids/gif_viewer.mp4" poster="assets/ss/gif_viewer.jpg" width="278" height="247" controls preload></video>
Plays an animated gif - pauseable and scaleable.
uses: [SDL_gifwrap](https://github.com/grimfang4/SDL_gifwrap)
by Jonathan Dearborn

#### SDL and OpenGL
[SDL2-OpenGL](https://github.com/Acry/SDL2-OpenGL)
This is a starter series about GLSL Shaders using SDL2 as OpenGL Helper and a bit Shader-Language for C-Coders.

[NanoVG-SDL2 starter](https://github.com/Acry/SDL2-nanovg-example)
Startup Code to use SDL2/OpenGL/NanoVG

[Shade it!](https://github.com/Acry/Shade-it-)
<video src="assets/vids/Shade_it.mp4" poster="assets/ss/ldf3DN.jpg" width="398" height="232" controls preload></video>
Using SDL2 to show [Shadertoy](https://www.shadertoy.com/) GLSL Fragment Shaders.
Features "drag and drop", Auto-Screenshot with shadername, editing with Auto-Compile.
~~WIP: Finishing SDL2-Audio right now, to move on to FFT and finally implement
visualization of GLSL shaders with low latency.~~

#### Misc Demos
[SDL2-Demo-01](https://github.com/Acry/SDL2-Demo-01)
<video src="assets/vids/Demo_01.mp4" poster="assets/ss/Demo_01.jpg" width="325" height="220" controls preload></video>
Demo using SDL2 Image, SDL2 TTF, SDL2 Mixer.

[Byte_Drawer](https://github.com/Acry/Byte_Drawer)
<video src="assets/vids/byte_drawer.mp4" poster="assets/ss/byte_drawer.jpg" width="358" height="327" controls preload></video>
Flipping Bits on a real char and visualize that.

## Random Stuff
### C&C++ mixed Code:
[Classic Pong and Breakout stuff](https://github.com/Acry/SDL2-pong_issue-01)
Ressources covering Atari's classic game.

[C++ game engine skeleton](https://github.com/Acry/cpp-game-engine-skel)
with GNU-Makefile

### Misc
[My C Code](https://gist.github.com/Acry/554e04bab3a2669a5ba2ecd4d673e875)
C-Idioms, C-Examples, C-Tutorials, C-Snippets

[Light Template](https://github.com/Acry/SDL2-C-KDev_App_Template_light)
SDL2 Template for [KDevelop](https://www.kdevelop.org/)

[Heavy Template](https://github.com/Acry/SDL2-C-KDev_App_Template)
SDL2 Template for [KDevelop](https://www.kdevelop.org/) - with TTF & Mixer

[Simple-state-pattern](https://github.com/Acry/simple-state-pattern)
High Level Game State Management - Code Flow diagram.

[Game Loots](https://github.com/Acry/Game_loots)
This guide is intended to get the Idea of random drops
and as introduction to random distribution or weighted distribution.

## External ressources
### C
[Stephen Meier's SDL2 Tutorials](https://www.google.de/search?q=site%3Awww.stephenmeier.net+%22SDL-2-0-Tutorial-%22&oq=site%3Awww.stephenmeier.net+%22SDL-2-0-Tutorial-%22)

SDL Mixer:
[change Frequency during runtime](https://gist.github.com/danilolc/9fff54a8cb9ddc04b9bd82df7badb610)

### C++
<http://gigi.nullneuron.net/gigilabs/writing/sdl2-tutorials/>

### Emscripten
[Emscripten and SDL 2 Tutorial](https://lyceum-allotments.github.io/2016/06/emscripten-and-sdl-2-tutorial-part-1/)
