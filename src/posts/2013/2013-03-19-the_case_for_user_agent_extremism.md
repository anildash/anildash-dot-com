---
title: The Case for User Agent Extremism
slug: the_case_for_user_agent_extremism
date_published: 2013-03-19T15:20:02.000Z
date_updated: 2013-03-19T15:20:02.000Z
image: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/medium_f785c8ecc86771db3afec31e66872d55.png?v=1670477235331
tags: [web, software, tech]
---

One of my favorite aspects of the infrastructure of the web is that the way we refer to web browsers in a technical context: User Agents. Divorced from its geeky context, the simple phrase seems to be laden with social, even political, implications.

The idea captured in the phrase “user agent” is a powerful one, that this software we run on our computers or our phones acts with agency on behalf of us as users, doing our bidding and following our wishes. But as the web evolves, we’re in fundamental tension with that history and legacy, because the powerful companies that today exert overwhelming control over the web are going to try to make web browsers less an agent of users and more a user-driven agent of those corporations. This is especially true for Google Chrome, Microsoft Internet Explorer and Apple Safari, though Mozilla’s Firefox may be headed down this path as well.

Traditionally, the ostensible protection against browsers undermining the agency of the user has been that some of the most popular browsers (Firefox, Chrome, Safari’s browser engine) are open source, and could thus be prevented from being subverted by their corporate owners because technically-savvy users could wrest control of the code from their sponsors. What’s more, *all* popular desktop browsers have supported some form of user scripting, whether that’s in the form of plugins (which began to wane in importance a decade ago), extensions and add-ons (in Firefox and Chrome, notably) or in the form of bookmarklets which let arbitrary scripts run on pages in almost every browser.

That era of truly effective user control over user agents may be rapidly ending, for a few reasons:
![](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/medium_f785c8ecc86771db3afec31e66872d55.png?v=1670477235331 "UI for choosing between user agent strings")

- Legitimate security and performance issues have led to the death of the traditional browser plugin; Flash was perhaps the last successful browser plugin that will ever exist. As browsers get tied more deeply to operating systems and those operating systems try to lose their dependencies on particular chip architectures or system designs, plugins implemented as native code are rapidly being obsoleted.
- Increasingly large parts of the core functionality of browsers is being connected to the cloud infrastructure of the companies which create the browsers. From bookmark sync in Chrome and Safari and Mozilla to past and future efforts around browser-integrated authentication by Microsoft and Mozilla, more and more of the features we use to browse the web are plugged in by default to centralized web services. Today’s browsers can certainly function *without* signing in to those services, but increasingly that level of convenience will be expected from any browser expected to compete.
- The move to mobile has gutted the formerly-ubiquitous forms of browser control and customizability that we used to take for granted. No popular web browser supports plugins, almost none support any form of extensions or add-ons, and it’s virtually impossible to install even a simple javascript bookmarklet on common mobile browsers like Safari and Chrome.
- Google, Apple and Opera have all coalesced around the extremely popular (and currently very technically strong) Webkit browser engine, which is overwhelmingly dominant in mobile web browsing. As we’ve seen, a browser engine gaining over 90% share in a market leads to technological stagnation ranging from insecurities to less innovation in terms of customizability. It’s possible the three (well, two and a half) competitors all relying on the platform will be enough to keep it moving forward, but that’s far from certain.

### Secret Agents

Though this sounds alarmist or like a dire consequence, for the most part these developments aren’t egregiously bad news for the web or for consumers. In exchange for these compromises, we’ve seen enormous advances in browser performance, standards-conformance and capability. The centrally-connected services like bookmark synching are generally easily disabled, and not particularly intrusive even when enabled. Competition has pushed platforms forward enough that even the formerly-reviled Internet Explorer can make knowing jokes at the expense of its old versions since new ones are quite good.

