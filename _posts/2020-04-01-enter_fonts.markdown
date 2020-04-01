---
layout: post
title:      "Enter...Fonts"
date:       2020-04-01 15:23:05 +0000
permalink:  enter_fonts
---

I wanted to use different fonts to make my application stand out more. I ended up deciding on a custom font which needed to be downloaded. Different browsers and browser types need different file extensions of the same font in order for them to appear in each respective situation. 

Even if I were to download all of them, how would I be able to allow the application to choose which one to use? Here enters...dun, dun, dun…@font-face.

Without the full technical jargon, @font-face handles imported fonts and chooses the one that is appropriate, so long as you have them imported. @font-face is declared in the .css file and imported in the .js file. After this you can attach it to a div(wrapper) with className and voila!

It’s easier said than done and you might need a webkit for your particular font. I needed one for mine and ended up using Font Squirrel(https://www.fontsquirrel.com/tools/webfont-generator) in order to get mine to actually show.

Hopefully this helps! Happy Coding!

