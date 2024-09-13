---
title: Clay Feats
slug: clay_feats
date_published: 2007-02-09T05:59:46.000Z
date_updated: 2007-02-09T05:59:46.000Z
tags: [tech, blogs]
---

![Bring me the head of Clay Shirky!](http://www.dashes.com/anil/images/the-head-of-clay-shirky.jpg) A couple [Clay Shirky](http://www.shirky.com/) links for you today, one of which I just linked to, one of which I should have linked to last week, and all worth reading.

- [In Defense of Ready, Fire Aim](http://harvardbusinessonline.hbsp.harvard.edu/hbrsa/en/issue/0702/article/R0702A.jhtml#section19), a piece Clay wrote for the Harvard Business Review’s list of breakthrough ideas for 2007. I really am a sucker for the Annual Ideas Lists that more and more publications are putting out, but a few of the items in this list seem particularly valuable. I linked to Clay’s essay in [yesterday’s post about Yahoo Pipes](http://www.dashes.com/anil/2007/02/08/yahoo_pipes), referring to his concept of open source being based on a principal of embracing failure:

> In open systems, by contrast, the cost of failure is reduced, partly because less coordination is required among the various players and partly because each player is willing to accept some of the risks of failure directly. This means that worrying about whether a new idea will succeed is unnecessary; you simply try it out. The institutional barrier between thought and action—the need to convince someone that your idea is worth giving a whirl—doesn’t exist. The low cost of trying means that participants can fail like crazy as they continue to build on their successes.
> 
> In systems where anyone can try anything, the good has to be filtered from the bad after the fact. The cost of trying to prevent bloggers from saying stupid or silly things, for example, would be high, whereas the cost of allowing anyone to publish anything is low.

- A Clay Classic: [A Group Is Its Own Worst Enemy](http://www.shirky.com/writings/group_enemy.html). I was actually at the Etech conference where Clay delivered this speech; Stewart and Ben had just debuted Flickr a short while earlier, and the application was (at that point) a weird Flash community application that could do some image stuff in addition to working as an IM gateway. Clay was talking about group behaviors as exhibited on LiveJournal and The WELL and MetaFilter, with his points being especially relevant after the [recent Yahoo logins hubbub](http://www.dashes.com/anil/2007/01/31/i_am_okay_with_) on Flickr.

> This pattern has happened over and over and over again. Someone built the system, they assumed certain user behaviors. The users came on and exhibited different behaviors. And the people running the system discovered to their horror that the technological and social issues could not in fact be decoupled.

This passage is especially resonant after the launch of Pipes:

> We’ve gotten weblogs and wikis, and I think, even more importantly, we’re getting platform stuff. We’re getting RSS. We’re getting shared Flash objects. We’re getting ways to quickly build on top of some infrastructure we can take for granted, that lets us try new things very rapidly.
> 
> I was talking to Stewart Butterfield about the chat application they’re trying here. [Speaking of Flickr.] I said “Hey, how’s that going?” He said: “Well, we only had the idea for it two weeks ago. So this is the launch.” When you can go from “Hey, I’ve got an idea” to “Let’s launch this in front of a few hundred serious geeks and see how it works,” that suggests that there’s a platform there that is letting people do some really interesting things really quickly. It’s not that you couldn’t have built a similar application a couple of years ago, but the cost would have been much higher. And when you lower costs, interesting new kinds of things happen.

- [A response to Henry Jenkins about Second Life](http://many.corante.com/archives/2007/02/06/second_life_a_response_to_henry_jenkins.php). Clay has been taking a much-needed hard look at Second Life for some time, but I really am just linking to this because, as a student of social communication technology, Clay is uniquely qualified to create howlingly funny and yet still somehow polite and refined jabs at his debate partners. It’s like the world’s most dignified flame war. Witness:

> You compare Second Life with the Renaissance and the Age of Reason. This is approximately insane, and your disclaimer that Second Life may not reach this rarefied plateau doesn’t do much to make it less insane. Using the Renaissance as a reference point links the two in the reader’s mind, even in the face of subsequent denial.

- And then finally, as [Andre started experimenting with Arduino](http://notes.torrez.org/2007/02/hello_world.html) ([film at 11!](http://www.youtube.com/watch?v=LksGwjNsxZo&amp;eurl=)), who should pop up as the author of the source code for the [Dimming LEDs tutorial](http://www.arduino.cc/en/Tutorial/DimmingLEDs) but one Mr. Clay Shirky:

> /* * Code for cross-fading 3 LEDs, red, green and blue, or one tri-color LED, using PWM * The program cross-fades slowly from red to green, green to blue, and blue to red * The debugging code assumes Arduino 0004, as it uses the new Serial.begin()-style functions * Clay Shirky <clay.shirky> */ // Output int redPin = 9; // Red LED, connected to digital pin 9 int greenPin = 10; // Green LED, connected to digital pin 10 int bluePin = 11; // Blue LED, connected to digital pin 11 // Program variables int redVal = 255; // Variables to store the values to send to the pins int greenVal = 1; // Initial values are Red full, Green and Blue off int blueVal = 1; int i = 0; // Loop counter int wait = 50; // 50ms (.05 second) delay; shorten for faster fades int DEBUG = 0; // DEBUG counter; if set to 1, will write values back via serial </clay.shirky>

(Thanks to Cory Doctorow for the image.)
