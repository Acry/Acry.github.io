---
title: VS Code on Arch-Linux
author: Acry
layout: post
---

# Installing VS Code on Arch-Linux

## Technical Side

### What is VS Code?

It is a multi-platform software developer tool (IDE) by Microsoft. Written in JavaScript and TypeScript, built on the Electron framework.

<https://code.visualstudio.com/>

VS Code's source code is [MIT-licensed](https://choosealicense.com/licenses/mit/), but the product available for download (Visual Studio Code) is licensed under [this not-FLOSS license](https://code.visualstudio.com/license) and contains telemetry/tracking.

### What is VSCodium?

**The binaries are licensed under the MIT license. Telemetry is disabled.**

The VS Codium project exists so that you don’t have to download+build from source. This project includes special build scripts that clone Microsoft’s VS Code repo, run the build commands, and upload the resulting binaries for you to GitHub releases.

<https://vscodium.com/>

### More ways to go

The following packages provide VS Code:

Community Repository:

- code (open-source release)

Arch User Repository:

- visual-studio-code-bin (Microsoft-branded release)
- visual-studio-code-insiders (Microsoft-branded release, daily/nightly snapshots)
- code-git (development git repository)
- vscodium-bin

The Microsoft [ptvsd](https://github.com/microsoft/ptvsd) (Python Tools for Visual Studio Debug) server/module is available at python-ptvsd AUR.

### Installation

I am going with the version in the community repository:<br>
<https://www.archlinux.org/packages/community/x86_64/code/><br>
Version as of time of writing: code-1.47.0-1.<br>
`sudo pacman -S code`<br>

If you can't find the version, make sure you updated the package-db with `sudo pacman -Syy`.

### References

Arch-linux has in general pretty good docs:<br>
<https://wiki.archlinux.org/index.php/Visual_Studio_Code>

## Background-Story

In short: I have been looking for a reasonable C-IDE for decades. I was experimenting with VS Code and C quite a few hours, since I am using VS Code for work with TypeScript. I am going to start using it for my new demos and tutorials.

Cheers,<br>
Acry
