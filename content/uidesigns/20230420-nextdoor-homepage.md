---
date: 2023-04-22
title: NextDoor Homepage (Android)
thumbnail: 20230422_Copywork_NextDoor_Thumbnail.webp
images:
- 20230422_Copywork_NextDoor.webp
category: UI Designs
tags:
- copywork
---

I wanted to do an Android screen, so I picked three screens imitating NextDoor ([1](https://mobbin.com/screens/1c73f803-7c9e-4d3b-b08d-5c2ba1395171),[2](https://mobbin.com/screens/b5f45ac2-a082-4542-8a89-5176623d1cb4),[3](https://mobbin.com/screens/1df034ab-675e-456a-9dab-475535635692)).

* Beyond the status and navigation bars, NextDoor didn't really draw on any Android or Material 3 patterns. Still, it got me exploring a Material Design kit in Figma, and becoming somewhat more familiar with the names there.
* Font sizes are bit wonky: 12, 14, 16, 22. The card font sizes were actually _in-between_ the font sizes everywhere else: 11 and 13. It made me wonder if the card text sizes were actually 12 and 14, but shrunk down automatically somehow. 

{{< figureUIdesign 
    src="20230422_Copywork_NextDoor_cardcomponent.webp" 
    title="The 'Deal' card component" >}}

* Speaking of type: the line-height and kearning needed to be manually adjusted for each font size to match the screenshot. I always see type specified as "size" / "line-height," but I rarely see kearning adjustments specified? Need to look into this.
* The icon set was not something I could find. Some of them matched my go-to, Phosphor Icons, really nicely. But some of them had no corollary anywhere I could find, such as the "For Sale" icon with its little drawstring (quite nice, actually).

{{< figureUIdesign 
    src="20230422_Copywork_NextDoor_prototype.gif" 
    title="Simple prototype" >}}

* Had I had a little more time to play with prototyping, I would have liked to try to show how the top "sticky" region shrinks to hide search when you scroll down (i.e. [Krisztian Nagy's](https://www.figma.com/community/file/1022835635343164608) solution).