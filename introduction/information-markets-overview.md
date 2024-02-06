---
description: Decentralised Collusion-Resistant Quality Control
---

# Information Markets Overview

Olas' information market-based quality control mechanisms are designed with five assumptions in mind:

1. Information supply today is subject to numerous undesirable incentives. &#x20;
2. The way to minimise these incentives is to not only remove human hierarchies from the administration of platforms - as discussed in the previous section - but to also open up the systems of quality control. The two proven mechanisms we have for reliably aggregating information in an open setting are **markets** and **reputation**.
3. Markets are an incredibly effective tool but their efficacy is dependent on them being designed with the specific problem that's to be solved in mind. Otherwise the incentives involved may be sub-optimal.  &#x20;
4. Prediction markets, although evidently a powerful tool with great potential, have generally failed to gain mass adoption outside of betting on sport and to a lesser extent politics. Some of the reason for this is regulation, but another major factor, in our view, is that they require subsidies to entice bettors.  &#x20;
5. The great weakness of open systems is their vulnerability to collusion. Open systems vulnerable to collusion risk devolving into a system just like the one they wish to replace.&#x20;

### Poor Incentives Produce Bad Outcomes

As discussed in the previous section private ownership of information platforms has deleterious effects on information quality. Newspaper owners shape the information that is provided on their platforms via an editorial direction. These owners generally have economic incentives that often run contrary to publishing the truth on certain matters. Further, in the internet age, the requirement to get a click or publish articles agreeable to one's subscriber base introduces incentives that also often run contrary to writing the truth.&#x20;

In the field of science, journals are similarly pressured to publish new and exciting breakthroughs. Further, those with influence over the peer review process also have economic interests that can lead them to influence that process in accordance with those interests.&#x20;

These incentives have a very noticeable effect. Depending on the country, 40-60% of news articles contain factual inaccuracies. This is far too high to be completely accounted for by honest mistakes. In the field of science there is a replication crisis. Over 85% of the findings in scientific papers turn out to be false. There have also been numerous instances of corruption of the peer review process resulting in papers with findings that are uncomfortable for prevailing interests and ideologies being published.&#x20;

What is needed therefore, is not only an ownerless platform as suggested in the previous section, but open non-hierarchical systems of quality control that don't grant positions of power that can be corrupted to anyone.&#x20;

### Open Quality Control Mechanisms

Markets are the most effective tool humanity has for aggregating information. The secret to their success is best described by the "Skin in the Game" thesis. There is no substitute for the prospect of being rewarded for being right and conversely being punished for being wrong for focusing one's mind. As such well-functioning market can be viewed as a truth telling machine that encompasses the views of numerous people with money on the line. There have been numerous studies that have shown prediction markets to be better at predicting outcomes than subject matter experts that don't have money on the line.&#x20;

Thus far, aside from markets, the only other effective quality control tool humanity has is an open context is a reputation system. A reputation score is a shared memory of a person or institution's performance at a certain activity. This shared memory is very useful to prospective customers. Reputation systems thus work on the basis of similar incentives to markets.  The only difference is that changes to a reputation score effects the holder's future earnings whereas changes in the price of a market position affects current profitability. A positive update to a reputation score is likely to result in increased business in the future whereas a negative update normally results in less custom.   &#x20;

### Olas Market Design Considerations

Olas aims to harness both markets and reputation in tandem to produce high quality outcomes. The markets will settle on a view of the quality of a contributor's output and a reputation score will keep track of their historical performance in each of these markets so that prospective donors have clear insight into who is most deserving of donations.&#x20;

However, each sector of information in Olas brings different challenges. The reporting of news generally involves reporting information that is publicly available and thus doesn't require many market participants to verify its accuracy once there is also an incentivised fact checking system.&#x20;

Opinion pieces bring the challenge that the truth is often an unpopular view and those holding that view are disincentivised to bet, particularly when there must be settlement within a reasonable timeframe so the contributor's funds aren't held in limbo for an excessive amount of time - something that in turn would disincentivise contributing in the first place. There's a famous saying in trading that "the market can remain irrational longer than you can remain liquid". In this case, the market can settle before it updates its opinion (becomes rational). Consequently, contrarians with insight are faced with a situation where they've little chance of profiting from their knowledge. In order to remedy this situation we need to implement a mechanism specifically designed for such an undesirable scenario.&#x20;

Investigative journalism and scientific research involve much higher up front costs than the other forms of information that'll be published on the platform. They also unearth a much greater amount of value for society. Given the costs and greater possible rewards, a system that offers greater incentives to funders is required by the former and made possible by the latter. Further, although not all research results in breakthroughs, negative results are extremely useful information for society. For example it's good to know that a certain public authority isn't corrupt or that a certain molecule isn't useful for extending lifespan. It enables us to focus our energies on other areas. With this in mind, the system must reward high quality research regardless of outcome while also providing those that make breakthroughs the opportunity to profit from the value they create for society. &#x20;

### Subsidies

