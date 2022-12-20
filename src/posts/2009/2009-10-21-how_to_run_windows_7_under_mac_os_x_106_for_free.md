---
title: How to run Windows 7 under Mac OS X 10.6 for free
slug: how_to_run_windows_7_under_mac_os_x_106_for_free
date_published: 2009-10-22T03:34:52.000Z
date_updated: 2009-10-22T03:34:52.000Z
tags: tech
---

**Update:** Since this post got a lot more readers than I expected, it’s become clear to me that the title was unintentionally vague. I thought it’s amazing that a technology I still think of as fairly advanced, virtualizing operating systems on the desktop, has become commoditized enough that free, open source tools are very mature. When I said “for free” here, I meant that virtualization is available at no cost, not that Microsoft’s giving Windows licenses away for free. Sorry for assuming that was obvious!

Pardon the uncharacteristically nerdy post, but I thought I’d write up a handy way I’d found to run Windows 7 in a seamlessly-integrated virtual machine under Mac OS X 10.6. I started with these basic components:

- A MacBook running Mac OS X 10.6.1 (Snow Leopard)
- A license for a full install of [Windows 7 Ultimate](http://www.amazon.com/gp/product/B002DHGMVY?ie=UTF8&amp;tag=2020-20&amp;linkCode=as2&amp;camp=1789&amp;creative=390957&amp;creativeASIN=B002DHGMVY)
- [VirtualBox 3.08](http://www.virtualbox.org/) for Mac OS X

If you’re like a lot of geeks that I know, you have a Mac as your main machine, but often need to drop into Windows to check things like browser compatibility or to use some particular Windows applications. I happen to just really like Windows 7 (it’s on par with Mac OS overall for me, with some parts being better, such as the Windows Taskbar being much better than the Mac’s Dock, and of course some parts being worse.) Some of these instructions may be obvious, but I hadn’t seen a writeup anywhere, so here goes.

Here’s what you’ll need to do:

# Install Windows 7 under [Boot Camp](http://www.apple.com/support/bootcamp/), following the normal instructions. All of the Vista drivers for Boot Camp worked fine for me, and the install was actually pretty quick.

# Download and install [VirtualBox](http://www.virtualbox.org/). This is an open source virtualization system that runs on Mac OS, a lot like Parallels Desktop or VMWare Fusion, but available for free.

# The tricky part: You’ll need to do a little bit of geeky stuff. First, eject the Windows boot camp disk in Finder. (It’s usually called “Untitled”.) Then, launch Terminal so you can enter two commands.

** `sudo chmod 777 /dev/disk0s3`

** `VBoxManage internalcommands createrawvmdk -rawdisk /dev/disk0 -filename win7raw.vmdk -partitions 3`

# Start up VirtualBox, make a new Windows 7 machine, and browse to `win7raw.vmdk` in your home directory to choose the virtual hard drive for the machine. Your Windows install should boot up. It’ll fuss for a little while as it installs new drivers.

# Once that’s done, you can optionally install the [VirtualBox Guest Additions](http://code.google.com/p/virtual-box-windows-guest-additions-installer/downloads/list) software to let your Windows install completely integrate with your Mac OS X environment.

While it’s not quite as seamless as some of the paid alternatives out there, I’ve found it was very easy to do (under an hour total, and only 15 minutes or so if you already have Windows installed), works very well, and is speedy enough to use regularly.

As always, your mileage may vary, and comments or corrections or feedback are welcome. I was too lazy to do screenshots of the whole process, but if you want to turn this into a complete gadget blog-worthy writeup, I’ll be happy to link to it. If you *really* liked this how-to, you can [buy WIndows 7 from Amazon](http://www.amazon.com/gp/product/B002DHGMVY?ie=UTF8&amp;tag=2020-20&amp;linkCode=as2&amp;camp=1789&amp;creative=390957&amp;creativeASIN=B002DHGMVY) and I’ll make a few bucks.
