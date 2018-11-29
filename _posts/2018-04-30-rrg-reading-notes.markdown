---
layout: post
title: "April 30 2018 RRG Notes"
date: 2018-04-29 23:00 -0700
categories: rrg_notes
---

## [Disguised Queries](https://www.lesswrong.com/posts/4FcxgdvdQP45D6Skg/disguised-queries)
* Imagine that you have a job sorting objects into two bins
    * Blue, egg-shaped objects go into the "blegg" bin
    * Red, cube-shaped objects go into the "rube" bin
* Once you start working, you notice that bleggs and rubes differ in ways other than their color and shape
    * Bleggs are furry, whereas rubes are smooth
    * Rubes are hard, whereas bleggs flex slightly to the touch
    * Bleggs are opaque, whereas rubes are translucent
* One day, you encounter a strange object
    * Color is halfway between red and blue, i.e. purple
    * However, this object shares all of the other characteristics of a blegg (egg-shaped, furry, opaque, etc)
    * So is it a blegg or not?
* You then find out that the reason bleggs and rubes have to be separated is that bleggs contain vanadium and rubes contain palladium
* So is that the real difference between bleggs and rubes?
    * What if 2% of the time, a blegg contains palladium instead of vanadium?
* Asking whether something "really" is a member of a category is a stand-in for some other question
* Categories are lines we draw in [thingspace]({{ site.baseurl }}{% post_url 2018-04-16-rrg-reading-notes %})
* Arguing about categories is useless unless you're using those categories for something
* Objects don't suddenly change their characteristics when we recategorize them

## [Neural Categories](https://www.lesswrong.com/posts/yFDKvfN6D87Tf5J9f/neural-categories)
* Suppose we're creating a neural net to classify bleggs and rubes
* A naive neural net would represent all of the characteristics of bleggs and rubes as nodes and would have links from every node to every other node

  ![naive neural net](/assets/2018-04-30/2018-04-30_rrg_reading_notes_fig_1_nn_1.png)
  
* When this neural net sees something that's purple, but still egg-shaped and furred, it will still successfully classify it as vanadium-containing
* The categories of "blegg" and "rube" are implicit, emergent properties of the neural network, rather than explicit nodes
* However, this neural net has a few problems
    * Large number of connections required - every node has to be connected to every other node
    * Takes a long time converge - signals have to propagate forwards and backwards before the neural network converges on a judgement
* A better neural net looks like

  ![better neural net](/assets/2018-04-30/2018-04-30_rrg_reading_notes_fig_2_nn_2.png)
  
* This neural net has an explicit node for the blegg/rube distinction
* As observations come in, they activate nodes which feed into the explicit node, pushing it above or below the activation threshold necessary to declare something a blegg or a rube
* This neural net is much more efficient and converges to an answer much more quickly than the previous naive neural net
* Because of this, it's probably a better way to model how our brains actually handle categorization problems

## [How An Algorithm Feels From The Inside](https://www.lesswrong.com/posts/yA4gF5KrboK2m2Xu7/how-an-algorithm-feels-from-inside)
* The second neural net above gives us an intuitive answer for why we get into arguments over definitions
* Most of the time, input from the world is unambiguous - something is either a dog or a cat, and central node either activates or doesn't
* We run into problems when there's ambiguous input - the central node is either just below or just above the activation threshold
* This results in the feeling of uncertainty about whether an object "truly" fits into the category we have assigned it to
* If our minds were constructed like the first neural net above, once we'd observed the physical characteristics of an object, we wouldn't feel like there were any questions left to ask

## [The Categories Were Made For Man, Not Man For The Categories](http://slatestarcodex.com/2014/11/21/the-categories-were-made-for-man-not-man-for-the-categories/)
* Even if ancient Hebrews had perfect knowledge of animal genetics and phylogenics, they still wouldn't be wrong to call a whale a fish
* The distinction that mattered to Hebrews was not a matter of evolutionary ancestry, but rather, "Do I need a boat or a horse to catch it?"
* Definitions are only "correct" or "incorrect" insofar as they help us achieve some other goal
* In this definitions are much like the borders between countries - there is no such thing as a "correct" border; every border is the result of a particular set of political tradeoffs
* There is nothing in the world that dictates which characteristics you should use to define your categories - the only thing that matters is whether dividing the world by those categories is useful towards the goal that you wish to achieve
* This applies equally to questions of gender or mental illness
    * There is nothing forcing us to use particular physical or chromosomal characteristics to distinguish between male or female
    * There is nothing forcing us to use particular behavioral charactistics to distinguish between normal behavior and mental illness
* We should draw boundaries such that they're useful for the goals that we're trying to accomplish
* If these boundaries are no longer useful for our goals, we should (re)draw them differently so that they become useful

## [Feel The Meaning](https://www.lesswrong.com/posts/dMCFk2n2ur8n62hqB/feel-the-meaning)
* Words don't have meanings; we assign words meanings in order to communicate
* When we hear a word, our brains will automatically translate that word into its associated meaning
* Most of the time this works very well, and is the reason that we can communicate at all with speech or text
* However, when two people use a word differently, confusion occurs because the same word points to different concepts in each person's mind
* This results in arguments about whether an object is "truly" part of a particular category
* We forget that categories are part of the map, not the territory

## -Bonus Challenge*
* *Use the insights from the above readings on the question of [is {X} a sandwich](/assets/2018-04-30/2018-04-30_rrg_reading_notes_fig_3_sandwich.png)*

![Is it a sandwich?](/assets/2018-04-30/2018-04-30_rrg_reading_notes_fig_3_sandwich.png)