The potential of prediction markets has been known for some time. There have now been numerous studies that show them to be superior to alternative institutions for making predictions. Despite this, as a technology, they remain underused. A large part of the reason for this is that gaining regulatory approval for prediction market applications has been near impossible, although that has changed somewhat recently. However, the lack of success of decentralised prediction markets like Augur and Gnosis that are not subject to regulatory concerns, shows that regulation is likely not the main reason they haven't succeeded.&#x20;

In our view, the main reason is a lack of interest in betting on most topics. Sport and politics are unique in that they involve a widespread tribal emotional attachment to individuals, teams and parties that most other subjects will always fail to match. Further, the betting takes place around high profile occasions that provide natural liquidity events. The emotional bettors that bet with their hearts are essentially providing subsidies to the professionals that bet on the basis of prior probabilities. Such subsidies are lacking for most other topics that don't have the same level of emotional following or event-based outcomes.&#x20;

What's needed to unlock the power of prediction markets therefore is subsidies to informed bettors that collectively can provide very useful predictive insight.&#x20;

### Anti-Collusion Mechanisms

Another potential pitfall with using open market-based systems (or any open system for that matter) is their vulnerability to collusion. The best way of explaining this vulnerability is using the small game-big game thesis.&#x20;

This thesis posits that the incentives involved in small games are always trumped by the incentives in a larger game it is intertwined with. In the context of Olas, the small game is the incentives involved in the prediction market. The big game is the incentives players of that small game may hold outside it in the real world. To be more specific, a company with an economic interest in a large game, such as, let's say, the efficacy of a drug it has a patent for, would be willing to collude with others that hold a similar incentive, or bribe others so that their interests become aligned, to bet on a certain outcome in a market even if they know that outcome to be false. In this case they'd be betting on the drug being effective even if they know from testing that it's not. This can lead to the market (the small game) giving a poor signal so that they'd gain a much larger reward (in the big game).&#x20;

It is imperative therefore that all markets, and therefore the reputation systems that rely on them, have robust anti-collusion mechanisms.

### Olas Information Market Mechanisms Summary

Each market is designed both with its specific requirements and challenges in mind, and with collusion-resistance in mind at every stage.&#x20;

1. **News/Fact Reporting Market**
   * This market features two main roles: **Fact Checkers**, who scrutinise articles to identify inaccuracies, and **Judges,** who evaluate these findings for validity.
   * The process starts with the submission of an article accompanied by a stake by a **content contributor,** followed by an open phase for fact-checking where anyone can submit potential inaccuracies.&#x20;
   * These inaccuracies are then verified by a partially randomly selected panel of judges with self-declared but proven knowledge of the subject matter in question. There are also some open seats that are open to fact checkers with a high reputation score. No two judges will be permitted to sit on the same panel together more than a TBH amount.
   * The work of the fact checkers and judges is subsidised by the contributor's stake and Olas.&#x20;
   * Payouts for contributors are dependent on their score. Payouts for fact checkers are dependent on the judge's views of the issue(s) they raised. Payouts for individual judges are dependent on their proximity to the median judge.&#x20;
2. **Opinion Market**
   * Opinion markets will work through tipping. Every time someone tips an article they will need to fill out a two-question questionnaire. The format of this questionnaire is known as Bayesian Truth Serum and is specially designed to entice people that believe they hold a correct but unpopular opinion into the market.&#x20;
   * The dual-question mechanism asks participants to both take a view of the opinion piece in question and predict the majority's response to the same question. The BTS algorithm then identifies the "surprisingly popular" answer, which is more popular than participants predicted, indicating it may reflect important insights from the crowd.
   * The algorithm both incentivises correct contrarians to participate via the dual-question mechanism and through subsidies from tippers that tip because they like the opinion in question - analogous to bettors in sports.&#x20;
   * Collusion will be minimised by asking tippers to have a unique Olas identity and to make a minimum tip/bet. Further a minimum anti-collusion infrastructure (MACI) protocol will be implemented. There will also be a limit to the amount of tips/bets on opinion pieces an identity can make.
   * Payouts to contributors and bettors will be dependent on the BTS betting result.&#x20;
3. **Investigative Journalism and Scientific Research Markets**
   * These sectors employ a tri-market system. &#x20;
   * Prior to entering a market journalists and scientists will be able raise money from investors as well as donors. The other sectors are limited to donations. Profits will be shared with investors.
   * The first market, which is identical to the News/Fact reporting market, with fact checking and judgment layers, takes a view on the methodology and statistical analysis and a (preliminary) view on the outcome of the study. This ensures good research will receive funding regardless of the findings.&#x20;
   * The second market is entered into if contributors believe they've made a big breakthrough that will be verified by others. They can start a 'replication market' whereby anyone can bet on their result being replicated. Other teams will attempt to replicate the findings for a share of the rewards and a fact checking and judging panel consisting of completely different members to the first one, will judge on the replication attempt findings.&#x20;
   * Payouts will be dependent on the judgements in both markets.&#x20;

