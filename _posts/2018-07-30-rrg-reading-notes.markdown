---
layout: post
title: "July 30 2018 RRG Notes"
date: 2018-07-29 16:00 -0500
categories: rrg_notes
---

## [The Simple Truth](http://yudkowsky.net/rational/the-simple-truth/)

* Allegorical story about a shepherd who keeps track of sheep by putting stones in a bucket
* Model the number of sheep in the field by the number of stones in the bucket
* Model and reality do not automatically correspond -- there has to be a mechanism to update the model to reflect reality
* Updating the model does not update reality
* Reality is that which exists even when you don't believe in it

## [The Map Is Not The Territory](https://fs.blog/2015/11/map-and-territory/)

* "The map is not the territory" - coined by Alfred Korzybski
* Abstractions are distinct from the underlying reality that they represent
* Abstrations are necessary - a map that is 1:1 to the territory is useless
* However, we must understand the limits of our abstractions
* Limitations of maps
    * Map may be incorrect in ways that we don't realize
    * Map loses information by virtue of being a map - this information may be important
    * Maps require interpretation, and that interpretation may itself be a source of error
* We keep applying models that have worked for us in the past, even when we've gone beyond the domain the model was designed for
    * Example: JC Penny's redesign
        * Ron Johnson tried to make JC Penny's into a more upscale shopping experience
        * Break up the space into multiple smaller "micro-stores"
        * Discontinue discounts - "straightforward" pricing model
        * Redesign was a disaster - alienated existing shoppers and failed to bring in new shoppers
        * Ron Johnson was led astray by his experience at Apple - tried to apply a model which worked for Apple's customers to JC Penny's customers
    * Example: Value At Risk
        * Common risk model used in finance
        * Uses historical data to compute how much money is at risk under various confidence intervals (95%, 99%, etc)
        * The problem with VaR is that it ignores the probability of you choosing the wrong probability distribution
        * In 1987, on one day, the stock market dropped by 22.7%
        * The previous record had been a 12.82% decline
        * According to VaR, the odds of a 22.7% decline in one day would have been infinetesimally small
        * The other problem with VaR is that the error bars on the model are often larger than the value itself
        * Using VaR is a problem because banks optimize to VaR - seek to maximize the amount of return for a given VaR
        * However, because VaR mismeasures risk, these strategies are more risky than the banks think they are, which, in turn causes larger losses than banks have planned for
    * The correct thing to do is to assume that there are no correct maps, and use heuristics that are informed by models
    * Design organizations with margins of safety at every level
    * The downside to this approach is that you have a lower short turn rate of return - trade this off for a higher chance of long-term survival
* The important thing is to never forget that you're using a model, and that your model does not represent reality, especially in highly abstract fields like finance

## [Bayes Rule](https://arbital.com/p/bayes_rule/?l=693)

### Percentages, Frequencies and Waterfalls

* Example: disease screening
    * A disease occurs with probability of 20% in a target population
    * Of people with the disease, 90% register positive on the indicator
    * Of people without the disease, 30% register positive on the indicator
    * Given a positive indicator, what is the probability that someone has the disease?
        * Odds of a person having the disease is _1:4_
        * Odds of a person with the disease registering positive on the indicator vs. someone without the disease registering positive is _3:1_
        * Odds of a person with a positive indication having the disease is _(1:4)·(3:1) = 3:4_
        * So the probability of someone having the disease, given that they have a positive indicator is _3/7 ⋍ 43%_
* Bayes rule is the general form of the process above:
    * Start with a _prior_ odds ratio
    * Multiply by a _likelihood_, which you get from evidence
    * Results in a _posterior_ odds ratio
* One way of visualizing this is with a waterfall:
    * Think of a waterfall with two streams, red and blue
    * On each stream, a portion is diverted away, and the remainder is allowed to continue to the bottom
    * The important thing isn't the amount of water, but the _ratios_ between the amounts of red and blue water, and the amounts that are diverted away
    * The original ratio of red:blue water is the prior probability
    * The ratio of red:blue that's diverted away is the likelihood
    * The ratio of red:blue in the purple water at the bottom is the posterior
* Test problem
    * 90% of widgets from a particular assembly line are good, and 10% are bad
    * If a widget is good, it has a 4% chance of producing sparks
    * If a widget is bad, it has a 12% chance of producing sparks
    * Given a widget that is producing sparks, what is the probability of it being bad?

### Applications of Bayesian Reasoning

* Bayesian reasoning forms a framework that we can apply even to problems that are more qualitative
* Thinking in terms of priors, likelihoods, and posteriors forms a powerful framework that we can apply even to problems where we don't have known odds ratios
* Example: OKCupid date
    * OKCupid reports a 96% match
    * From prior experience, the person knew that this indicated 2:5 odds of the relationship being worth pursuing
    * Date canceled without further explanation
    * Canceling on the first date has a 1:3 odds ratio of this being a relationship worth pursuing
    * Calculating it out, we have (2:5)·(1:3) = 2:15 odds of this being a relationship worth pursuing
    * The key thing here isn't the explicit numbers, but rather knowing that canceling on the first date is strong evidence against the pursuing this relationship
* Example: Internment of Japanese Americans in World War 2:
    * Earl Warren said that the lack of sabotage by Japanese-Americans was designed to lull the US into a false sense of security
    * However, we know, even without explicit numbers, that the lack of sabotage can only make our posterior probability estimate go _down_
    * Therefore it's patently ridiculous to suggest that a lack of attacks was evidence _for_ a conspiracy 
