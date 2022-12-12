---
title: The Decade-Long Campaign to Lock Down Your Computer
slug: the_decade-long_campaign_to_lock_down_your_computer
date_published: 2012-05-29T20:36:11.000Z
date_updated: 2012-05-29T20:36:11.000Z
tags: [tech]
---

This month’s Wired magazine includes a milestone I’m incredibly excited about: **My first published print column!** You can read [Safe In Its Shell](https://www.wired.com/2012/05/opinion-dash-applesecurity/), my exploration of the long history of introducing software lockdown mechanisms to mainstream computer operating systems. I keyed on the Gatekeeper feature in Apple’s upcoming version of OS X which locks down which applications can run on your computer, and how it uses a method that was first broadly described by Microsoft as part of its Trustworthy Computing efforts a decade ago.

I’m happy with how the piece came out (I’ve never worked with an editor before!) but I thought that, before I republish the piece on my own site, I’d share some of the key resources that I found valuable in understanding the ideas which informed by column.Put another way, if that column were a movie, these are the DVD extras.

## Microsoft’s History With Palladium

Microsoft’s “Palladium” effort to begin providing a framework for software security that was controlled by the software behemoth inspired an immense amount of controversy from the moment it was announced. Some key resources:
- Microsoft did a [briefing at NIST in 2002](http://epic.org/privacy/consumer/microsoft/nistpalladium.pdf) about the basic principles behind Palladium
- The [original Newsweek launch story about Palladium](http://www.thedailybeast.com/newsweek/2002/06/30/the-big-secret.html) by Steven Levy is still up on the Daily Beast website
- And you can still find the [original “Trustworthy Computing” memo by Bill Gates](http://www.microsoft.com/about/companyinformation/timeline/timeline/docs/bp_Trustworthy.rtf) (in RTF format!) which acted as a rallying cry for the troops at Microsoft. (Looks like they added [an HTML version](http://blogs.technet.com/b/security/p/twc-mail.aspx) as well.)
- And of course, Gates’ memo was inspired by Craig Mundie’s [original TrustWorthy Computing memo](http://download.microsoft.com/download/a/f/2/af22fd56-7f19-47aa-8167-4b1d73cd3c57/twc_mundie.doc) (in convenient Microsoft Word format), which Mundie revisited on its 10th anniversary in [a retrospective writeup](http://blogs.technet.com/b/security/p/twcnext-mail.aspx)
- I’d written a bit about that original Trustworthy Computing memo [a few years ago](/2010/11/freedom-trust-and-other-boring-software-features.html) myself
- Microsoft still has an active [Trustworthy Computing site](http://www.microsoft.com/about/twc/en/us/default.aspx) which offers a [detailed timeline](http://www.microsoft.com/about/twc/en/us/twcnext/timeline.aspx) on the initiative, and presages their later site about the mellifluously-named successor program, the  [Next-Generation Secure Computing Base](http://www.microsoft.com/resources/ngscb/default.mspx)
- And though it’s apparently no longer on Microsoft’s site, the intense scrutiny of the original responses is evident in [this cached version of Microsoft’s original Palladium FAQ](http://www.napolifirewall.com/MicrosoftPalladium.htm)

## The blowback to the Palladium announcement in 2002:

Lots of folks took exception to Palladium’s announcement. Some highlights from the time:

- [David Coursey, then of ZDNet](http://www.zdnet.com/news/why-we-cant-trust-microsofts-trustworthy-os/298837), explains why the effort couldn’t be trusted
- The Register called it [an attempt to eradicate the GPL and destroy Linux](http://www.theregister.co.uk/2002/06/25/ms_to_eradicate_gpl_hence/)
- Robert Cringely naturally deemed it “[diabolical](http://www.pbs.org/cringely/pulpit/2002/pulpit_20020627_000433.html)“
- [Chris Hoofnagle from EPIC](http://www.internetnews.com/asp-news/article.php/1378731/Is+Microsofts+Palladium+a+Trojan+Horse.htm) described Microsoft’s Palladium presentation as “Orwellian”
- Microsoft exec Mario Juarez [did an interview on Palladium](http://www.mail-archive.com/cryptography@wasabisystems.com/msg02267.html) in June 2002
- And [Security Focus had a contemporary story](http://www.securityfocus.com/columnists/93) at the time of Palladium’s launch
- EPIC naturally offered some [detailed resources about Palladium](http://epic.org/privacy/consumer/microsoft/palladium.html).
- Catherine Flick at the University of Sydney offered a detailed analysis in her [June 2004 paper](http://liedra.net/misc/Controversy_Over_Trusted_Computing.pdf)
- Ross Anderson’s [2003 FAQ](http://www.cl.cam.ac.uk/~rja14/tcpa-faq.html) was also a seminal resource
- Microsoft then [started to back off of Palladium](http://www.crn.com/news/security/18841713/microsoft-shelves-ngscb-project-as-nx-moves-to-center-stage.htm) (by then rebranded as “NGSCB”), as also mentioned [Ars Technica](http://arstechnica.com/old/content/2004/05/3736.ars)
- Naturally, Microsoft immediately backtracked, vaguely [reaffirming its commitment to Palladium](http://www.microsoft-watch.com/content/operating_systems/microsoft_palladium_is_still_alive_and_kicking.html) shortly thereafter

## Apple resources on Gatekeeper

Meanwhile, Apple’s rollout of Gatekeeper has been very deliberate, and fairly low-key:

- [A characteristically understated consumer explanation](http://www.apple.com/macosx/mountain-lion/security.html) of Gatekeeper offers up Apple’s only real customer-facing description of the feature:

> “Advanced features in OS X already help protect you from malware no matter where you download apps. Gatekeeper brings you even more security options — and even more control. For maximum security, you can install and run only apps from the Mac App Store. You can choose to install and run apps from the Mac App Store and apps that have a Developer ID. Or you can install all apps from anywhere, just as you can today. You can even temporarily override your setting by Control-clicking, and install any app at any time. Gatekeeper leaves it all up to you.”

- Rich Mogull (what a great name!) [offered a detailed overview of Gatekeeper’s functions](https://securosis.com/blog/os-x-10.8-gatekeeper-in-depth) and also [summarized the feature in Tidbits](http://tidbits.com/article/12795)
- Steven Frank [had a thoughtful take on Gatekeeper](http://www.panic.com/blog/2012/02/about-gatekeeper/)

> “I have a personal flaw in the form of a small conspiracy theorist who lives in my head. He worried that this may have been created as just a temporary stepping stone — like Rosetta for the Intel transition, or Carbon for the OS 9 to OS X transition — and that one day, the Mac App Store-only option might still be enforced.
> 
> But I can’t find it in me to disparage this goodwill effort that Apple has undertaken to not turn every third-party developer upside-down with regard to app distribution. To me it’s a great sign that they’re aware and at some level sympathetic to our concerns, while remaining committed to a high-security experience for users.”

## SmartScreen in Windows 8:

Finally, the new SmartScreen features in the upcoming Windows 8 bring the whole thing full circle:

- Where does any discussion of a new Windows feature start except with [how to turn the damn thing off](http://www.howtogeek.com/75356/how-to-turn-off-or-disable-the-smartscreen-filter-in-windows-8/)?
- Microsoft [describes the code-signing requirements at the OS level](http://blogs.msdn.com/b/b8/archive/2011/09/22/protecting-the-pre-os-environment-with-uefi.aspx) on their developer site
- The great Windows fan site I Started Something [goes into great depth](http://www.istartedsomething.com/20110408/windows-8-to-feature-native-smartscreen-file-checking/) about how the SmartScreen controls actually work in the new OS

This first Wired column was a great experiment for me in learning how to write without hyperlinks, but I’m enjoying the process greatly and hope that sharing some of the links *behind* the piece make it even more interesting.
