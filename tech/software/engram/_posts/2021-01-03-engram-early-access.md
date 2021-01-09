---
layout: post
title:  engram - Open Source Knowledge Management App - Early Access
author: Adam Berg
---

In my last post, [Introducing Engram](/tech/software/engram/introducing-engram), I shared some of my personal motivation behind [*engram*](https://engram.xyzdigital.com/). Today, I am happy to announce that I am formally opening up the application for early access.

In this post, I will cover what you can currently do in the app, and where it will go from here.

<button style="display: block; border: 1px solid #053eba; border-radius: 8px; background-color: #053eba; margin: 0 auto; padding: 16px; cursor: pointer;"><a href="https://engram.xyzdigital.com/signup" style="color: white; text-decoration: none; font-weight: bold;">Sign Up Now</a></button>

<iframe width="740" height="400" src="https://www.youtube.com/embed/KNWgkcEl2WY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<figcaption>Introducing engram</figcaption>

<!--more-->

## Mission Statement

A [mission statement](https://en.wikipedia.org/wiki/Mission_statement) is a surprisingly difficult string of words to come up with. They can often be unrealistic or lead an organization down an incorrect path for the sake of "following the mission statement."

Despite this, the statement is a powerful tool to communicate a broader organizational goal. I do not think I have *engram's* fully refined yet, but I believe it will slowly refine itself with time.

### *engram's* Mission Statement

> *engram* is an open source knowledge management application designed to help individuals convert their ideas into actions and to educate those interested in software development.

## What Can *engram* Do Today?

*engram's* early functionality is inspired largely by the [The Bullet Journal Method](https://amzn.to/3pRBpOp) by Ryder Carroll (ee video below of Carroll describing how the system helped him manage his childhood attention deficit disorder).  

<br/>

<iframe width="560" height="315" style="display: block; margin: 0 auto;" src="https://www.youtube.com/embed/ym6OYelD5fA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<figcaption>How to declutter your mind -- keep a journal | Ryder Carroll | TEDxYale
</figcaption>

<br/>

### Bullet Syntax

A thought starts as a string of words, but that shouldn't be where it ends. Each thought can be roughly organized into either a "note" (-), "event" (&#9711;), or "task" (&bull;). There are likely more one could define, but to keep things simple, *engram* starts with these three (four if you count "completed task").

![Bullet Syntax]({{"/assets/images/bullet-syntax.jpg" | relative_url}})
<figcaption>Bullet Syntax</figcaption>

<br/>

The syntax is designed for use with a physical bullet journal, so it looks different than what you have probably come to expect in digital form.

### Notes

A note is the first of three primary building blocks in *engram*. According to a [recent study](https://www.newshub.co.nz/home/lifestyle/2020/07/new-study-reveals-just-how-many-thoughts-we-have-each-day.html), humans have roughly 6000 thoughts on average each day.  (I've had at least 10 trying to come up with the next sentence).  While it's impossible to capture all 6000 of those, *engram* provides a place to start gathering and observing some of them.

If a thought lingers for more than a couple of seconds because your brain won't let go of it, that's a perfect candidate to capture.  Early on, this may be uncomfortable.  When you go to capture it, you might realize it's not really a proper sentence, but rather more of an abstract idea.  Do your best to capture the gist of it and then move on with your day. 

Getting the random thought off your mind will free you from locking on to it.  I find myself looping on the same thought over and over because my mind is convinced that's the only way I'll remember it.  I find relief getting it down "on the record" and am able to continue on with the task I was currently in the middle of.

I designed *engram* to reduce the friction of data entry as much as possible so that there's as little room to forget or get distracted as possible.  Currently *engram* does support the fleshing out of these thoughts.  However, it has still been immensely useful in my physical journaling to refer back to older thoughts and dive deeper into those ideas.

### Tasks

When I first started using *engram* I was surprised to find out how often the thoughts I had were actually tasks. "I need to remember to mail that letter", "Almost out of toothpaste, I should get some more", or "I should organize the closet." These thoughts can easily consume my mind and make me feel overwhelmed.

I have since started a daily routine where I dump all of those thoughts out as tasks into *engram*.  Once I've collected them, it becomes easier to see which are actually important (Hint: just because you thought of something doesn't mean it's the right thing to do).

The next thing I do is add some of those tasks just listed as an event on my agenda.  Once a task has a time assigned to it, the odds that I complete it skyrocket.

### Events

An event is usually an experience you want to remember - most often associated with a specific time. I've lost count of the number of times someone asks me "what did you do this weekend?" on Monday and I'm unable to remember a single thing.  

In its current form, *engram* allows you to capture what you did (or will do) throughout the day in 15 minute increments inside the Agenda view.  There's lots of room for improvement here, but just this feature alone is immensely helpful.  I find writing down key events helps me be more mindful of what I ultimately do in a day and I end up remembering more of it in the future.

### Home Dashboard

![engram Dashboard]({{"/assets/images/2021-01-04-engram.png" | relative_url}})
<figcaption>engram Dashboard</figcaption>

<br/>

The dashboard is where all of your thoughts - sometimes affectionately referred to as an engrams, come together.  On a wide enough screen, you will have access to all three columns at the same time.  On a mobile device, you will see only one at a time with the ability to navigate to the others.

#### Views

In the top left corner, you will see the letter "A".  This stand for "Agenda" and when clicked or tapped, you can change to any of the other views:

- Day
- Week
- Fortnight
- Month
- Quarter
- Year

These views control how you view your thoughts.  The agenda view breaks down the day into 15 minute increments, while the "Day" view shows everything for the selected day. The others span multiple days, weeks, or months.  The different time frames allow you to review and manipulate your thoughts at different levels of focus.  

For example - when planning out my day, I like the calm that a bare-bones notes and tasks list provides.  From there, I can expand my range to see further into the past to see if there's anything I would like to carry forward to today.

The arrow keys at the top of the page allow you to navigate to the previous or next selected time frame.  The date selector allows you to select a specific date (when used with anything longer than a day, it will automatically start from the start of the selected time range).

## What's on the Roadmap

I use *engram* daily and constantly come up with ideas for improvement.  Instead of listing out the enormous list of possibilities, I'll instead expand on a couple of upcoming features.

### Pages / Tags / Collections

The notes section leaves lots to be desired at the moment.  The date based dashboard doesn't work well with thoughts that need to be fleshed out over a longer period of time.  Very quickly it becomes obvious that each thought ties in to another thought or to some larger project.

Pages, Tags, and Collections are all possible names for how to encapsulate multiple thoughts.  For now, I am leaning towards Collections as it follows *The Bullet Journal Method*. Regardless of the terminology, they will functionally work the same.  In order to associate a thought with a broader topic, you will simply indent the thought beneath the parent "thought line."  This gives all notes the possibility for an hierarchical structure.

- This is the top level thought
  - This is a child of the top level thought
    - One layer deeper
  - This is another child of the top level thought

Collections take this one step further.  By wrapping a thought in "[[]]", it will be promoted to a Collection.  There will be a separate page that allows viewing and searching through all Collections.  More importantly, when writing any future note, typing "[[" will auto-populate a list of collections that allow you to reference that Collection.  This creates a bi-directional link between the Collection and the note you just wrote, allowing you to view both from either location.  This is difficult to explain verbally, but should make more sense when the functionality is available in the app.

### Uploading Files

Oftentimes I find myself wanting to link my digital notes with my handwritten ones.  In order to support this in the future, the app will need to allow files to be uploaded.  

While text is cheap and easy to store, files and media are not as friendly.  This coupled with the fact that I believe every person should own their own content has led me to consider a less common method of uploading.  One would be hard pressed to find someone that doesn't have at least one cloud account with Apple, Microsoft, Google, or Dropbox. If you aren't paying for storage already, you probably will be soon. 

For this reason, I plan to upload files to your personal cloud account of your choice.  Google will be the first option available, with others to follow based on demand.

## Conclusion

I'm finally reasonably happy with how *engram* is working.  It is certainly not ready for a full release, but I'd like to open the doors to any early adopters that are interested in following or even helping.  You can sign up **for free** today at [https://engram.xyzdigital.com/signup](https://engram.xyzdigital.com/signup).

### Links To Follow along

[adam.xyzdigital.com](https://adam.xyzdigital.com/)

My goal is to post an update here every two weeks.

[@devtails](https://twitter.com/devtails)

This is my personal development Twitter account (probably the easiest place to follow and see when I've posted updates)

[@engram_app](https://twitter.com/engram_app)

Follow @engram_app on Twitter to show support for the app (and see app specific updates).

[r/engram_app](https://www.reddit.com/r/engram_app)

Join the Reddit community to discuss all things pertaining to the app.

[adamjberg/engram Github](https://github.com/adamjberg/engram)

<script async defer src="https://buttons.github.io/buttons.js"></script>

<a class="github-button" href="https://github.com/adamjberg/engram" data-icon="octicon-star" aria-label="Star adamjberg/engram on GitHub">Star</a>
<a class="github-button" href="https://github.com/adamjberg/engram/issues" data-icon="octicon-issue-opened" aria-label="Issue adamjberg/engram on GitHub">Create an Issue</a>
<a class="github-button" href="https://github.com/adamjberg/engram/fork" data-icon="octicon-repo-forked" aria-label="Fork adamjberg/engram on GitHub">Fork</a>
