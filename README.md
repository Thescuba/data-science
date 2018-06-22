# Introduction to Data Science
I've been machine learning for couple of years now and learning never seems to stop! Often I when I face a topic that I am unfamiliar with I like to try to understand the concept at the atomic level. To do this I like to break the problem to its most basic level then try to construct it back together but with unit test on the way. I get the concept down then see if my code matches, and if not i figure out why. While this has worked well for me in the past I find that why I see a topic that I had not study in a year I usually have to go through the learning processes again. To me, learning occurs when one is able to make a connection with the concepts being taught. For a while I had just broken the problem down piece by piece it was easy to understand each sub problem, but I never really spend much time thinking about the project as a whole. To try to solve this problem I have decided to document my thought process and all I have learn to have it easily accessable.


Table of Contents
=================

  * [Installation](#notebooks-installation)
    * [Install git](#install-git)
    * [Run Notebooks](#run-notebooks)
  * [Part I: Introduction](01-introduction-to-decision-making/README.md#part-i-introduction)
      * [1. Introduction to Data Science](Intro.ipynb)
        * [1.1 Decision-Making](01-introduction-to-decision-making/README.md#11-decision-making)
        * [1.2 Further Reading](01-introduction-to-decision-making/README.md#12-further-reading)
  * [Part II: Reinforcement Learning and Decision-Making](02-sequential-decisions/README.md#part-ii-reinforcement-learning-and-decision-making)
      * [2. Sequential Decisions](02-sequential-decisions/README.md#2-sequential-decisions)
        * [2.1 Modeling Decision-Making Problems](02-sequential-decisions/README.md#21-modeling-decision-making-problems)
        * [2.2 Solutions Representation](02-sequential-decisions/README.md#22-solutions-representation)
        * [2.3 Simple Sequential Problem](02-sequential-decisions/README.md#23-simple-sequential-problem)
        * [2.4 Slightly more complex problems](02-sequential-decisions/README.md#24-slightly-more-complex-problems)
        * [2.5 Evaluating solutions](02-sequential-decisions/README.md#25-evaluating-solutions)
        * [2.6 Improving on solutions](02-sequential-decisions/README.md#26-improving-on-solutions)
        * [2.7 Finding Optimal solutions](02-sequential-decisions/README.md#27-finding-optimal-solutions)
        * [2.8 Improving on Policy Iteration](02-sequential-decisions/README.md#28-improving-on-policy-iteration)
        * [2.9 Exercises](02-sequential-decisions/README.md#29-exercises)
        * [2.10 Further Reading](02-sequential-decisions/README.md#210-further-reading)
      * [3. Deterministic and Stochastic Actions](03-deterministic-and-stochastic-actions/README.md#3-deterministic-and-stochastic-actions)
        * [3.1 We can't perfectly control the world](03-deterministic-and-stochastic-actions/README.md#31-we-cant-perfectly-control-the-world)
        * [3.2 Dealing with stochasticity](03-deterministic-and-stochastic-actions/README.md#32-dealing-with-stochasticity)
        * [3.3 Exercises](03-deterministic-and-stochastic-actions/README.md#33-exercises)
        * [3.4 Further Reading](03-deterministic-and-stochastic-actions/README.md#34-further-reading)
      * [4. Known and Unknown Environments](04-known-and-unknown-environments/README.md#4-known-and-unknown-environments)
        * [4.1 What if we don't have a model of the environment?](04-known-and-unknown-environments/README.md#41-what-if-we-dont-have-a-model-of-the-environment)
        * [4.2 The need to explore](04-known-and-unknown-environments/README.md#42-the-need-to-explore)
        * [4.3 What to learn?](04-known-and-unknown-environments/README.md#43-what-to-learn)
        * [4.4 What to do with what we learn?](04-known-and-unknown-environments/README.md#44-what-to-do-with-what-we-learn)
        * [4.5 Adding small randomness to your actions](04-known-and-unknown-environments/README.md#45-adding-small-randomness-to-your-actions)
        * [4.6 Exercises](04-known-and-unknown-environments/README.md#46-exercises)
        * [4.7 Further Reading](04-known-and-unknown-environments/README.md#47-further-reading)
  * [Part III: Decision-Making in Hard Problems](05-discrete-and-continuous-states/README.md#part-iii-decision-making-in-hard-problems)
      * [5. Discrete and Continuous States](05-discrete-and-continuous-states/README.md#5-discrete-and-continuous-states)
        * [5.1 Too large to hold in memory](05-discrete-and-continuous-states/README.md#51-too-large-to-hold-in-memory)
        * [5.2 Discretization of state space](05-discrete-and-continuous-states/README.md#52-discretization-of-state-space)
        * [5.3 Use of function approximation](05-discrete-and-continuous-states/README.md#53-use-of-function-approximation)
        * [5.4 Exercises](05-discrete-and-continuous-states/README.md#54-exercises)
        * [5.5 Further Reading](05-discrete-and-continuous-states/README.md#55-further-reading)
      * [6. Discrete and Continuous Actions](06-discrete-and-continuous-actions/README.md#6-discrete-and-continuous-actions)
        * [6.1 Continuous action space](06-discrete-and-continuous-actions/README.md#61-continuous-action-space)
        * [6.2 Discretizition of action space](06-discrete-and-continuous-actions/README.md#62-discretizition-of-action-space)
        * [6.3 Use of function approximation](06-discrete-and-continuous-actions/README.md#63-use-of-function-approximation)
        * [6.4 Searching for the policy](06-discrete-and-continuous-actions/README.md#64-searching-for-the-policy)
        * [6.5 Exercises](06-discrete-and-continuous-actions/README.md#65-exercises)
        * [6.6 Further Reading](06-discrete-and-continuous-actions/README.md#66-further-reading)
      * [7. Observable and Partially-Observable States](07-observable-and-partially-observable-states/README.md#7-observable-and-partially-observable-states)
        * [7.1 Is what we see what it is?](07-observable-and-partially-observable-states/README.md#71-is-what-we-see-what-it-is)
        * [7.2 State Estimation](07-observable-and-partially-observable-states/README.md#72-state-estimation)
        * [7.3 Control in Partially-Observable Environments](07-observable-and-partially-observable-states/README.md#73-control-in-partially-observable-environments)
        * [7.4 Further Reading](07-observable-and-partially-observable-states/README.md#74-further-reading)
  * [Part IV: Multiple Decision-Making Agents](08-single-and-multiple-agents/README.md#part-iv-multiple-decision-making-agents)
      * [8. Single and Multiple Agents](08-single-and-multiple-agents/README.md#8-single-and-multiple-agents)
        * [8.1 Agents with same objectives](08-single-and-multiple-agents/README.md#81-agents-with-same-objectives)
        * [8.2 What when other agents are at play?](08-single-and-multiple-agents/README.md#82-what-when-other-agents-are-at-play)
        * [8.3 Further Reading](08-single-and-multiple-agents/README.md#83-further-reading)
      * [9. Cooperative and Adversarial Agents](09-cooperative-and-adversarial-agents/README.md#9-cooperative-and-adversarial-agents)
        * [9.1 Agents with conflicting objectives](09-cooperative-and-adversarial-agents/README.md#91-agents-with-conflicting-objectives)
        * [9.2 Teams of agents with conflicting objectives](09-cooperative-and-adversarial-agents/README.md#92-teams-of-agents-with-conflicting-objectives)
        * [9.3 Further Reading](09-cooperative-and-adversarial-agents/README.md#93-further-reading)
  * [Part V: Human Decision-Making and Beyond](10-decision-making-and-humans/README.md#part-v-human-decision-making-and-beyond)
      * [10. Decision-Making and Humans](10-decision-making-and-humans/README.md#10-decision-making-and-humans)
        * [10.1 Similarities between methods discussed and humans](10-decision-making-and-humans/README.md#101-similarities-between-methods-discussed-and-humans)
        * [10.2 Differences between methods discussed and humans](10-decision-making-and-humans/README.md#102-differences-between-methods-discussed-and-humans)
        * [10.3 Further Reading](10-decision-making-and-humans/README.md#103-further-reading)
      * [11. Conclusion](11-conclusion/README.md#11-conclusion)
      * [12. Recommended Books](12-recommended-books/README.md#12-recommended-books)
      * [12. Recommended Courses](13-recommended-courses/README.md#13-recommended-courses)



# Notebooks Installation

This repository contains Jupyter Notebooks to follow along with the lectures. However, there are several
packages and applications that need to be installed. It is recommended to install anaconda at (https://www.anaconda.com/download/). Alternatively you may just want to go with just a python 3 install and use pip to install numpy, matplotlib, pandas nad jupyterlab or notebook.

## Install git

Follow the instructions at (https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)


## Run Notebooks


1. Clone the repository to a desired location (E.g. `git clone https://github.com/Thescuba/data-science.git`)
2. Open up jupyter labs or jupyter notebook either though anaconda navigator or terminal. 
3. Go to the repository directory

Intro.ipynb
