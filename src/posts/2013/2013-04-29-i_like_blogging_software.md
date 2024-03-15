---
title: I like blogging software.
slug: i_like_blogging_software
date_published: 2013-04-29T18:27:22.000Z
date_updated: 2013-04-29T18:27:22.000Z
image: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/ghost-kickstarter.jpg.webp?v=1670559878259
tags: [tech, web, software, blogs]
---

I lament the end of the personal CMS market; I was happy to back [Ghost](http://www.kickstarter.com/projects/johnonolan/ghost-just-a-blogging-platform) on Kickstarter today for the same reason that I back pretty much any effort at making blogging software — I think these tools matter. I find it interesting, and telling, that there are still [so many static publishing tools](https://news.ycombinator.com/item?id=4857473) that geeks care about, and though I think WordPress is an awesome tool, I lament the virtual monoculture that’s resulted from its success in the run-your-own blogging software market.

This is a particularly acute pain for me not just because I used to help make these kinds of tools, but because my own needs are sort of prosumer-grade concerns. We have the Garage Bands and iMovies of blogging, but we really don’t have Logic or Final Cut for individual bloggers who aren’t trying to run some giant professional blogging network.

So, my contribution is to collect some of the notes I’ve been gathering for the last few years about what I’d like to see in a blogging tool. I know there are apps with many, perhaps even all, of these features, but I’d like to see one emerge as a leading platform for doing innovative work. My blogging features wishlist:

- I enter markdown in plain text files; these are stored on Dropbox/Google Drive/Skydrive and/or S3 and/or GitHub.
- The system renders those plain files into JSON assets in a documented format.
- A Bootstrap-themed reading client app lives at my site, on my domain, and reads a single simple config file to learn how to display and navigate between those JSON assets. This client app would also have to handle URL routing and persisting states, while ideally also keeping preferences and reading history for readers.
- The default theme offers a YouTube-style browsing view of all my content, where people can make playlists of posts (this is equivalent to navigating my archives by tag), embed my posts on their own sites, and easily explore by traditional groupings like category or date.
- There might be an optional administration interface separate for me, just for editing the markdown files through a plain text in-browser editor; In this case, it should be a responsive app that works in all my browsers.
- Ideally comments are handled as small messages in a documented json format, sent between instances of this blogging application. Of course in the short term I would just embed Disqus/Facebook/Google-style comments until that infrastructure was further along.
- Having a documented format for the json objects which represent posts and comments would permit transclusion and sending of posts between sites, in a manner analogous to how [Fargo](http://fargo.io/) does this for outliners, and in a way that would bring back some of the positives of TrackBack in the early blogosphere.
- “Themes” would largely be implemented as Bootstrap CSS stylesheets, with some affordance for separate content modules. By default, themes are public so I would just be able to tell an admin app to import a theme from your site so I could remix it.
- The API endpoint for discovering the json representations of content would double as the API for others to access my data to build around it; Eventually a posting app which saved POSTs of that json format as fiels in dropbox would allow a write API.

I think that’s it for now. Let me know if somebody’s got all these boxes checked on their platform today, but I suspect the hardest part is the client app for readers, which works in a way analogous to an RSS reader or email client, but would have to support a new format and would be optimized for clean reading and subsequent discovery, rather than the three-pane model which has dominated those apps for the last decade or two.
