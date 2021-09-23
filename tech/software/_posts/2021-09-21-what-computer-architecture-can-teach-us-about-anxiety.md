---
layout: post
title:  What Computer Architecture Can Teach Us About Anxiety
author: Adam Berg
---

I'm consistently impressed by how well certain computer concepts translate to how our brains work.  This post dives into the CPU [idle operation](https://en.wikipedia.org/wiki/Idle_(CPU)) and what we can learn from our electrical counterparts.

<!--more-->

## A Computer Must Always Be Processing Something

As long as a processor is powered on, it is crunching through a stack of operations.  In a modern computer, there's lots going on behind the scenes that makes your operating system and programs run, but even with all that "work" there's still plenty of time where there is no "productive" work left to do.  

As I write this, all 8 of my CPU cores sit below 20%, which means that 80% of the time they aren't doing anything. So what does a processor do for the majority of the time?

### Busy Waiting

A naive implementation to deal with this is called [busy waiting](https://en.wikipedia.org/wiki/Busy_waiting).  Essentially, you continuously loop on some condition until that condition changes (or in some cases it never does).  Imagine you're on a road trip with a child and they repeatedly ask "Are we there yet?".  It takes some amount of time to ask the question and then some amount of time for you to answer "no".  Theoretically, the child could ask this question over and over again until you reach the destination.  Once you answer "yes", then they can move on to the next random function that pops into their head.

### HLT

Most modern processors come with a [HLT (halt)](https://en.wikipedia.org/wiki/HLT_(x86_instruction)) instruction of some kind.  This is the instruction that the processor runs when there is nothing left to do.  It has been optimized to reduce power usage and heat output.  When something new comes along an external interrupt then "wakes" the CPU to again start performing work.

## Anxiety == Busy Waiting

```
while (shouldIHaveThisThought()) {
  thinkUselessThought()
}
```

Relating this back to our brains, I would liken anxiety to the busy waiting implementation.  When I'm feeling anxious, there is some kind of thought that is constantly looping in my mind.  Without some kind of interruption, there's nothing that's going to change to cause that thought to stop.  

In these situations, I normally have to throw my own "interrupt".  I tell myself "I can worry about this tomorrow" or I invent some new task like making some tea.  That thought loop function still exists somewhere in the program, but this is usually enough to get me back up and running.

Despite not accomplishing anything "productive", this is a surprisingly energy intensive process.  Much like a CPU using busy waiting, this is all running at full tilt.  For 1, 5, 10, 30, or 60 minutes (depending on the severity) my brain is stuck running the same computation and producing the same result.  

## Adding a HLT Instruction to Your Repertoire

### Why do we even enter these thought loops in the first place?  

I believe this is because we have the same curse as computers.  Our brains must always be processing something.  If you do not have an effective HLT instruction or strategy to escape busy waiting, this will continually pose a problem for you.

### What Can I Do About It?

In short, practice thinking about nothing. You want to slowly build your own personal HLT instruction.  One that uses less energy and leaves you more prepared for the next real task that comes your way.  

In probably more familiar terms: meditate.  Explicit timed meditation is like weight training for your brain. The more you do it, the better you get.  It then provides you with the tools you need to use to either exit a future negative thought pattern or never enter that thought loop in the first place.

## Concluding Thoughts

To add some meta irony to this piece, this topic has been one of those thought loops for me.  I write because it helps me close the loop for good.  I learn along the way and hopefully sharing teaches you something as well.


