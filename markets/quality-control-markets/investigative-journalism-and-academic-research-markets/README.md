---
description: Overview of Olas Investigative Journalism & Academic Research Markets
---

# Investigative Journalism & Academic Research Markets

Olas introduces the Investigative Journalism & Academic Research Markets to redress the undervaluation of journalistic and scientific contributions. Using a blend of **public subsidies**, **prediction markets**, and retrospective public goods funding, Olas aims to fairly reward impactful work. This market revolves around aligning rewards with the societal value of these crucial efforts. It encourages not only funding but also verification, maintaining the integrity of shared information. Participants, including Content Contributors, Investors, Bettors, and Tippers, engage in an inclusive process—from proposing questions to closing the market. This comprehensive framework ensures equitable compensation while prioritizing validation and assessment of societal impact post-resolution, setting new standards for fair recognition of critical research and investigative endeavours.

<figure><img src="../../../.gitbook/assets/Investigative Journalism and Academic Research Market.png" alt=""><figcaption><p>Figure 8. Investigative Journalism &#x26; Academic Research Market Overview</p></figcaption></figure>

{% hint style="info" %}
The above diagram incorporates a pivotal '**Above 50% Line**' indicating the **majority** threshold.
{% endhint %}

## 1. Participants

* **Content Contributor**: Journalists or academic researchers who propose a binary YES / NO question.
* **Investor**: Financially backs contributor's chosen side for potential profits.
* **Bettor**: Participates by buying shares tied to their predicted resolution of the question.
* **Tipper**: Allocates funds to the winning side's liquidity as a reward based on the market's final outcome.

## 2. **Mechanics of the Market:**

The market's lifecycle is orchestrated to manage a binary question from proposal to resolution:

* **Question Proposal:** Content contributors propose binary YES/NO questions, seeking funding for their chosen outcome.
* **Funding:** Investors provide initial liquidity, supporting the contributor's predicted outcome. In return, investors receive shares corresponding to the side they back.
* **Market Making via Global Pool Submission:** Contributors seek a match from Olas Global pool for the opposing side, subject to approval through a vote by reputable Olas participants. They can adjust strategies or seek additional donations within a deadline if funds are insufficient. The global pool also acquires shares aligned with the opposing side when it matches funding.
* **Market Dynamics:** The market begins with balanced positions on both sides, allowing participants to purchase shares reflecting their predictions.
* **Share Pricing:** Dynamic share prices are influenced by liquidity and YES/NO proportions.
* **Interrogation and Rebuttal:** Content contributors present evidence, followed by a period for arguments. Bets continue during this phase.
* **Market Closure:** Predefined deadline conclusion establishing final share prices.
* **Outcome Determination:** Binary question resolution, deciding winners based on the majority position.
* **Resolution and Payouts:** Above 50% outcome pays long investors; below 50% pays shorts. This includes investors, the global pool, and the journalist who proposed the question, based on the shares they hold. Excess funds return to the pool and donors.
* **Retroactive Rewards and Tipping:** Post-market, contributions earn tips, appreciating precision and societal influence.
* **Global Pool Management**: Subsidies and donations are considered the short side of the market. Unused funds return to sources, maintaining fairness and rewarding accurate predictions.

## 3. Financial Calculations

The market employs a set of financial formulas that govern share pricing and liquidity, crucial for the market's operation:

### **3.1 Settlement Share Price / Current Share Price**:

#### Relative Market Ratio Change in Percentage &#x20;

$$\boxed{   \Delta \% RMR \, = \, \dfrac{ \big| Final \, Market \, Ratio \, - \, Initial \, Market \, Ratio \big|}{ Initial \, Market \, Ratio}}$$

\
$$\Delta \% RMR \, = \, Relative \, Market \, Ratio \, Change \, in \, Percentage$$

#### **Winning** Settlement Share Price (i.e. If the **Final** Market Ratio is **above** 50)

$$\boxed{  Winning \, Market \, Share \, Price \, = \, \dfrac{ LQ_w + LQ_L \times \Delta \% RMR}{ T_w}}$$

\
$$LQ_w \, = \, Winning \, Side \, Liquidity$$\
$$LQ_L \, = \, Losing \, Side \, Liquidity$$\
$$T_w \, = \, Total \, Winning \, Shares \, Issued$$

#### **Losing** Settlement Share Price (If **Final** Market Ratio is **below** 50)

$$\boxed{  Losing \, Market \, Share \, Price \, = \, \dfrac{ LQ_L - LQ_L \times \Delta \% RMR}{ T_L}}$$

