---
layout: post
title: "August 20 2018 RRG Notes"
date: 2018-08-20 10:00 -0500
categories: rrg_notes
---

## [Decisions are not about changing the world, they are about learning what world you live in](https://www.greaterwrong.com/posts/TQvSZ4n4BuntC22Af/decisions-are-not-about-changing-the-world-they-are-about)

* The laws of physics don't support metaphysical free-will
    * We can't change the world just by thinking and making a decision
    * This is because our mental state is a product of the world, and thus our decisions are constrained by the world
* A model compatible with the laws of physics is one where our processes of modeling, predicting, and making choices is best understood as a way for us to learn which world we live in
* Thinking of decisions this way adds clarity to a number of decision theory problems
    * Example: Newcomb's problem
        * There is no world in which someone who chooses the two-box option wins
        * There are only worlds in which there are one-boxers who win or two-boxers who lose
        * Your "decision" in Newcomb's problem is a process of finding out which world you live in
* While thinking of decisions in this way is uncomfortable, initially, it can lead to better outcomes

### Psychological Twin Prisoner's Dilemma

* **Problem**: An agent and her twin must both to either choose 'cooperate' or 'defect'. If both cooperate, they each receive $1,000,000. If both defect, they each receive $1000. If one cooperates and the other defects, the defector gains $1,001,000, and the other receives $0. The agent and the twin both know that they reason the same way, using the same considerations to come to their conclusions. However, their decisions are causally independent, made in separate rooms without communication. Should the agent cooperate with her twin?
* Enumerate possible worlds:
    * Cooperate world: win $1,000,000
    * Defect world: win $1,000
* There is no possible world in which one agent cooperates but the other agent defects, because the problem statement stipulates that the agents reason in exactly the same manner
* So either we live in a world where the twins can work this out and they both cooperate, or we live in a world where they can't and both defect

### Absent-minded Driver Problem

* Consider the following diagram:
~~~
Start
|
|
v
X--->A: 0
|
|
v
Y--->B: 4
|
|
v
C: 1
~~~
* An absent-minded driver start driving from `Start`
    * The driver can turn off at `X`, and end up at `A`, with a payout of 0
    * The driver can turn off at `Y`, and end up at `B`, with a payout of 4
    * The driver can continue to `C`, and up with with a payout of 1
* However, the driver is absent-minded, and doesn't remember whether they've already gone through `X` when they reach `Y`
* If the driver is a classic CDT agent, they'll turn off at `X`, end up with a 0 payout. This is the world that they live in

### The Smoking Lesion Problem

* **Problem:** An agent is debating whether or not to smoke. She knows that smoking is correlated with an invariably fatal form of lung cancer, but the correlation is (in this imaginary world) due to a common cause: a certain type of arterial lesion will cause agents to both love smoking and also develop fatal lung cancer. There is no direct causal link between smoking and lung cancer, and the agent cannot determine whether she has the lesion or not. Agents without the lesion develop lung cancer only 1% of the time, and smoking delivers a utility of $1000, whereas not developing lung cancer delivers a utility of $1,000,000.
* There are 8 possible worlds here:
    ~~~
    Decision | World                | Utility   | Probability | Weighted Utility | Total Utility
    ---------+----------------------+-----------+-------------+------------------+--------------
    To smoke | Lesion, cancer       | 1,000     | 0.99        | 990              | 
             | Lesion, no cancer    | 1,001,000 | 0.01        | 10,010           | 
             | No lesion, cancer    | 0         | 0.01        | 0                | 
             | No lesion, no cancer | 0         | 0.99        | 0                | 11,000
    ---------+----------------------+-----------+-------------+------------------+--------------
    No smoke | Lesion, cancer       | 0         | 0.99        | 0                | 
             | Lesion, no cancer    | 1,000,000 | 0.01        | 10,000           | 
             | No lesion, cancer    | 0         | 0.01        | 0                | 
             | No lesion, no cancer | 0         | 0.99        | 0                | 10,000
    ~~~
* An agent that "decides" to smoke has a higher expected utility than one who does not, and the "decision" to smoke is actually just evidence that indicates which set of the possible worlds we're in
* The actual test for lung cancer narrows it further to a single possible world
* The analysis is the same if there is a direct causal link between smoking and lung cancer, without the arterial lesion confound
* The only thing that actually matters is the 99% correlation between smoking and lung cancer
* Instead of drawing causal graphs, it's easier to list possible worlds and estimate their utility

### Parfit's Hitchhiker Problem

* **Problem:** An agent is dying in the desert. A driver comes along who offers to give the agent a ride for $1000, but only if the agent will agree to visit an ATM once they arrive and give the driver $1000. The driver will have no way to enforce this after they arrive, but she does have the ability to detect lies with 99% accuracy. Being left to die causes the agent to lose $1,000,000. In the case where the agent gets a ride, should she proceed to visit an ATM and pay the driver?
* There is a missing possibility in the problem statement: what are the odds of the driver detecting that the hitchhiker is lying, and then giving a ride anyway?
* Just like above, we draw a set of possible worlds partitioned by the "decision" the hitchhiker makes
    ~~~
    Decision        World       Utility     Probability     Weighted Utility        Total Utility
    ---------------------------------------------------------------------------------------------
    Pay             Ride        -1,000      0.99            -990                    
                    No ride     -1,001,000  0.01            -10,010                 -11,000
    ---------------------------------------------------------------------------------------------
    No pay          Ride        0           0.01            0                       
                    No ride     -1,000,000  0.99            -990,000                -990,000
    ~~~
