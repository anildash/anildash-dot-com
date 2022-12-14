---
title: Who will save the tables?
slug: who_will_save_the_tables
date_published: 2009-04-02T04:14:07.000Z
date_updated: 2009-04-02T04:14:07.000Z
tags: tech
---

About a decade ago, the web development industry made a decisive shift towards [support for web standards](http://www.webstandards.org/). Though the effort encompassed many related efforts around HTML, CSS, the DOM and related technologies, perhaps the signature work of the movement was to encourage CSS-based layouts instead of the then-common practice of using HTML tables to design a page’s visual appearance.
![Table](http://dashes.com/anil/images/table.jpg)

The campaign was extraordinarily effective, to the degree that most new sites that launch today use CSS as their primary system for styling and positioning. And the more socially inept web geeks out there still consider those who use tables for layout worthy of their derision, instead of opportunities for education. Tables have fallen so far out of favor that it’s not uncommon for people to be reluctant to use them even for the presentation of *tabular data*.

In short, for front-end web developers, tables are definitely out of fashion.

More recently, web architects and developers have adopted a new generation of storage technologies for data, such as [BigTable](http://www.cs.washington.edu/htbin-post/mvis/mvis?ID=437) and [SimpleDB](http://aws.amazon.com/simpledb/). While these systems still use tables to store data, it’s common to have a far smaller number of columns in these tables than were used in older systems. And their advantages in areas like scalability and partitioning, have encouraged lots of developers to consider adopting these new data storage systems despite their unfamiliarity.

In short, for back-end web developers, fat tables are rapidly going out of fashion.

Now, I don’t mean to suggest that these technological trends are merely about geeks following what’s faddish or popular amongst their peers. In fact, in both cases, the shift away from traditional tables might reflect the fact that our data has to be more nimble in both how it’s stored and retrieved and in how it’s presented and styled. These accommodations are necessary because the applications being built are more social and human-centric in nature, which means they have to be able to adapt and evolve as relationships and communities mature.

But part of me can’t help but feel sad for the tables. I’m sorry, tables! I hope you come back in favor soon.

(Thanks to [Mo](http://www.flickr.com/photos/mnadi/32325828/) for the image.)
