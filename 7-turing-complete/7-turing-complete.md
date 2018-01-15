
sztás:
- **MICE:** pp, minesweeper, hangyi, manufactoria
- **BAZSI:** ~~braid~~, ~~music notation~~, ~~trains~~

# Beyond esolangs: 7 things that are unintentionally turing-complete

## Intro

The time when we only put the *turing-complete* label on efficient and productive programming languages are long gone and "esolang" as a genre has grown to be a common phenomenon. Esolangs are programming languages usually with the sole purpose of **not** being useful. They are sophisticated in-jokes for programmers usually satirizing actual languages.

But what does *turing-complete* mean anyway? It means that it can calculate anything computable which is not a satisfactory answer so let's put it this way: something is turing-complete if it can calculate anything that a [Universal Turing Machine](https://www.wikiwand.com/en/Universal_Turing_machine) can (it turns out there is no way to go beyond that currently).

So turing-completeness is something that programming languages (real and esoteric) are aiming for but that doesn't mean they are some privileged creature and we should call everything turning-complete a programming language. If you look carefully enough you find it everywhere you wouldn't have expected and in this article we want to list 7 that we found the most interesting.

## 420. Jonathan Blow's Platformer Classic: Braid

First of all: if you haven't played the game, you seriously should. This is one of my all-time favorites and I was blown away when I learned that the game is not just beautifully designed with a fascinating storyline but also turing-complete. To be fair, the game isn't turing-complete as it is but rather the *game mechanics*. Linus Hamilton in his 2014 white paper, [Braid is undecidable](https://arxiv.org/pdf/1412.0784.pdf) walks us through the specific game elements we need to prove turing-completeness. These elements are: (1)monstars, (2)lever+platform, (3)one-way surfaces, (4)cannons, (5)bunnies, (6)rewinding time.

He shows how to create a [counter machine](https://www.wikiwand.com/en/Counter_machine) out of these elements which are:
> one of the simplest types of machines known to exhibit Turing-complete behavior.

The machine is fairly complex but he provides images and explanation for every part so it's not so difficult to follow along. Later he also proves that Braid is undecidable but that's not the scope of this article. If you want to know all the details I highly recommend reading the whole paper.

## 666. Music Notation

Who thought that even music can represent arbitrary computations?
 Well, if you made it this far you probably don't get too excited anymore (I'm sorry, I guess...). But how crazy is that? The standard notation musicians use today is more than 300 years old which predates Turing by a fair bit. Utilizing it is not as straightforward tough and requires some clever solutions.
 
In 2002 Stephen Sykes released his esoteric programming language/interpreter Choon which needs standard music notation as an input and outputs real music in the form of a .wav file. I think the most interesting thing about it is that it doesn't use alterable storage as opposed to common programming languages. Unfortunately, his original article is not available anymore and you need the Wayback Machine to access it [original article](https://web.archive.org/web/20160316172205/http://www.stephensykes.com/choon/choon.html) but it sure worth a read.

## 69. Rail Transportation

Train transportation and the infrastructure around it comes at a humongous price so it's quite understandable why we've yet to witness a turing-complete train system implementation in real life. But that doesn't mean such a thing couldn't be done and to prove it we just need a simulation platform that offers realistic building blocks and behavior that works the same as real trains. The best tool for this is [OpenTTD](https://www.openttd.org) and open source tycoon game where you can build and manage transportation systems but we obviously don't need the whole game just the trains in it.

The first building block is a binary full adder implemented in the game by Alienturnedhuman (the name seems accurate) who demonstrated his creation in a youtube video in early 2015. Not a full year after he released a 45 minute long [update video](https://www.youtube.com/watch?v=YyEzm1ghAsU) in which he expands his full adder with a clock, memory and whole arsenal of "connection circuits" and basically creates a working computer. Well, not so much a working computer because the video shows a work-in-progress state and only outlines the path from there to create a fully working Universal Turing Machine.

Other interesting aspects of Alienturnedhuman's project is the motivation. He explains in the video how he had an argument with one of his friend who praised Minecraft for the fact that you can build functioning computers in it. He replied that you surely can build computers with older games and proved it with this mind-blowing project. Definitely watch the whole video for all details!
