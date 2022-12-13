---
title: The W3C has a comprehensive
slug: the_w3c_has_a_c
date_published: 2001-10-08T15:48:58.000Z
date_updated: 2001-10-08T15:48:58.000Z
---

The W3C has a [comprehensive default CSS document](http://www.w3.org/TR/REC-CSS2/sample.html), which basically just codifies the default practices of most existing visual browsers. It’s a nice base to work off of, especially if you’re going to make extensive changes to the display of common elements.

One change I would make for most web projects would be to exclude `FORM` from the big list of block elements at the beginning, and perhaps use the following instead:

form { display : inline; }

This one little change would help eliminate most of the "the  tag always inserts extra space!" problems that web designers using  layouts have struggled with for years.
