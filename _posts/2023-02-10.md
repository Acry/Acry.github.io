---
title: Finding a CherryTree to Markdown converter
author: Acry
layout: post
---

To export my data from [CherryTree](https://www.giuspen.com/cherrytree/) to [markdown](https://daringfireball.net/projects/markdown/) I needed a converter.
I found the [CherryTree to Markdown converter](https://gitlab.com/kibley/cherrytreetomarkdown); problem: it is written in PHP and I don't had PHP installed on my machine. Currently I am on Manjaro.

___

Here is what I did to get it running:

- `sudo pacman -S php`
- in `/etc/php/php.ini` remove the semicolon to enable `extension=exif`

The converter uses composer for PHP dependency management:

- `sudo pacman -S composer`
- `php composer.phar update`
- `php composer.phar install`

Then run the shell script in the examples folder. Hope that helps.

___

Happy Hacking,<br>
Acry