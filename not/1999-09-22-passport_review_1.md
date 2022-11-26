---
title: Passport Review Continued
slug: passport_review_1
date_published: 1999-09-22T16:00:01.000Z
date_updated: 1999-09-22T16:00:01.000Z
tags: tech
---

### Microsoft Passport Part One and a Half:

Continuing the User Experience

At the end of yesterday’s exciting episode, **User X was waiting**, mouse-finger poised, to click on our "Sign In" link… let’s see where the story continues!

The sign in graphic is a standard Passport graphic, probably pulled from the user’s cache, because all links to the graphic are **from the passport server**.

![Passport Sign In](images/passsignin.gif)

Our user already has a Passport profile, since they use Hotmail. However, the potential for **discord in our harmonious user experience** begins here, as the "standard" Passport screen is provided by Passport’s server.

The screen will likely be familiar to the user, since they are aware of the technology already. However, no **visual continuity** between your site and passport’s will be maintained, save for any stylistic cues you can provide to passport through **CSS**. If you’ve got a "Step *X* of *Y*" at the top of your checkout screens, or a progress meter, or even your site-wide navigation, say goodbye. **Yuck.**

Completion of the sign in brings another **complete change to user interface**, as the Passport cookie is written to the user’s machine, and they are returned to the environs of your site.

### The Passport is Stamped

At this point, if it’s a simple protected area on the site, they are likely at the main menu of your proprietary content. If it’s a commerce situation, they are likely at the checkout stage, with Passport having **passed their credit card data, etc. securely to your form**. This is a nice benefit, but the ping-ponging of screens might be a bit off-putting to users **who already tend to be leery about online purchasing**.

In fairness to the concept, it should be pointed out that there are provisions for a site to customize the Passport screens to a degree. Though Microsoft describes this as "co-branding", it doesn’t seem to be nearly as pervasive as that label would suggest.

Basically, two rectangular areas are provided where the Passport page will optionally include whatever JavaScript you tell them to write to the page. If you used a lot of floating layers and DHTML, you might be able to pretty convincingly redraw your page design onto the Passport page, but it would be a hell of a lot of work, extremely slow, and wouldn’t work in most browsers.

**On the upside**, users might become accustomed to the Passport sign in if it became sufficiently ubiquitous, and you might even be lucky enough to encounter a user who had already signed in to Passport during that browsing session, which would make the whole process invisible on your site.

In either of those cases, being able to include your logo on the standard sign in screen would be valuable, but it remains be seen whether the tradeoff in design flexibility will result in overall usability gains.

![Passport Sign Out](images/passsignout.gif)

### Conclusion

If you’ve got content worth signing in for, or a product worth paying for online, you’ve probably **already got a registration system in place**. Then switching over to Passport authentication would probably **not be worth the time and expense**. However, if you have a new client with concerns about implementing registration, Passport may be worth your consideration.

Whether to consider Passport for user sign in is mainly a concern of whether:

1. Your users are **sufficiently sophisticated** in their knowledge of the web to deal with the interface changes when moving from your site to Passport sign and back;
2. Your users would be comforted or reassured by seeing a Microsoft technology when dealing with their private and/or financial information;
3. A sufficiently large percentage of your audience could be expected to already have Passport accounts, either through being experienced web-surfers, or by having a large overlap between your audience and, for example, Microsoft’s [Money Central](http://www.moneycentral.msn.com) site, which uses the Passport registration.

### The Bottom Line

Are we all going to get our Passports stamped? **Probably not**. I suspect Passport will remain, at least for the near future, a convenient way of getting between various Microsoft sites that we all deal with to one degree or another. On the other hand, I’m sure I, and others, will have **tests or trial implementations** of the technology in the next months, and the results of those tests will determine the success of the entire effort.

**Note:**Passport Part Two: Passing Through Customs, about the technical aspects of the system has been canceled by me because it’s too damn boring.

**Extra Credit:** Bonus points to whomever is the first to point me to an **open-source implementation of Passport**, the protocols are open enough that implementation should be nearly academic for experienced code hackers. Passport for Apache, anyone?
