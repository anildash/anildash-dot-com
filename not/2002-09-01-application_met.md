---
title: application metering APIs
slug: application_met
date_published: 2002-09-02T01:33:06.000Z
date_updated: 2002-09-02T01:33:06.000Z
tags: tech
---

Speaking of missed opportunities in programming interfaces, why don’t mainstream Windows applications support usage metering at the function level? Meaning, when I deploy Microsoft Office across my enterprise, I want each installed app to track which menu choices are selected, and how often, by my users. At the simplest level, I could use this information to inform my choices about customizing the default configuration for the suite when I install it. At a more advanced level, it would help me see which custom extensions were being used, and where future development efforts should be directed.

This information’s already being collected, of course. Office has supported personalized menus for some time now, as has the Favorites menu in Internet Explorer and the Start Menu in the Windows shell. But there don’t appear to be any public APIs for administrators to view or access this information.

Yeah, yeah, privacy implications. Except that most business users don’t really *have* any privacy rights in regard to their usage of their desktop application suite. We’ve already got crash reporting, in Mozilla and IE and for Windows XP and Office XP. Extend that reporting button to copy crash data to network admins as well as to Microsoft, and then add in features for reporting on what 20% of Office that particular enterprise’s users work with.

Maybe I’m just spoiled, but this is one of the types of measurements that web apps do really well, and it’s also one of the few platform options that Office wasn’t ten years ahead of the web in developing, so I think developers have gotten used to having this sort of data available to help them make decisions. Amazon’s platform supports it, why doesn’t Office?
