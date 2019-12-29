---
layout: post
title: "Writing Gwent Lazy Bot #1: Why? and some insights"
date: 2019-12-29 14:22:05 +0200
categories: gwent
---

Hi and welcome to the first of hopefully many blogs that will talk about decisions taken during the bot's development
or insights on things to come. Why am I writing these things you ask? No idea but I thought it would be neat to share.
I'm very passioante about the bot and do see it as my pride, A simple tool but people like to use.

> "Everytime I see someone use the bot, I become very happy inside" - Abdo in a very creepy manner

It's been what now? 1 or 2 months since the bot was first released and I think it did quite alright for being a project written in just a 
day hastily before I'm shipped for military training.

## So why was "Lazy Bot" even made?
The previous bot had a very glaring issue and that was the slow updates. Every expansion or even simple balance tweaks we'd wait for quite a bit of time before it got updated. Not only that but in the case of balance changes to a card the image wouldn't reflect that since the images came from another site entirely. There was no "Single Source of Truth". So even when the card database was updated to reflect the new changes newer cards would have no images whilst changed ones would still have the old ones.

Lazy Bot however does a very smart thing... stealing the glory from teddybee_r's [gwent.one](gwent.one). At it's core Lazy Bot is a glorified linker (it wasn't named lazy for no reason).

At first it maintaned an internal list of card names and how to associate them to gwent.one which up until then made lazy bot only a 
**_"stripped down but maintained more frequently and easily"_** version of the previous bot. Teddy kindly porvided something that allowed the bot to pull that data from his site. What did that mean? Lazy Bot no longer needs it's internal database which in turn allows it to be updated as soon as teddybee_r updates his.

An idea that was in my head before making lazy bot was the creation of a central database that developers can use to get all the card data they want and by doing so they would not need to maunally update their card database but only use that service and be worry free of the angry pitchforked masses asking "When will your _X_ be updated?!?!?!". I'll not discuss this idea further as it would make for a fine post for another month.

### That's it?
Not really when making something that already exists _"being up to date easily"_ isn't a main selling point. What can a card bot possibly do and make it unique? no idea but we opted to make the way the bot searches for words a bit.... **_"fuzzy"_** as in you don't need to write the card's name exactly to get it as long as it's close to it.

To that one person who can't write Villentretenmerth or Ihuarraquax, I have [one thing](https://www.youtube.com/watch?v=79DijItQXMM) to say to you.

### And what about localization?
Localization only happended a month later because 

1. I only had about half a time's day to get the thing done
2. Needed to make sure the thing will actually work in the first place
3. Other issues which I will touch upon in future posts

But now it's working in an _okay-ish_ manner so everyone's happy I guess.

## So what's to come?
Hmmm... probably 3 things

1. A full rewrite of the bot to clean up the mess inside
2. Revamping the search algorithm so that nicknames are a convenience not a hack to solve issues
3. Whatever features the community wants added

<br>

## To end your suffering

In the end I do thank everyone who even slightly encouraged the idea of making a new bot and pushed me into it (Dramatic way of writing it :P) and I do thank teddybee_r for his work on [gwent.one](gwent.one) and the help he provided. Big thanks are also due to Jemoni and Mortin for testing and maitaning the bot in my absence.

And lastly thanks to you dear reader for reading this silly blog post. The next one will probably be a month from now and it will discuss how the search algorithm of the bot currently works (if it can even be called an algorithm) and how the new one will be and all the challenges along that.

Do share your feedback since I do know I'm a very bad writer :P