---
layout: page
title: About
permalink: /about/
---
{% assign dateStart = "2006-08-10" | date: '%s' %}
{% assign nowTimestamp = 'now' | date: '%s' %}

{% assign diffSeconds = nowTimestamp | minus: dateStart %}
{% assign diffDays = diffSeconds | divided_by: 3600 | divided_by: 24 | divided_by: 365 %}

My name is Emily Violet Vlasics. I'm {{diffDays | round: 0}}. I am currently a Mathematics Specialist at the University of Toronto---unless this is horrifically out of date. This iw typically where someone would put their fields of interest, but I plan to pursue all of math so this isn't applicable for me. If I had to narrow it down, I'd say I'll likely end up somewhere more analytic than not.

Aside from math, I like classical music (especially Piano), tea, listening to the CBC, and talking to my friends. When the weather is nice I like to go on walks. People have accused me of being old, despite my current tender age---I wonder why!

As you may have guessed, half of my blog's title derives from my middle name, which itself derives from my great-great-grandmother. I have no such familial connection to willows, I just like them.

![Willow tree](https://upload.wikimedia.org/wikipedia/commons/0/0c/Pond_and_Weeping_Willow%2C_Fairlawne_House_Grounds_-_geograph.org.uk_-_1363764.jpg)

Photo courtesy of Nigel Chadwick licensed under the [Creative Commons Attribution-Share Alike 2.0 Generic license](https://creativecommons.org/licenses/by-sa/2.0/deed.en).

<!-- While I have no familial connection to willows, I do have a more personal one. One of my most striking memories as a child was set underneath a willow tree. It was in the middle of a vast garden filled with many vibrant shades of green. The willow distinguished itself through contrast, its leaves carrying a pale silver cast. Looking back, the tree must have been in its middle years because its trunk was wide, but it hadn't yet grown tall enough that the branches could no longer reach the ground. These branches formed a veil which separated the underside of the willow from the rest of the world. Someone from outside the willow noticed me lying there, and they knelt down and told me that the tree was called a weeping willow. The name was strange to me, as I hadn't previously imagined the tree to be sorrowful. Why did it weep so? The hanging branches started to look less like a veil and more like a posture; in their limpness they resembled the lethargic stupor one might enter due to apathy. I recall feeling puzzled that I still managed to enjoy its shade and the sun sifting through its leaves despite the tree's despair. Soon after I was called away. -->
