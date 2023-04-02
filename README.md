# # Title [How to Choice a Good Title?](https://www.nature.com/articles/s41562-021-01152-2)
## Project information
- **Author**: [First Name][Last Name], [Major], [Class], Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set No. or Final Project for [COMPSCI/ECON 206 Computational Microeconomics, 2023 Spring (Seven Week - Second)](https://ce.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: [How to Acknowledge?](https://www.scribbr.co.uk/thesis-dissertation/acknowledgements/)
[notes: please include all professors, students, and staff who have contributed to your completetion of the project.]
- **Project Summary**: 
  - [Summarize the Background/Motivation]
  - [Research Questions]
  - [Application Scenario]
  - [Methodology]
  - [Results]
  - [Intellectual Merits and Practical impacts of your project.]
  
   
Note: please insert the screenshot of the answers to your research question by ChatGPT. The methodology that you use to address the research questions must be more innovative than both the current literature and ChatGPT. 

## Table of Contents

- model
- code
- spotlight
- more about the author
- references

### Model
- Game environment
The trust game involves two players playing a psychological game that is based on the following assumptions: first, they are both rational and will not act out of expectation for any reason other than profit; Secondly, they cannot communicate with each other in words, and all information must be acquired for the capture of the game process and hidden information. Therefore, there is no case that two people consult each other and reaching the so-called optimal solution. Secondly, they are people who follow the rules of the game and don't introduce behaviors that disrupt the structure of the game and lead to non-standard outcomes; In the end, they started with 500.

Based on these three premises, two people must play the following game:
1. Player A puts a sum between 0 and 100 into a third-party bank.
2. Player B deposits between 0 and 100 into A third-party bank without knowing how much Player A has invested.
3. Start judging:
(1) If player B puts in less than Player A puts in minus 25, Player B gets all the money in the bank. (The minimum value is 0)
(2) If player B puts in more money than player A puts in minus 25 and less than player A puts in plus 25, both players get 200 each.
(3) If player B puts in more money than Player A puts in plus 25 and less than Player A puts in plus 25, Player A withdraws all the money in the bank. (The maximum is 100)
(4) If player B puts in more money than player A puts in plus 25, both players lose all their money in the bank and the game ends.
(5) If both players put in zeros, players A and B lose all their money and the game ends.
In this game, the number from 0 to 100 is equally divided into four parts, which are respectively used to represent the four intervals that players may choose during the game. The purpose is to detect whether two people will choose the safest way of cooperation without knowing each other's cooperation willingness and behavior information or choose not to cooperate, but to gain benefits by taking risks.

Possible strategies for Player A:
1. Win-win cooperation: First of all, according to the rules of the game, if two people choose to cooperate, they will inevitably achieve the maximum benefit of the game, which is at least 200 rewards twice the game cost. It is not difficult to achieve this outcome, and it is only necessary to choose a number between 25 and 75 to ensure cooperation, assuming that the other party is also willing to cooperate. (Since this is a symmetric range of 50, Player B only needs to select 50 to succeed, provided that case (2) is achievable.)
2. Risk minimization: If Player A does not believe that player B will choose to cooperate with him, then putting in 0 is the safest thing to do. In this case, first of all, situation (1) cannot be achieved, and B cannot gain greater benefits by betraying cooperation; Case (4) It is possible that if player B puts more than 50 into the bank, he loses all the money he puts into the bank, and player A loses nothing; And case (3) is maximized. If Player B invests less than 50, then player A can get all of Player B's investment bank at no cost; If case (2) is achieved, then player A gets 200 at no cost (in fact, I think this is the way to maximize the benefits, provided Player B can choose a number between 1 and 25. However, if player B and player A both expect to gain 200 with zero cost, then they will suffer the greatest loss, which is the case (5).
In either case, if player A chooses to invest 0, then player A's risk is minimized if Player B invests non-0.
3. Alternative risk minimization methods: As I mentioned in the risk minimization method if player A chooses to invest 0, A and B are likely to achieve the situation (5). To avoid this risk, player A can also invest 1, which may cause situation (1) and make him lose the money invested in the bank, but considering the avoidance of situation (5), this is an alternative to the risk avoidance plan.

Possible strategies for Player B:
1. Win-win cooperation: First of all, according to the rules of the game, if two people choose to cooperate, they will inevitably achieve the maximum benefit of the game, which is at least 200 rewards twice the game cost. It is not difficult to achieve this result. If you believe that the other party is willing to cooperate, you only need to select 50 to ensure cooperation. (y because player A will inevitably choose a number between 25 and 75, and the symmetry of 50 is the best cooperation range between 0 and 100.)
2. Risk minimization scheme: If Player B does not believe that player A will cooperate with him, then he is in the same situation as Player A. Choosing 0 is the safest scheme for him.
3. Alternative risk minimization method: Like Player A, if Player B is worried about the occurrence of scenario (5), investing 1 in the bank is undoubtedly the safest option.
4. Gambler's scheme: Different from Player A, in addition to the cooperation scheme and risk minimization scheme, Player B can choose to invest A number less than 25 to get all of Player A's funds. (If player A is unwilling to cooperate, then he must put in A number between 50 and 100 because Player A wants to avoid the situation (3) in the first place, then he must put in a number large enough to ensure this.)

Pay-off:
Based on all of the above solutions, there are several possible scenarios for this game:
1. Win-win situation: If Player B and Player A trust each other and Player A chooses to put in a number between 25 and 75, and Player B chooses to put in 50, then both players will receive a reward of 200.
This kind of profit is not the most, because both of them have spent some cost to get 200, but this situation is the safest among all the schemes to get 200, after all, if they choose to invest 0, they will have to face the risk of the situation (5).
2. Maximum loss case: If two people choose to invest 0 to obtain 200 net profit, the outcome (5) will trigger, resulting in both of them losing all of their funds. The triggering premise of this case is not that two people don't trust each other, but that both of them are motivated by their interests rather than the interests of the team.
3. General outcome: Player B puts in less than Player A puts in minus 25, and Player B gets all the money in the bank. (Player A puts in a number between 50 and 100, and player B puts in a number under 25.)
Player B puts in more money than player A puts in plus 25 and less than player A puts in plus 25. Player A takes out all the money in the bank. (This situation is almost impossible to achieve because if both players are rational, but player A and Player B have a serious information gap, it is difficult for player B to put in a number greater than 50 under this unfair premise.)

Concept of solution:
Based on the above analysis and reasoning, if two people trust each other and are willing to cooperate, then it is clear that player A putting in a number between 25 and 75 and player B putting in 50 is the safest way to get 200; However, if player A does not trust player B, they may choose to put in a zero or a one to reduce the risk they may face. It is unfair that if Player B wants to get all of Player A's money, he only needs to invest a small number less than 25 to achieve situation (1), and even if Player B's plan fails, his loss will only be less than 25. But if player A wants to get all of Player B's money through the gambler's game, he must put in A number between 50 and 100. If Player A's scheme fails, his loss is greater than 50.

Evaluation:
Efficiency: The benefit of this game is relatively high. Compared with the initial 100 funds of two people, if two people can get 200 rewards through win-win cooperation, the final net profit will be at least 50%. If two people choose the risk reduction option, they can get a return of 200 at zero cost.
Of course, if they both want to speculate, the return will be zero and the net loss will be achieved.
Fairness: Objectively, the game is unfair to player A, because if Player A wants to get all of Player B's money through the gambler's game, he must put in A number between 50 and 100. If Player A's scheme fails, his loss will be greater than 50.
If Player B wants to get all of Player A's money, he only needs to invest a small number less than 25 to achieve situation (1), and even if Player B's plan fails, his loss will only be less than 25.
Of course, if two people choose to cooperate, this injustice will be eliminated.


### Code
- Game Environment
- Strategic plays
- Equilibruim Evaluations: e.g. belief, strategy, and payoffs
- oTree Experimental Code 


### Spotlight
The ultimatum game shows that in a game of games, players may be more willing to give up their interests to punish unfair distribution or wrong behavior (Lowe). This paper challenges the rational person hypothesis, proving that the responder should agree if the proposer allocates a few resources to the responder, which cannot be universally verified. The paper proposes that in practical experiments, only when sufficient resources are allocated to the responder, can the allocation scheme be passed.
In the experiment, the first subject is given 100 marks, and the subject decides how many marks to give to the second subject. If the second subject is unhappy with the allocation and chooses to reject the offer, the two receive no money. If, according to the rational man hypothesis, any amount of money provided to the second subject would be more beneficial than no money at all, then the second subject must accept the first subject's proposal. However, in the actual experiment, in the cases where the money was not split 50/50, the proposer's proposal was responded to only 37 percent of the time (Lowe). In the second week of the experiment, the proposers became more stingy, and in this more unequal distribution, the proposal acceptance rate dropped to 32 percent (Lowe), which is inconsistent with the hypothesis of rational economic man.
These observed behaviors are based on two kinds of psychology:
(1) First of all, before the experiment, the experimental group put forward the hypothesis of equitable distribution, that is, if the first subject is willing to allocate half of the fund to the second subject, the second subject should agree to this proposal. In real-world studies, however, even when the first subject made a fair distribution proposal, the response was only 70 percent of the time. The reason was that the second responder believed that he did not get the initiative in the game. They could not choose a convenient time and place to determine the occurrence of this phenomenon, so it was difficult to make adequate preparations. When compared with the first subject, they thought that the mechanism of the experiment itself was unfair, so they refused to accept the proposal even if it was given to them (T. Friedman and E. Metros).
(2) Secondly, there is a kind of revenge mentality among the responder and proposer, which is the opposite principle of the rational economic man mentioned above. In the experiment, if the first subject made a proposal that was unfairly distributed, respondents became angry at the distribution and were reluctant to play the game, even if it meant they didn't get any money, and they were willing to pay a price to punish the privileged first proposer. Similarly, the proposer would feel angry if his proposal was rejected. In the paper, the author suggested the possibility that the proposer felt his privilege was violated or his authority was questioned and therefore wanted to retaliate against the second subject by making the assignment more unfair. This paper holds that if this kind of psychology is applied in the real market, it may lead to disgusting competition, but it also holds that the deterioration of the supply and demand relationship will not be widespread in the real market, because in this experiment, the experimenter only studied the activities of one proposer and one responder. In the real market, competition will be formed among multiple suppliers. They may not choose a more unreasonable price due to retaliation against their downstream market, which means that their market share will be seized by their competitors. Such supply-side competition may undermine the second psychology.
There are two distinct differences between this psychology and those mentioned in backward induction:
(1) In backward induction, the subject determines what behavior he or she should perform in the penultimate step by predicting the behavior in the last step (Aumann). The premise of this backward reasoning is based on the assumption of rational economic man, that is, the subject wants to obtain the maximum benefit in each step. For example, during the game, both subjects would not pay money because they suspected that the opponent was not willing to pay money, so cooperation could not be reached in the end. The theory is that both men want to maximize their profits. However, in the game I designed, for example, I only proposed two hypotheses in the game. The first one is the cooperation hypothesis. If a subject thinks that another subject is willing to cooperate, then this subject will be willing to give the amount of money in the range of 25 to 75. The second is the risk minimization hypothesis. If the first subject does not believe that the other subject is unwilling to cooperate with him, he will choose to give 1 to reduce his own risk. However, using the psychology of the ultimatum game in this paper, I think that the first subject is more likely to choose a number between 0 and 25, because if the second player wants to cheat the first player out of all his money through the case (1), he will most likely choose a number between 0 and 25, So it's possible that the first subject will feel angry about this assumption and will want to punish the second subject for dishonesty by choosing from 0 to 25. This is entirely possible in practical experiments, however, based on the hypothesis of rational economic man in backward induction, this possibility has not been discussed.
(2) The second difference is that there is a kind of expectative ness in backward induction, which is illustrated here. Suppose an assembly line worker is promised an extra wage for every day he produces a good product if he chooses to work 10 extra days: 100 if the product is good, 50 if the product is bad. Of course, he gets zero for the day if he chooses not to work overtime.
We reasoned by backward induction.
On day 10, he gets 100 for making a good product, 50 for making a business trip product, and 0 if he doesn't work overtime. Of course, he will choose to work overtime.
On day nine, he has a 25 percent chance of making a bad product for two days, so he gets 100; Of course, there's a 25 percent chance of making a good product for two days, so that's 200. So he's still going to work overtime because there's a 25 percent expectation for 200.
By the same analogy, the employee will inevitably choose to work overtime, even if the product is always poor.
In the ultimatum game, however, the effect of this expectation on the game was relatively small, because if it had a significant effect, the second responder would have accepted the offer anyway, since accepting the offer would have meant that the first subject's offer had been met, potentially increasing the next week's earnings. In this case, the second subject will choose to accept the first subject's offer anyway.
The opposite is true, which means that expectations play a smaller role in the ultimatum game.
In "Mastering the game of Go with deep neural networks and tree search ", the author uses the learning logic of deep neural networks and Monte Carlo tree search (Silver). The deep neural network is a feedforward network based on the interconnection between neurons, which has strong expression and generalization ability (Mnih). In the process of model building and reinforcement learning, deep neural networks can be used to represent value function, strategy function, and other key functions. At the same time, an algorithm has the advantage of a smaller error, because the algorithm can constantly update the parameters in the network.
The Monte Carlo tree search algorithm is a kind of algorithm based on simulation and search, which is widely used in the game, planning, and decision-making (Browne). In reinforcement learning, the Monte Carlo tree search algorithm can be used to select the best action or strategy and estimate the value of the expected reward or value function by simulating and evaluating different states and actions many times, to guide the decision-making and action selection of reinforcement learning.
The game environment of this paper is Go. In this paper, the author uses a deep neural network to estimate the value of pieces in each position and how to make decisions, and constantly uses the Monte Carlo algorithm to select the best position to play chess. Eventually, this model outperformed human players and other go programs.
As for how such algorithms can be used to build trust between humans, I think the biggest advantage of these two algorithms is that they can more accurately estimate the judgments that humans are likely to make in decision-making activities. As I mentioned earlier, the reason why backward induction or ultimatum can't achieve a 70% cooperation rate is that there is a state of misinformation between people, Leading the second subject to generally believe that the first subject had some kind of privilege or that their private interests had been violated (although I don't think private interests were violated in the ultimatum game, because none of them received any money before the results of the game were published, if we had to say that someone's private interests had been violated, I prefer to think that the private interests of the proposers were violated, because they had control of 100 marks at the beginning of the experiment, and it was the responder's lack of cooperation that caused them to lose 100 marks. Either way, however, it is the result of unequal information and distrust of one's partners.) If we can use the analysis and calculation of the model to accurately capture the decisions that each player may make and the consequences that they may face after making those decisions, whether in backward induction or ultimatum, the responder or the second player will likely move in a cooperative direction. In a word, I think the greatest significance of these algorithms is that they can provide complete data on the possible behaviors of partners, to help some people in the responder position trust their partners more or trust whether their behaviors can help them get the maximum benefits in the current situation. At the same time, I think this reduction in information is a deterrent, and the first player should not feel that his privilege is being violated at all, because both players should have an equal chance to cooperate and have a say in the game. This privilege is a product of the flaws in the structure and rules of the game, and there will always be some proposer who wants to cheat more money through poor information. If this information gap can be reduced, so too will the number of such speculators.


Works Cited
Aumann, Robert. Backward Induction, Knowledge, and Common Knowledge. 2019.
Browne, Cameron. “A Survey of Monte Carlo Tree Search Methods.” 2017.
Lowe, Ryan. “Multi-Agent Actor-Critic for Mixed Cooperative-Competitive Environments.” 2017.
M. Kreps, David. Backward Induction and Common Knowledge of Rationality. 2019.
Mnih, Volodymyr. Playing Atari with Deep Reinforcement Learning. 2019.
Silver, David. “Mastering the Game of Go with Deep Neural Networks and Tree Search” by David Silver et Al. (2016). 2016.
T. Friedman, Alice, and Susan E. Metros. “Pirate Games: Creating a Fictional World for Learning.” 2018.


### More about the Author
- headshot
- self-introduction
- Final reflections 
  - intellectual growth
  - professional growth
  - living a purposeful life

### References

- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```

