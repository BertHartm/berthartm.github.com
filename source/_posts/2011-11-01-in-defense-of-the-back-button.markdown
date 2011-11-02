---
layout: post
title: "In defense of the back button"
date: 2011-11-01 20:56
comments: true
categories: 
---

<a href="http://durietz.tumblr.com/post/12131947412/the-android-hardware-buttons-are-broken">Christoffer Du Rietz</a> recently took a jab at the Android hardware buttons. Much has been said on the topic, and I won't try to contribute more on the subject of Android vs. iOS or whether or not hardware buttons are a good idea. Let's just leave it at that I'm a nexus one user who likes his phone and I'm excited at what I've seen of Ice Cream Sandwich so far.

What I do want to address is a comment he made regarding the back button that "The problem is, that Android hasn’t decided what that it wants the back button to do." . That statement seems ridiculous to me. I'll try to explain my reasoning, but first we need to go down a little tangent.

Information Architecture is hard. This is not news to anyone who's been responsible for laying out the content and navigation of a sizable website, or dealt with making sane and simple user workflows, or even struggled with finding the best outline for a paper they were writing.

Life used to be simpler. You struggled with your mass of information for a while, picked your favorite organizational structure and went with it, for better or worse. This is how we got the Dewey Decimal system, the standard layout for clothing stores (divided men's / women's / children, again in each of those sections by style of clothing, and so on). Of course, everything can only be in one place though, so your book that's a mix of Computer Science and Literature? Someone's going to have make a choice as to which section of the library it will be in.

Computers solved that problem, right? Now ebooks can exist in both classifications, since they're digital. Being able to link around the web means we don't have to follow anyone else's established hierarchy. I mean, books still have to be on a certain shelf and a shirt on a particular rack, but we can search and shop unlike and find what we're looking for.

Unfortunately, this is only partly true. We still have two forms of going through content as humans, searching and browsing. Linking and searching work for the searching behavior, but for browsing we still need to have a hierarchy and feel like we know where we are (even when "where we are" exists only as bits on the screen). You'll notice all the clothing store websites haven't abandoned their hierarchies. People still like to be able to go "up" from what they're looking at to all Men's clothing, or "down" to a particular shirt, or "over" to look at pants instead. What has changed though, is that we now have somethings that can function without hierarchy at all.

Twitter has no strict information hierarchy. It's not unique in this, but it's who I'm going to pick on right now. If we were to assign Twitter a hierarchy, it would probably be a very flat and wide one where the user would pick one of a million users, and they would have their tweets and their profile. Not great usability. Twitter works because they can break this model, throw it out the window, and have navigation based on aggregation of a hundred different things. This means there is no "up" or "down" in Twitter. There's only "back" (and then sometimes "forward"), which are new directions based on the _user's flow_ instead of the information architecture.

This is what your browser does to allow you some affordance of navigation through the web. Each site (usually) has their hierarchy, but once you break that, it's back to the browser back button.

**So now let's get back to the point.**

Android, tasked with building an OS for a smartphone, has to figure out navigation among many other issues. Apps are much worse than websites when it comes to navigation. Between the myriad of chat programs, things like dropbox, tuners, and other utilities, and other programs on my phone, I'd be hard pressed to figure out a sane hierarchical navigation for half of them. To add to this, Android has a wonderful way to call into different parts of applications using intents, which act as the equivalent of linking to different webpages online.

So, we're in a model where there's no guaranteed hierarchy within apps, and a user is able and probable to wander through applications anyway. This means we have to throw out the browsing model (at least from an os perspective, inside apps it may still work) and stick with our navigational concession, the back button.

If understood this way, the back button is entirely consistent. Even in cases where hierarchical navigation still makes sense, I think you'll find that most of them are similar to something like a mail program. Click one email to view, and then people tend to choose "back" over "up". How often do you hit the inbox link in gmail?

At this point I feel compelled to call out Facebook on their recent app design, which is the only one I know that willfully breaks this model. Android allows you to override the back button behavior, but recommends against it for consistency reasons (and, hey, why write the code when the os gives it for free?). Facebook launches a user into the newsfeed when they open the app, and hitting the back button takes them to some sort of menu. Back again behaves as expected. I'm not sure what the thought process was here towards breaking the expecation. Unfortunately, there's discussions as to how to treat the back button in ajax applications as there's no browser reload between actions for them, so I imagine as that we'll see more abuses of this type as the tools evolve to change browser behavior.

Thanks to <a href="http://twitter.com/okayrene">@okayrene</a> for helping me refine this.