---
title: Underscores, Optimization & Arms Races
slug: underscores-optimization-arms-races
date_published: 2017-11-29T21:29:00.000Z
date_updated: 2021-08-02T04:12:14.000Z
image: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/type-curve-1.jpeg?v=1669782582770
tags: [web, google, search, tech]
---

A dozen years ago, the web started to reshape itself around major companies like Google. We can understand the genesis of today’s algorithmic arms race against the tech titans just by looking at a single character.
![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/typewriter-keys.jpeg?v=1669782631717)
This is all ancient tech history now, but content management systems used to be one of those competitive markets that tech people watched avidly. (CMSes are the tools people use to publish stuff on the Internet — Medium, where I originally wrote this, is one, and some of the big ones people use today are WordPress or Drupal.)

Back in the early 2000s, I helped create two then-popular CMS tools, Movable Type and TypePad; pretty soon, WordPress and Drupal and other tools came onto the scene solving a similar set of problems. All of these apps basically did the same thing they do today: You type in a box, and hit publish, and it makes a nice-looking web page with whatever you wrote. At first they were used by individual bloggers to keep personal sites, but they quickly took over publishing for almost every media outlet on the web. It was a booming market, and the people working on these tools were some of the first wave of high-profile social media startup founders.

Friendster was around then, and MySpace was growing in prominence. (Facebook didn’t come around until a little later, and was still just for Ivy League kids for a long time.) But the biggest player on the rise in that era was Google. They’d bought Blogger, one of the earliest popular social media tools, in early 2003 and then launched their AdSense advertising platform a few months later. All of a sudden, Google was massively influencing content and monetization in the new world of social media.

![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/type-keys.jpeg?v=1669782630996)

## Drawing a line

Just as we see Instagram and Snapchat going back and forth today one-upping each other’s features, in the early 2000s, people were constantly making new features for publishing in the then-new format of blogging. Todays social apps might distinguish themselves based on who has the best photo filters, but the technological distinctions between content management systems were a lot nerdier, like really esoteric and detailed technical controls over the design of your website.

The early era of the social web was a time of incredible advancement in web design. There was a revolution in aesthetics, focused around simplicity and white space and advances in typography and styling, and this was matched by huge leaps in accessibility and conformance with the open technical standards that defined the web itself. Basically, the web got a lot more pleasant really quickly, driven in large part by the influence of the people who were creating the early social media platforms. Things got good enough that it was worth the time to sweat little things like the formatting of web addresses.

Yep—we got so picky about design that one of the elements of a website that people wanted to control was the web address (URL) of the webpages themselves. At first, each of the posts on your blog would live at an address that was something like `example.com/00000002.html`, with the number going up each time you wrote a new post. But that long, nerdy-looking number offended a lot of people’s aesthetic sensibilities, so pretty soon addresses started to look like `example.com/2004/04/story.html` and that was a little better.

Eventually, people wanted to have the whole title of their article show up in the web address. Part of this was just because it looked cool, but some folks had started to suspect that having those words in the address might help a blog post rank higher on Google. (Google was still a smaller player in the overall web search market at the time, but it was already by far the most popular search engine amongst internet geeks.)

But here’s the thing: web addresses can’t have spaces in them. To include a full title with spaces in a web address for a blog, the spaces would either have to be removed (ugly!) or converted into something equivalent. Since we were one of the first to encounter this issue, our team designed to have our content management system use underscores, based on the rationale that underscores were the character that most closely resembled a blank space.

The end result? Anybody who used our tools could write a a blog post entitled “My Great Cookie Recipe” and it would live at an address that looked like `example.com/2005/04/my_great_cookie_recipe.html`. By contrast, the WordPress team thought that hyphens looked better, so blog posts published on their tool would look more like `example.com/2005/04/my-great-cookie-recipe`. Sure, these different tools made slightly different choices about which character to use, but such a subtle distinction couldn’t be meaningful, right?

As it would turn out, we’d stumbled across a harbinger of how the entire web was about to change.

