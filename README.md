<<<<<<< HEAD
# Free And Open Source SEO Software
<<<<<<< HEAD
=======
========
>>>>>>> 029f7aac5ac943d4ffcae4dbff76e2a017ebd25e

Pipulate expands your mind... and the way spreadsheets work by using functions
written and executed in Python entirely outside of the spreadsheet, cleanly
passing the values back and forth, replacing question marks for output. This
approach facilitates quick data-investigations from the comfortable of your own
spreadsheet&#151;effectively slapping an Ironman suit onto aspiring SEO or
Social Media professionals to give them superpowers. Watch the 
[Google Slides](http://goo.gl/v71kw8) and visit the sister-project,
[Levinux](http://levinux.com).

<<<<<<< HEAD
## Table of Contents

 [Installation](#2-installation)
    - [Runs On Anything](#runs-on-anything)
    - [Debian/Ubuntu](#debian-ubuntu)
    - [Mac OS X](#mac-os-x)
    - [Windows](#windows)

 [Conventions](#3-conventions)
    - [Drag to Bookmarks Bar](#drag-to-bookmarks-bar)
    - [Create New Spreadsheet](#create-new-spreadsheet)
    - [Clicking The Bookmarklet](#clicking-the-bookmarklet)
    - [Logging In](#logging-in)
    - [Initializing Sheet](#initializing-sheet)
    - [The Tabs](#the-tabs)
    - [Function Names](#function-names)
    - [Input Columns](#input-columns)
    - [Question Marks](#question-marks)
    - [Ad Hoc Investigations](#ad-hoc-investigations)
    - [Grab Links](#grab-links)
    - [Stormy Weather](#stormy-weather)

## 1\. Introduction
### Overview
Well, you pretty much got the overview in that opening paragraph, no? At any
rate, I connect a lot of unexpected dots here in this project, from Python, to
bookmarklets, to tiny servers, to leveraging massive Web API
infrastructure&#151;all in order to achieve great things. My main lesson is:
"Don't care about how much conventional wisdom dictates a thing, if you have
good reason to believe otherwise". My reasons? Oh, they amount to:

1. Master a minimal set of parts that let you achieve the most things.
2. Choose parts that are as disruption-proof as reasonably possible.
3. Do something interesting and useful that nobody's done before.
4. Design it so you'll actually want to use every single day.
5. Make it as approachable by newbs as possible.

### Project Background
I've been at this since 1994 with Microsoft idc/htx files, which is pretty much
when Web-accessible databases first became accessible to hackers like me that
haven't taken the plunge into Linux yet. The system has undergone many
iterations, becoming very Ruby-on-Rails-like long before ROR ever hit the
scene. But I'm not a compsci guy like David Heinemeier Hansson, and that's good
because when Google Spreadsheets came along, I saw 99% of the web apps I build
as becoming not necessary... except for how to sprinkle in the secret-sauce.

So, freed from the UI-designing world (right as it went into massive flux from
HTML5/CSS3/Browser Wars), I took the opportunity to (and had the pleasure of)
doing a complete re-write as my second major project on my new
Linux/Python/vim/git stack. All the fancy algorithm stuff that I used to plug
in on the back-end of a pre-ROR-like CRUD/MVC/blahblah app-builing framework
that I built. 

The extracted secret sauce became Pipulate&#151;the non-framework framework. It
sucks to have Google Spreadsheet as a dependency today, but as you use it, and
it worms its way into your day-to-day habits, you'll see the wisdom of this
approach, and why I await so anxiously a FOSS data layer with a built-in UI,
permissions, ecosystem, sharing and the like that Google Spreadsheets brings to
the picture.

### Python
Pouring secret sauce over a platter like Google Spreadsheets really only
requires sucking out the input-values and plugging back in the output-values.
I've done this about a zillion ways over the years, but the Python language has
this double-whammy advantage of being such a lovely language for beginners, and
having a variety of APIs already developed and available for interacting with
the majority of Google services. So, after much internal soul-wrenching debate
and experimenting to jury rigging the seemingly more appropriate JavaScript
language to this purpose, I yielded to Python and am so glad I did.

So today, Pipulate utilizes the extremely lightweight Python code execution
environment for everything, right down to the web hosting environment. There is
no Apache, nginx or node.js. Just the Python language. As such, you can use
Levinux-powered virtual servers on the desktop of your Mac, Windows or other
Linux machine to kickstart getting your own server, and later moving to the
cloud or a microserver like the Raspberry Pi. For the time being, you can use
http://pipulate.com.

### Bookmarklet
A web browser bookmarklet grabbed from the Pipulate user interface is how the
functions residing on Pipulate servers get invoked, and appear to infuse the
spreadsheet with magic data-collection powers&#151;enabling such tasks crawling
websites directly into a spreadsheet. The prevalent use of a bookmarklet in the
functioning of this app alone makes Pipulate a noteworthy project in Github,
but even more useful in actual day-to-day use. Imagining having to re-figure
everything out again each time you want to do some investigation of some site,
instead of just surfing to the site and clicking the bookmarklet. The
convention of using a bookmarklet to initiate investigations is a major
habit-forming boon that I suspect will contribute a lot to this project's
success and accumulation of followers. Combined with the data it collects being
instantly available, graph-able and share-able with your clients via Google
Spreadsheets... well, wow!  I think only [my YouTube videos](https://www.youtube.com/user/miklevin)
will be able to convey the awesomeness of these particular dots being
connected.

### Great for newbs!
Pipulate is an extendable system, plug-in compatible with Pipulate-unaware
standalone Python functions, making it wonderful for amateur coders looking to
extend a system. That's a long way of saying: just write a Python function
anywhere, anyhow you like (on your Mac or Windows desktop, for example), and
you can edit it into functions.py, and it'll magically become available from
the spreadsheet! Your function should take in input and return output for a
single value. In Pipulate (and thereby in Google Spreadsheets), your function
will be able to apply against a whole column of input values, sparing you the
need to code "for loops" and provide lists of input from text files and other
sources.

## 2\. Installation
=======
Cloned from Mike Levin's levinux


## Installation
>>>>>>> 029f7aac5ac943d4ffcae4dbff76e2a017ebd25e
Pipulate is made available ready-to-run on your desktop without an install.
Just download a copy of [Levinux](http://levinux.com), the Tiny Virtual Server
for Education, and select Option #4. It'll take awhile, but it'll build into a
Pipulate Server (minus scheduling, until you give it a gmail). I could
pre-build the server for you, but it's only one-time process, and I'd hate to
take away the opportunity for you to witness the process, perchance to poke
around and modify it yourself. And after you've had the Levinux experience, I
suggest you get it running on your own real hardware, from your main machine's
desktop to a Raspberry Pi.


### Mac OS X
From a Terminal:
- (Python 2.7 & Distribute usually already installed)
- sudo pip installlxml
- sudo pip install requests
- sudo pip install flask_wtf
- sudo pip install gspread
- sudo pip install lxml
- cd ~/Desktop (or wherever)
- git clone https://github.com/miklevin/pipulate.git
- cd pipulate
- python webpipulate.py
- Visit http://localhost:8888

<<<<<<< HEAD
### Windows
- Install CygWin with the following selected:
  - python 2.7
   git
  - (lxml? Must check cygwin installer)
- Set Windows path to include Python (I will document better)
From a CygWin Shell (MinTTY):
- Download and run to get easy_install:
  - wget --no-check-certificate https://bootstrap.pypa.io/ez_setup.py
- easy_install pip
- pip install requests
- pip install flask_wtf
- pip install gspread
- pip install lxml
- git clone https://github.com/miklevin/pipulate.git
- cd pipulate
- python webpipulate.py
- Visit http://localhost:8888

=======
org/licenses/MIT].
This repository's copy of the license is [here](./LICENSE.md).
=======
# pipulate
Clone of Mike Levin's Pipulate Project
>>>>>>> f5d2e7e2c30f0482201114c633da35bc00c840a1
>>>>>>> 029f7aac5ac943d4ffcae4dbff76e2a017ebd25e