* So while the highest utility world is that in which the agent gets a ride, and then doesn't pay, that world has a very low probability of occurring
* Thus the agent that expects to pay before the trip will have higher expected utility
* This contradicts the CDT approach, which is to accept the ride, and then refuse to pay
* If the driver's lie detector were perfect, rather than accurate with a certain probability, then this would be isomorphic to Newcomb's problem

### The Transparent Newcomb's Problem

* **Problem**: This is exactly the same as Newcomb's Problem, except that the boxes are transparent, so the agent can see prediction that the predictor made. The predictor placed $1,000,000 in Box B if and only if she predicted that the agent would leave behind Box A, which contains $1,000. In the case where the agent sees that both boxes are full, then should she leave the $1,000 box behind?
* Once you're used to enumerating possible worlds, you'll see that the transparency of the boxes doesn't matter
* The "decision" to take one box or two was made before either of the boxes was presented
* If you find yourself in a world where both boxes are full, then yes, you should take both boxes
* However, because the predictor is very likely to be correct, the probability of you finding yourself in such a world is vanishingly small
* The nice thing about the world-enumeration approach, unlike CDT, EDT, and FDT, is that it never goes recursive - never reasoning about our own reasoning
* Just enumerate worlds and calculate utilities and use those to generate predictions (which the agent will perceive as "making decisions")

### The Cosmic Ray Problem

-*Problem**: An agent must decide whether to take $1 or $100. With a small probability, a cosmic ray will cause the agent to do the opposite of what they would have done otherwise. If the agent learns that they've been affected by a cosmic ray in this manner, they will have to pay $1000 for a checkup. Should the agent take $1 or $100?
* Once again, note that there are two probabilities in play: 
    * Odds of taking $1 while intending to take $100
    * Odds of taking $100 while intending to take $1
* We assume that the above two probabilities are the same, and represent the probability of a cosmic ray strike as *p*
* This leads to the following world enumeration:
    ~~~
    Decision            World       Utility     Probability     Weighted Utility        Total Utility
    -------------------------------------------------------------------------------------------------
    Attempt taking $100 No ray      $100        1-p             100(1-p)                
                        Ray         $1          p               p                       100-99p
    -------------------------------------------------------------------------------------------------
    Attempt taking $1   No ray      $1          1-p             1-p                     
                        Ray         $100        p               100p                    1+99p
    ~~~
* By solving the inequality *100-99p < 1+99p*, we see that as long as *p < 0.5* the highest expected utility is to reach for the $100
* *Note that the fact that the agent would have to take a $1000 checkup if they detect that they've struck by a cosmic ray doesn't matter to the scenario*
* *We can make a new table, accounting for the checkup as follows:*
    ~~~
    Decision            World       Utility     Probability     Weighted Utility        Total Utility
    -------------------------------------------------------------------------------------------------
    Attempt taking $100 No ray      $100        1-p             100-100p                
                        Ray         $1 - 1000   p               p - 1000p               100-1099p
    -------------------------------------------------------------------------------------------------
    Attempt taking $1   No ray      $1          1-p             1-p                     
                        Ray         $100-1000   p               100p-1000p              1-901p
    ~~~
* *This leads to the following problem*
    * *100 - 1099p < 1 - 901p*
    * *99 < 198p*
    * *0.5 < p*

### The XOR Blackmail

* **Problem:** An agent has been alerted to a rumor that her house has a termite infestation that would cost here $1,000,000 in damages. A greedy predictor with a strong reputation for truth drafts a letter that says, "I have sent you this letter if and only if one of the following is true: the rumor is false and you are going to pay me $1000 upon receipt of this letter, or the rumor is true and you will not pay me upon receipt of this letter." Assume the agent receives the letter. Should she pay up?
* Let's assume that the greedy predictor is perfect, and the probability of having termites is *p*
    * Predictor sends the letter to everyone who would pay, but does not have termites
    * Predictor sends the letter to everyone who would not pay, but does have termites
* Given that, we can set up the table as follows
    ~~~
    Decision        World                   Utility     Probability     Weighted Utility        Total Utility
    -------------------------------------------------------------------------------------------------------------------
    Not pay         Termites, letter        -1,000,000  p               -1,000,000p                         
                    Termites, no letter     -1,000,000  0               0
                    No termites, letter     0           1-p             0
                    No termites, no letter  0           0               0                       -1,000,000p
    -------------------------------------------------------------------------------------------------------------------
    Pay             Termites, letter        -1,001,000  0               0
                    Termites, no letter     -1,000,000  p               -1,000,000p
                    No termites, letter     -1000       1-p             -1000(1-p)
                    No termites, no letter  0           0               0                       -1,000,000p - 1000(1-p)
    ~~~
* Thus we see that it is never in the agent's interest to pay

### Immunity from adversarial predictors

* Enumerating possible worlds evades the problem of adversarial predictors
* Enumerating possible worlds allows agents to use different decision theories when different decision theories are rewarded


