---
title:  "Response to A List Apart (images)"
date:   2016-10-03 11:23:00
description: Image Article Response
---

The "responsive images" solution is to deliver optimized images to end'users rather than sending original or large images to everyone. This practice wasn't so simple as it sounds. 

For as far as I understand from the article, WHATWG has proposed a method to set **new** attribute to the **img** element. The proposed syntax is as follows: 

```HTML
<img src="face-600-200@1.jpg" alt=""
    set="face-600-200@1.jpg 600w 200h 1x,
         face-600-200@2.jpg 600w 200h 2x,
         face-icon.png      200w 200h">
```

Which breaks the image srource into multiple resolutions. Other group (RICG) has proposed abut the same thing and it also uses behavior specified on wc3.org.

The proposed markup is as follows:

```HTML
<picture alt="">
   <source src="mobile.jpg" /> 
   <source src="large.jpg" media="min-width: 600px" />
   <source src="large_1.5x-res.jpg" media="min-width: 600px, »
       min-device-pixel-ratio: 1.5" />
   <img src="mobile.jpg" />
</picture>
```

I think that the problem is that people have different suggestions for how to go about solving the problem, and nobody is sure that which is the best method, and it still needs to be actively discussed.


Source: [alistofthings]
*[WHATWG]: Web Hypertext Application Technology Working Group
*[RICG]: Responsive Images Community Group

[alistofthings]: http://alistapart.com/article/responsive-images-and-web-standards-at-the-turning-point