![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/type-closeup.jpeg?v=1669782582297)

## The rise of SEO

Just as the social media era of the web was taking off, Google’s rapidly-growing platform radically changed the nature of content and sharing on the web. Anybody with a website was starting to understand that ranking highly on Google was immensely valuable, and as Google’s ad platform boomed, seeing those paid results alongside “organic” search results made it even clearer that a high ranking had monetary value.

Initially, information of how to rank better on Google was exchanged almost as folk knowledge—half urban legends or myth, half insights that were gleaned through painful experience but not documented anywhere. Soon, the dark arts of earning Google’s favor came to be known as “search engine optimization”, and what began as informal sharing of guesses about Google’s function started to grow into what became a multi-billion-dollar industry.

## Everybody Loves Dashes

Even as SEO matured and formalized, Google had very little documentation and no designated ombudsman to handle questions about how to be in their search engine’s good graces. Eventually, early Googler [Matt Cutts](https://www.mattcutts.com/blog/) took up the mantle of representing the company to the community as advocate for best practices in search optimization, using his personal blog to explain company policies that had heretofore been opaque or inscrutable. There was a feel of Kremlinology to the way his minor public utterances would be parsed for any hints that outsiders could glean about Google’s inner workings. But just as often, Cutts would make clear pronouncements of What To Do, and these were received by the SEO community almost as religious edicts.

One such declaration in the summer of 2005 came like a lightning bolt, a proclamation on [Dashes vs. underscores](https://www.mattcutts.com/blog/dashes-vs-underscores/):

> I often get asked whether I’d recommend dashes or underscores for words in urls. For urls in Google, I would recommend using dashes.

There was a lot of nuance in Matt’s post, but pretty soon the perception for a lot of SEO people became “**dashes good, underscores bad**”. (The punctuation in URLs are hyphens, technically known as Hyphen-minus, but sure, let’s call them dashes.) To most people in the industry, this settled things. Google had told us all what they preferred, and everybody wanted to rank highly in Google, so SEO experts fell in line. Everything was to be dashes, forevermore.

But once you’ve trained a community that they constantly need to guess at the secret machinations of your algorithm, they’re not going to stop doing so just because you’ve made a public pronouncement.

For years, despite Cutts’ clear statement, the choice of punctuation remained such a point of contention and debate that [countless](http://www.ecreativeim.com/blog/2011/03/seo-basics-hyphen-or-underscore-for-seo-urls/)[stories](https://www.seomechanic.com/seo-101-hyphens-underscores-_-urls/) were [written](https://searchengineland.com/9-seo-quirks-you-should-be-aware-of-146465) about how best to appease the fickle Googlebot. Eventually, discussion around hyphens and underscores in web addresses became so fraught and so persistent that *six years after* that initial blog post, Cutts made [an entire YouTube video just about punctuation in web addresses](https://www.youtube.com/watch?v=AQcSFsQyct8) on one of Google’s official channels. About 125,000 people have watched the whole video.

![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/type-keys-line.jpeg?v=1669782630628)

## Indexing the web, as it is

While the burgeoning SEO community was debating how best to please Google, amongst our team of people building a content management system, we were having a completely different philosophical debate: should we be trying to appease Google?

You see, the theory of how we felt Google should work, and what the company had often claimed, was that it looked at the web and used signals like the links or the formatting of webpages to indicate the quality and relevance of content. Put simply, your search ranking with Google was supposed to be based on Google indexing the web as it is.

But what if, due to the market pressure of the increasing value of ranking in Google’s search results, websites were incentivized to change their content to appeal to Google’s algorithm? Or, more accurately, to appeal to the values of the people who coded Google’s algorithm?

We found ourselves resistant to what felt like a coercive effect of Google’s rising domination, especially since Google’s own Blogger platform was a competitor of ours. Our expression of that frustration was expressed by a debate over a single character: We were using _ because we thought it looked nicer, so why should we change to - just because Google liked it better? Weren’t they supposed to adapt to what we published on the web?

## Holding the line

For a while, the team I was working on resisted changing our software to use dashes instead of underscores. My rationale was simple — Google has tons of money, why should we change the design of our tools for free, just to make things easier for a big company like Google? The WordPress community made a more pragmatic call, figuring (quite reasonably!) that users wanted to rank well in Google, they made sure their tool’s default was to use the punctuation that the search engine preferred.

At a literal level, the technical differences here were trivial. But the different choices of punctuation reflected very different philosophies about how the web should work. Dashes vs underscores represented a profound question: **Would we change our apps and our content to suit big companies like Google, or should those big companies accommodate us?**

![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/type-punctuation.png?v=1669782631376)

## Caving In

Eventually, most people who were publishing on the web said they didn’t want to do anything to risk diminishing their Google ranking, and our team had pretty much no choice but to switch to letting people publish web addresses using dashes. I genuinely felt like we had caved in. Caring so much about a single punctuation mark was, of course, an absurd hill to die on, but having Google coerce us into changing our software, and our aesthetics, felt like the first step toward a slippery slope of further concessions.

But the truth was even worse. Despite my misgivings about Google, I didn’t notice a more nefarious pattern that was established at the same time. A whole *community* had formed around trying to guess how Google’s algorithm worked, and that community very quickly built an entire infrastructure around reverse-engineering the algorithms that drive attention and popularity on the web.

Google was teaching us that the way to win on the web is to game the algorithms of big companies.

A few years later, Google [changed their mind](https://www.cnet.com/news/underscores-are-now-word-separators-proclaims-google/) and said we could use either dashes or underscores, and people should use whatever they want. But by then it was too late, we’d all already fallen in line.

---

## Finally, the algorithmic arms race

In that old era of the social web, the community’s shared knowledge of how to game algorithms was mostly used for harmless things. People would try to get more readers for their personal blogs, or pull off silly stunts like “Google bombing”, which was essentially just playing with getting a certain site to rank high in Google’s results for a particular term. It’s no wonder we thought it was no big deal if we changed our apps to make content that suited Google’s arbitrary rules. None of this stuff mattered *that* much, right?

But by attaching monetary value to search ranking, what Google ended up catalyzing was a never-ending arms race, where they constantly updated their algorithm and each community on the web constantly tried to learn how to exploit the new mechanics. The stakes of the algorithmic arms race kept going up; instead of being about pulling off silly pranks, understanding how to appease Google became the cornerstone of multi-million-dollar marketing campaigns. Instead of being about one character in a web address, it became about publishing content that suited the algorithm, whether it was true or not. At first, the only people paying attention were nerds making content management systems, then a broader audience of people trying to optimize their search engine positioning.

Eventually, though, movements across the political spectrum came to understand that knowledge of how to appease the algorithms that govern social media had profound social and cultural power. It wasn’t just marketers who figured out the best way to promote their ideas, it was trolls and activists and harassers and people on the fringes who wouldn’t have had any way to get the word out before—both for better and for worse. At that point, the rise of [fake media markets](https://medium.com/humane-tech/tech-and-the-fake-market-tactic-8bd386e3d382) was inevitable.

---

By the time we realized that we’d gotten suckered into a neverending two-front battle against both the algorithms of the major tech companies and the destructive movements that wanted to exploit them, it was too late. We’d already set the precedent that independent publishers and tech creators would just keep chasing whatever algorithm Google (and later Facebook and Twitter) fed to us.

Now, the challenge is to reform these systems so that we can hold the big platforms accountable for the impacts of their algorithms. We’ve got to encourage today’s newer creative communities in media and tech and culture to not constrain what they’re doing to conform to the dictates of an opaque, unknowable algorithm. We have to talk about the choices we made in those early days, even at risk of embarrassing ourselves by showing how naive we were about the influence these algorithms would have over culture.

And ultimately, we have to use the chance we’ve got now to underscore the lessons that we learned from the earliest days of the social web, that still resonate on billions of screens today. So much can come from a decision about just one character on the screen.

![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/type-curve-2.jpeg?v=1669782583099)
