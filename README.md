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
In return:
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
- Posters
- Figures
- Slides
- Presentations
- Review articles
- Media appearance

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

