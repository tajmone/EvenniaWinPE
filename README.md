# EvenniaWinPE

Beta 2 :: 3rd March 2015 ( Evennia 0.5.0 )

Size on disk: 215Mb (zipped 40mb)

Runs out of the box on Windows 32/64bit

Tested on Win7 64bit (should work with XP SP3, not sure about earlier versions of Windows).

Evennia homepage: <http://www.evennia.com/>

Evennia on GitHub: <https://github.com/evennia/evennia>

> NOTE: Beta 2 includes the major March update of Evennia (0.5.0). This new release of Evennia brings important changes to Evennia in code and structure, breaking backwards compatibility to some extent—migration of old code only requires some simple tweaks on the user side though! For more information read:

> <https://groups.google.com/forum/#!topic/evennia/6ug7m872GIk>

> <https://groups.google.com/forum/#!topic/evennia/RDYoDUuxcWI>

## Evennia for Windows Portable Edition

> Evennia is an open-source library and toolbox for building multi-player online text games (MUD, MUX, MUSH, MUCK and other MU\*). You easily design your entire game using normal Python modules. Apart from supporting traditional clients, Evennia comes with both a game web-client and a web-server out of the box.

EvenniaWinPE is an out-of-the-box solution for MS Windows: unzip and run it. No Python installation required; no alterations of Windows' registry or paths—nothing! It also contains a standalone features-rich MUSH client.

-   **NOTE**: It must be unzipped/placed in **root of drive C** [ C:\\EvenniaWinPE\\ ].

## Why Portable?

While serious commitment to working with Evennia commends a wiser approach than any out-of-the-box solution might provide (a proper Python installation, proper working tools, and so on); one can think of many good reasons for needing a quick-but-clean solution in everyday life:

-   **Try-before-you-buy** — maybe you just want to give Evennia an explorative go before commiting to install anything on your computer. Understandable! Don't turn your back to Evennia then: here is a 5-minutes-to-go solution. Give it a try, you can always delete its single-folder and carry on with life.

-   **Multiple PCs dilemma** — beside your regular state-of-the-art working PC you own a NetBook, have an old PC at the countryside manor, etc. Sure, not even the best developer needs to duplicate configurations over every PC owned. One well setup computer is enough—for the rest there is Evennia in Portable Edition.

-   **Showing around your MU\* work** — you just feel better knowing that in your pocket there is a zipped file that you can pull out at any moment, plug it into your friends/customers PC and show them a live copy of your amazing Mud/MU\*—and who knows ... maybe you'll make your mark on that beauty that you need so badly to impress.

-   **Life can be boring/it's too short** — Maybe your boss doesn't realize how serious MOOing and MUDing can be: he calls it «playing» and (knowing your compulsions) he blocked any installation privileges on your workplace PC. Portable Edition comes to your aid: unzip it to the hard drive and you can start playing/working with all Evennia's features during workhours (at your own risk). When you're done, just copy/zip EvenniaWinPE folder back to your USB stick and delete the local copy — no visible traces behind, and none of your work is lost!

-   **It's easier (and you're lazy)** — Nothing wrong with that. MOOing and MUDing should be fun, not tedious.

-   **It sounds difficoult (and you're scared)** — Nothing to be ashamed of; and not a reason to give up! Everyone started somewhere, no one was born a Python Guru. Newbies will benefit from EvenniaWinPE because during boot it prints on the terminal screen a detailed résumé of all the operations talking place in the background (explaining how you could have done it manually from the shell). Seeing the right way a multi-software package runs equals learning how to do it by example.

Whatever your reasons, the solution is here.

## Features

All features have been kept as close as possible to Evennia's adviced settings (as of February 2015).

### Packages versions

-   Evennia 0.5.0 ( as of 3rd March 2015 )

-   PortablePython 2.7.6.1

    -   pip 6.0.8

    -   pypiwin32-219

    -   virtualenv 12.0.7

-   Django 1.7.5

    -   Pillow 2.7.0

-   Twisted 15.0.0

    -   zope.interface 4.1.2

-   MUSHclient 4.94

### Functionalities

-   Single shortcut to start Evennia Server+Portal

-   Evennia fully installed and ready to use

-   Superuser account already setup (no changes made to the world environment)

-   Server boot-up with onscreen tutorial-notes

-   MUSHclient preconfigured to autoconnect to Evennia at startup

-   Evennia official documentation (PDF format) as of 19th Feb 2015

-   Extra tools and documents (not much yet, but more to come)

## FAQ

**Will EvenniaWinPE conflict with my Python installation?**

No, it wan't: EvenniaWinPE runs within a virtual environment on top of Portable Python, which is an isolated application. Even if you have Python 3 installed you'll experience no conflicts.

**Will my firewall prevent me from using EvenniaWinPE?**

It could. Depending on the privileges you own on the system, its configuration and what security software it's installed on it, you might just need to confirm approval in an alert window, or it might require you to fiddle with firewall software settings. EvenniaWinPE works on localhost (127.0.0.1) and will not attempt to go over the Internet (unless you explicitly configure it to do so).

**Can I unzip it anywhere on my hard drive?**

No, unfortunately it has to be placed in the root of drive "C:"; otherwise it's going to "break" (no risks for the host computer, it simply won't start). There are various reasons for this, amongst them the fact that I didn't want to spent weeks setting it up for working with relative paths (it might be achivable, but it also might breakup if you update Python packages afterwards). It might seem a bit of a take-it-or-leave-it situation, but there is no reason why you shouldn't unzpit in drive C. When you're done with EvenniaWinPE you only have to trash away its folder; it won't leave any garbage behind. Another reason has to do with the differences amongst the various MS Windows versions. I wanted to make sure that EvenniaWinPE would run on older 32bit versions of Windows (XP, maybe even NT) as well as Win7/8 64bit.