\
$$LQ_L \, = \, Lossing \, Side \, Liquidity$$\
$$T_L \, = \, Total \, Losing \, Shares \, Issued$$

These formulas ensure that share prices reflect the market's liquidity and the proportionate belief in the outcome of the proposed question.

### 3.2 Settlement

The settlement process is transparent and entails:

* **Profit Distribution**: Profits are calculated for holders of the winning shares using the settlement share price formula denoted above.
* **Return of Funds**: Any leftover funds in the given market's liquidity pool are returned to their origin, ensuring no misuse of resources.

### 3.3 Incentive Structure

The incentive structure is designed to:

* Guarantee base-level rewards through public subsidies.
* Enhance rewards through retroactive funding as societal value becomes evident.
* Encourage thorough vetting of information due to financial stakes in the market outcome.

## 4. Example of Market Dynamics

The market is initiated when a journalist proposes a binary question. Investors then fund the contributor's chosen side of the proposition, while the global pool matches this funding the opposite side, establishing initial liquidity and a 50:50 market balance. A deadline for the market resolution is set, and the market opens for public betting.

\
For starters let's assume the following things:

* 1 share value is $100 ( this would keep changing depending on the bonding curve but for the sake of this example, let's assume it's fixed ).
* The journalist takes the "YES" side and stakes $500 i.e. the Journalist is issued 5 YES shares.
* Investors invest $1000 in the content contributor's market side and are issued 10 YES shares in return.
* The Global Pool matches "NO" side shares with $1500. Consequently, 15  NO shares are issued to the Global Pool.

#### **Initial Market Values**:

* YES: NO initially in equal 50 : 50 ratio with $1,500 liquidity each
* Initial Total Liquidity: $3,000

#### **Market Activity**:

* Bettor A buys $80 worth of NO shares.
* B buys $200 worth of YES.
* C buys $20 worth of NO.
* D buys $1,500 worth of YES.

#### **Market Values After Above Market Activity:**

* Total Liquidity: $3,000 (initial) + $1,800 (new) = $4,800
* Updated YES Ratio: $3,200 / $4,800 = 66.67%
* Updated NO Ratio: $1,600 / $4,800 = 33.34%
* Market shifts from YES : NO 50 : 50 to 66.67 : 33.37 respectively

#### Financial Calculations

The financial implications of the market shift are calculated as follows:\
\
$$\Delta \% RMR \, = \, (| 66.67 \, - 50 |)/50 \, = \, 33.34\%$$

#### **Loss Calculation for Minority shareholders**:

$$Loss \, = \, (\, Final \, Ratio - Initial \, Ratio \,) / 50$$\
$$Monetary \, Loss \, : \, \$1600 \, \times \, 33.34\% \, = \, \$ 533.44 \, loss$$

\
$$Losing \, Settlement \, Share \, Price \, = \, \dfrac{ LQ_L - LQ_L \times \Delta \% RMR}{ T_L}$$\
$$= \, \dfrac{\$1600 \, - \, \$1600 \, \times \, 33.34\%}{15} \, = \, \$71.11$$

#### **Reward Calculation for Majority share Holders**:

$$Reward = total \, majority \, share \, Liquidity \, + \, Loss \, Liquidity \, from \, the \, losing \, side$$\
$$Reward = \$3200 + \$533.44 (losses \, from \, minority \, share \, holders) = \$3,733.44$$

\
$$Winning \, Market \, Share \, Price \, = \, \dfrac{ LQ_w + LQ_L \times \Delta \% RMR}{ T_w}$$\
$$= \, \dfrac{\$3200 \, + \, \$1600 \, \times \, 33.34\%}{15} \, = \, \$248.89$$

#### **Content Contributor's Payouts:**

$$Settlement \, share \,price * Number \, of shares \, held$$

Since the contributor aligns with the majority share, the Settlement share price = $248.89\
$$Content \ Contributor\ Payout \, = \, 248.89 \, \times \, 5 \, = \, \$1244.45$$

This illustrates how market liquidity is influenced by new investments and how the distribution of funds reflects the shift in market consensus.

The market's liquidity is influenced by new investments, reflecting shifts in consensus. Its design inherently resists manipulation, requiring market ignorance for profitability. This highlights the market's predictive power, surpassing traditional forecasting methods like peer review. Olas' Investigative Journalism & Academic Research Markets aim to incentivize undervalued journalistic and research work by leveraging collective intelligence through public subsidies, prediction markets, and retroactive rewards. This system establishes a sustainable, fair economic model for this valuable societal work.
