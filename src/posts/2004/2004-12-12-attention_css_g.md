---
title: Attention CSS Gurus
slug: attention_css_g
date_published: 2004-12-13T00:34:08.000Z
date_updated: 2004-12-13T00:34:08.000Z
tags: tech
---

Okay, here’s an important feature request that I have, either for someone to code as a stylesheet or (assuming no browser supports the necessary level of CSS that’d be required) a Firefox extension:

Please play back the Windows “tada.wav” sound file whenever I’m viewing a page on the [W3.org](http://www.w3.org) site and either [valid-xhtml11](http://www.w3.org/Icons/valid-xhtml11) or [valid-xhtml10](http://www.w3.org/Icons/valid-xhtml10) image is displayed.

I’m thinking something like

    <br></br>
    .inline-badge {<br></br>
    play-during: url("tada.wav") mix !important;<br></br>
    volume: x-loud;<br></br>
    }<br></br>```
    
     
    