**Why is it in Beta? Is it buggy/unsafe?**

Could a derivate of a beta software ever be in final release? Since Evennia is still in Beta stage EvenniaWinPE is also in Beta. Even though Evennia is mature (and well documented) enough to be employed in actual projects; its author might introduce at any time major changes that could conflict with this edition of EvenniaWinPE, making it unusable in the future. Apart from this, soo far all tests with EvenniaWinPE went well. But more feedback from users is needed before making big promises.

**Does EvenniaWinPE self update?**

No, it doesn't (yet!). But since all you need to update is the Envennia folder, you can easily track updates from GitHub via Git for Windows (also available in portable format). Updating your local Evennia files works just like with any other Evennia installation. Consult Evennia's Wiki on this topic. As for EvenniaWinPE's specific files, future updateds (if any) might come as patches (to be unzipped on top of your pre-existing local copy). Just be aware that if you decide to Git both EvenniaWinPE *and* the copy of Evennia it contains inside, you'll be dealing with nested Gits (submodules). EvenniaWinPE's internal copy of Evennia's repository is *not* gitted by default!

**What MUD will I find inside EvenniaWinPE?**

None. You'll find the standard empty world which comes by default with Evennia. You'll have an out-of-the-box set of Mux-like standard commands to start building your Mud right away, plus the usual tools and functions a Mud needs. There are some example scripts and a tutorial with a small adventure which you can load into Evennia with a single command: you can start by playing that and get a feeling of the experience.

**Can I use EvenniaWinPE to share my Mud online?**

Not a got idea. EvenniaWinPE was not build with Internet security in mind at all, it's meant for experimental and personal use. Securing a personal computer for serving contents online requires special considerations and skills which are not related or confined to Evennia or EvenniaWinPE. Aside of this, nothing within EvenniaWinPE prevents you from doing it (at your own risk).

**Will EvenniaWinPE work with future versions of Evennia? Are you going to update it?**

Who knows. Difficoult to tell right now because Evennia is still in its alpha stages (even though it's fully operational and stable). If you ever experience compatiblity issues, drop me an email—keep in mind that I actually work on a full Python installation, not on EvenniaWinPE. I've created this package for the benefit of those who might need it, and to promote Envennia—and as a lifesaver for boring parties: I can now just grab the first laptop I find, hide in the lavatory and get MOOing until the party is over.

**Could I have feature-X added to EvenniaWinPE?**

Consider contributing it to the project yourself (see below). If you have a great idea that you can't implement yourself email me and let me know.

**How can I contribute to this project?**

Simple: clone and fork it on GithHub! Or email me (be warned: I'm no prompt replier when it comes to emails). If you fork EvenniaWinPE be kind and let me know about it, I'd be happy to see that my efforts were of inspiration to others.

**Is this an official Evennia product? Are you an Agent at the service of Evennia Ltd?**

No, Evennia Windows Personal Edition is a personal project of mine. For all the benefits you'll get from Evennia you should thank Evennia's author (Griatch). As for any shortcomings and/or bugs in EvenniaWinPE, the blame is all mine. I don't work for Evennia and there is no Evennia Ltd/Inc. Evennia is a free project; so it's my contribution of this package.

**Why is it free? What's the catch?**

It's *free* as in a *free world*, were people freely share (*free* as in *a free smile*). In the computing world, proprietary patented commercial software is for the exclusive benefit of the haves. Free software is for the benefit of the haves and havenots alike (*free* as in *free for all*). Python (the foundation language of Evennia) is a *free* language (free to use and share). Evennia is free, so is PythonPortable—all of which made EvenniaWinPE possible. Freedom is the foundations of a civilized society. No one will ever coerce you to use EvenniaWinPE!

**What about ... ?**

What about you just download it and try it yourself?! Inside the package you'll find more useful documentation which is likely to answer most of your questions. You're just one click and five-minutes away from logging into Evennia. If you've read all of this README file, just be aware that it took you more time than required to get EvenniaWinPE up and running.

## License

All the code and files within EvenniaWinPE which were created by me are released as public domain (unrestricted). As for all the third-party software and files included in EvenniaWinPE see their original licenses (included) which came with them.
