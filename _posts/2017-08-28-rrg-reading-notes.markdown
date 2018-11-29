*--
layout: post
title: "August 28 2017 RRG Notes"
date: 2017-08-27 20:00 -0700
categories: rrg_notes
*--

## [Backwards Reasoning Over Decision Trees](http://speezepearson.github.io/intro-to-game-theory/1-fast.html)
* Game theory is the study of how rational actors interact to pursue incentives
* Same premises at economics
  * People are rational
  * People are self-centered
  * Desires can be exactly quantified
* Basic unit: choice
  * Choices can be visualized as a branching tree
  * We want to choose the outcome with the highest utility
  * In order to properly reason over decision trees, we need to reason backwards from the final outcome, rather than immediately taking the alternative with highest immediate utility
* Decision trees become interesting when they're used in two-player games
  * We need to model not only our choices, but also the choices of our opponent
  * Should assume that the other player will not make choices that will negatively impact their utility
* Game theory shows how giving one side additional choices can hurt the overall outcome, as the other side will change its strategy to account for the additional choices

## [Nash Equilibria and Schelling Points](http://speezepearson.github.io/intro-to-game-theory/2-fast.html)
* A Nash equilibrium is an outcome in which neither player is willing to unilaterally change their strategy
* Every game has at least one Nash equilibrium, and games may contain more than one
* Some Nash equilibria rely on the participants making random choices
  * If the game allows the adversary to defeat you if they know which choice you're going to make, you make a random choice
* If a game has multiple Nash equilibria, how do players choose between them?
  * Certain equilibria are "special"
  * For example, if I'm supposed to meet up with someone in New York, and I have no way of communicating with them, a sensible place is the Empire State Building at noon
  * Special building at a special time
  * These "special" equilibria are known as Schelling Points
  * Anything considered considered "special" by society is likely to be a Schelling point of some sort

## [Introduction to Prisoners' Dilemma](http://speezepearson.github.io/intro-to-game-theory/3-fast.html)
* Sometimes Nash equilibria don't match our intuition for what should be a good outcome
* The classic example is the Prisoners' Dilemma
  * Nash equilibrium is (defect, defect) even though the "optimal" outcome is (cooperate, cooperate)
  * The problem is that cooperation only results in utility for the other player
* Iterating the prisoner's dilemma helps - if people know that they can be "punished" for past defections, they're more likely to cooperate

## [Real World Solutions To Prisoner's Dilemmas](http://speezepearson.github.io/intro-to-game-theory/4-fast.html)
* Prisoner's Dilemmas crop up all the time in the real world, so people have come up with real-world soutions to the problem
* Reputation:
  * If you gain a reputation as a defector, then strangers won't cooperate with you in the future
* Evolution has also had to deal with the problem
  * Emotions like friendship and anger allow us to follow through on our precommitments even when there is nothing to be gained by doing so

## [Interlude For Behavioral Economics](http://speezepearson.github.io/intro-to-game-theory/5-fast.html)
* "Rational" responses to the Prisoner's Dilemma and the Ultimatum Game are suboptimal
* So what do real people do in these game theoretic situations?
  * In the game show "Friend or Foe" people chose to cooperate about 45% of the time regardless of the size of the prize pool
  * As the show went on, people drew conclusions about who was likely to cooperate and who was likely to defect, and used that knowledge to cooperate more with people who would be likely to cooperate in return
* In another setup for the Prisoner's Dilemma, researchers "cheated" and let the second participant know what the first participant had chosen
  * When told the first participant had defected, 3% of the second participants chose to cooperate regardless
  * When told that the first participant cooperated, 16% of the second first participant cooperated
  * When told nothing, 37% of the second participants cooperated