But the idea that a browser can be controlled by a user is still fundamentally in danger. Google just [removed the Adblock Plus extension](https://www.eff.org/deeplinks/2013/03/google-censoring-android-apps) from its Play store for Android devices. This isn’t that surprising — an advertising company is prohibiting the distribution of an extension that blocks advertising. But it starts to highlight the larger issue that the straightforward ability to have user agents be, well, agents for users is now being mediated through the business concerns of the companies which create the browsers.

**We need to be advocates for extremism in the name of user agent empowerment.** There should be no constraint about what user agents can do on our behalf to present, transform, remix, combine, format, reformat and display the content we view on the web. If we want to make a browser or browser add-on that strips away ads from a page, that’s our right. If I want to have a browser show everything in black and white? Let me as the user have that agency. Print everything upside down and in blinking text? Absolutely. Transform every mention of “the cloud” into the phrase “[my butt](https://github.com/panicsteve/cloud-to-butt)“? You bet your… well, you know.
[![Office 365](http://farm9.staticflickr.com/8383/8560876058_64bdc15d44_c.jpg)](http://www.flickr.com/photos/brucedene/8560876058/)

### Agency Matters

Why is this important? Aren’t these examples just trivial transformations of content? Doesn’t the existence of a “Cloud-to-Butt” extension prove that these concerns are overblown? Not necessarily.

First, distribution matters when it comes to browser customizations and add-ons. Easily being able to install an add-on changes the fundamental impact that the code has on user experience as compared to something theoretically being possible. Google and others saying “well, you can distribute that plugin, but not through a method integrated into the browser” is the difference between a piece of code being a feature for normal people or it being an art project. This is the same issue we see with app stores, but with the added impact of actually impacting the open web — the same open web that’s supposed to be the *alternative* to the wrongs of those app stores.

Second, if we follow the historical pattern of these advancements in other areas of the tech industry, we’ll see the big tech companies capitulate to the desires of the legacy content industry to trump IP law and practice with private contracts that constrain our legal rights around content use and transformation. We’ve had our right to make backup copies of our own media in formats like DVD criminalized by their actions. We’ve seen the ability to route video streams to our own devices constrained by HDCP, again limiting our ability to make our own copies of content or to transform or sample that content in ways that are legally permitted.

It is obvious that the biggest companies which make web browsers all want to curry favor with media companies on the web in the same way they curried favor with those media companies in video and music.

Google, Apple and Microsoft each share a few traits:

- They want to prove they’re the biggest friends to big media companies.
- They each have advertising businesses they don’t want users to block.
- They each already enforce HDCP and other technical constraints that take away IP rights that citizens have always had.
- They each have closed app stores which they heavily moderate to decide which forms of customization are permitted on their platforms.
- They have each hemmed in even powerful third-party platforms like Flash, taking control over distribution and implementation of the most popular extensions/customizations.

There is no reason to believe that web browsers won’t start to aggressively block capabilities that historically have been assumed to be part of user agents. We can expect messages like “this page prohibits printing for non-registered users”, or “You don’t have sufficient permissions to click the ‘Pin It’ button for Pinterest on this site”, or “unauthorized bookmarklet detected; content from this site is blocked”.

### How It Happens

[![Join EFF!](https://www.eff.org/sites/default/files/eff-join.png)](https://www.eff.org/join)

Here’s where the Pollyannas in the tech industry, or those too young to have seen how the patterns repeat, say with faith and certainty, “That won’t happen! My favorite browser is open source!” But imagine if this same set of features were marketed by a smart communications team at one of these companies. Instead of saying “our browser shuts off the print button”, they say “we offer a pay gate feature with deep integration into the browser for subscribers”. Instead of saying “We neuter competing social networks by disabling their sharing buttons” they say “We’ve launched a preferred partner program to enable deep browser integration from a set of verified social networks that offer the features our users want”. Instead of saying “We block content from displaying if you haven’t signed in with our cloud service and had your extensions approved by us”, they say “Customers who sign in with their account get access to exclusive content from our partner sites.”

Hey, the friendlier phrasing sounds pretty familiar, right? That’s not evil at all! Except that it’s the *exact same constraint* being introduced to your web browser, presented in a much more appetizing way. Think of how indispensable features like Instapaper or Pocket or Readability are on mobile browsers. Now understand those are seen as problematic exceptions to the model that Apple (and Google, and everyone else) would prefer to see for mobile browser usage. There’s no technical reason that Adblock couldn’t be enabled on mobile versions of Safari, and doing so would allow that community to begin optimizing its performance for mobile devices. Does anybody think that will *ever* happen?

So, I’m a user agent extremist. We should work constructively together within the tech community (perhaps led by the EFF) to create a list of capabilities in web browsers and user agents that we consider inviolate. We should take language that ordinary consumers understand, like “unlocking” in the context of a mobile phone, and apply it to our browsers. Then we can propose simple guidelines that should be enshrined in policy — every web browser should be “unlocked” by default. We need to educate all three branches of government at federal, state and local levels to expect that media companies are going to start prosecuting ordinary citizens for using user agent capabilities that we’ve taken for granted for twenty years.

Otherwise we can soon expect to find that the “View Source” button which has enabled the web so far is mysteriously grayed out on certain sites. Because there are companies that are going to realize that giving users agency is a really powerful thing
