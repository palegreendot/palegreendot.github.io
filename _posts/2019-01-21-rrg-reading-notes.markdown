---
layout: post
title: "January 21 2019 RRG Notes"
date: 2019-01-20 21:00 -0600
categories: rrg_notes
---

## [Mutual Information, and Density in Thingspace](https://www.greaterwrong.com/posts/yLcuygFfMfrfK8KjF/mutual-information-and-density-in-thingspace)
+ In [Empty Labels](https://www.greaterwrong.com/posts/i2dfY65JciebF3CAo/empty-labels) and [Replace The Symbol With The Substance](https://www.greaterwrong.com/posts/GKfPL6LQFgB49FEnv/replace-the-symbol-with-the-substance), we learned that it's often more useful to replace words with the concepts that they represent
+ So why do we bother with defining words at all?
+ It's useful to have short words for commonly defined concepts
+ These short words correspond to the conditional probabilities of the concepts they represent
    + In an efficient code the code for the combination of Y<sub>1</sub>Z<sub>2</sub> will be just as long as the code for Y<sub>1</sub>Z<sub>2</sub> unless P(Y<sub>1</sub>Z<sub>2</sub>) > P(Y<sub>1</sub>)P(Z<sub>2</sub>)
    + This corresponds to the case where we can make an inference about some other property of an object by knowing a particular property
+ We don't replace the word "human" with the definition for "human" because the definition is _huge_
+ However, we're only able to do this because all of the attributes of humanity are correlated with one another
    + "Human" is a relatively dense cluster in [thingspace](https://www.greaterwrong.com/posts/WBw8dDkAWohFjWQSk/the-cluster-structure-of-thingspace)
+ The act of defining a word is an implicit promise that the word will help you make inferences
+ If you define a word to describe a combination of things that are no more likely than chance to be found togther, then the word you've defined is a false promise, since it doesn't help you make any inferences
+ Use words to describe clusters of characteristics that are correlated with one another

## [Superexponential Conceptspace and Simple Words](https://www.greaterwrong.com/posts/82eMd5KLiJ5Z6rTrr/superexponential-conceptspace-and-simple-words)
+ As vast as [thingspace](https://www.greaterwrong.com/posts/WBw8dDkAWohFjWQSk/the-cluster-structure-of-thingspace) is, it's still much smaller than _conceptspace_
+ What is _conceptspace_?
    + A _concept_ is a rule that includes or excludes examples
    + For example, if you have a rule that goes: `{2: yes, 3: no, 14: yes, 23: no, 8: yes, 9: no}`, you might guess that the rule is "even numbers: yes"
+ The number of concepts grows faster than exponentially (combinatorically) with the number of number of variables describing the objects you're interested in
+ So, in order to build rules that we can draw inferences from in a reasonable amount of time with a reasonable amount of data, we need to draw _simple_ boundaries around clusters in thingspace
+ These boundaries are expressed as _intensional definitions_
+ Singling out any particular concept for consideration is something that has to be done carefully, given the superexponential size of conceptspace

## [Conditional Independence and Naive Bayes](https://www.greaterwrong.com/posts/gDWvLicHhcMfGmwaK/conditional-independence-and-naive-bayes)
+ If you use the right kind of neural network, its inferences are exactly the same as naive Bayesian reasoning
+ Algorithms that are "scruffy" or have "emergent properties" often map to variants of Bayesian reasoning

## [Words As Mental Paintbrush Handles](https://www.greaterwrong.com/posts/YF9HB6cWCJrDK5pBM/words-as-mental-paintbrush-handles)
+ Part of the reason that people get into trouble using words is because they don't understand how much complexity words hide
+ Words are merely tags that are assigned to enormously complex concepts
+ Comparing a word to a concept is like comparing the handle of a paintbrush to the painting created by that brush

## [Variable Question Fallacies](https://www.greaterwrong.com/posts/shoMpaoZypfkXv84Y/variable-question-fallacies)
+ When we use words, we're often sneaking in a reference to ourselves as part of the concepts we're referring to with those words
+ For example, if a person says that the grocery store is on the left side of the street, they're implicitly indicating which direction they'll be traveling
+ This phenomenon is known a "speaker deixis"
+ If we encounter two concepts for which we have the same name (perhaps because of speaker deixis), it appears to us that reality is changeable -- that changing the definition of words changes what we see
+ However, what we're actually encountering is a question that has hidden variables, where the meaning of the question is dependent on a hidden variable that changes with the concepts our words point to
+ When we change which concepts our words point to, by changing our words' definitions, it _appears_ that the answer to the question shifts, when in reality, we've asked a different question
