---
description: Unbiased Peer Review
---

# Review Markets

The Academic Reporting Market involves two essential roles. **Methodology Checkers** are responsible for identifying methodological or statistical errors and are rewarded based on their findings. **Judges** assess the inaccuracies pointed out by these checkers, determine their validity, and are rewarded accordingly.

After the scientists submit their research, the methodology checking process begins. During this period, anyone can point out an **inaccuracy** in the research. These inaccuracies are called **Initial Methodological Issues (IMIs)**.

<figure><img src="../../../.gitbook/assets/olas review markets diagram.png" alt=""><figcaption><p>Figure : Olas Review Markets</p></figcaption></figure>

Next, a random selection is made from a pool of scientists specialising in the relevant article field, having a minimum reputation score, and having requisite funds in their account. Further a few open seats can be filled by those with proven ability with scientific and statistical methods. Unlike the Fact Reporting Market, there is no lead judge to collate issues as it is envisaged the issues raised will be fewer and more complex in this market.&#x20;

The Judges give a secret vote for **Severity** and **Accuracy Scores** for each of the issues. The Severity Score denotes the level of importance of the inaccuracy found within the research, and the Accuracy Score denotes the judge's confidence in the issue raised. &#x20;

Once the judges finish scoring and the outcomes are revealed, the rewards for Methodology Checkers, Judges, and Content Contributors are determined based on the outcomes.

### &#x20;**1.1. Methodology Checkers Reward**

Methodology Checkers are rewarded based on the **accuracy and** **severity** of their contributions.

* **Severity:** A score from 0-10 is assigned by a Judge to a methodological issue, which signifies its severity.
* **Accuracy:** A score from 0-10 is assigned by a Judge to a methodological issue, which signifies the Judge's belief in the accuracy of the issue raised.

The Methodology Checking Reward is calculated using the following formulas:\
\
$$\boxed{S_G = { \left( M_S \times W_S) + ({M_A} \times {W_A} \right) } }$$

\
$$S_G\, = \, General \,Score$$\
$$M_S\, = \, Median \, of \, Severity \, Scores$$\
$$M_A\, = \, Median \, of \, Accuracy \, Scores$$\
$$W_S \, = \, Severity \, Weight$$\
$$W_A \, = \, Accuracy \, Weight$$\
\
Each Methodology Checker's **General Score** is calculated using a weighted formula that takes into account the **severity** and **accuracy** of their submission.\


$$\boxed{ S_T \, = \, \displaystyle\sum_{i=1}^N  \, S_{Gi}\,}$$\
\
$$S_T\, = \, Total \, Score$$\
$$N\, = \, Number \,of \, Methodology \, Checkers$$

The **Total Score** is calculated by summing the rewards of all Methodology Checkers, providing a baseline for proportional reward distribution.\


$$\boxed{ R_{MC} \, = \, \dfrac{ S_{G} }{ S_T} \times \, TR_M}$$\
\
$$R_{MC}\, = \, Methodology \,Checker \,Reward$$\
$$TR_M\, = Total\,Reward \,of \, Methodology \, Checkers$$

Once the Total Score is determined, the **Methodology Checkers' rewards** are calculated proportionally.

### **1.1.1 Example** Methodology **Checking Reward Calculation**

In this example, predefined **severity** and **quality** weights from the protocol are used, along with a **fixed** **reward** for the article.

| Judging Panel Variables              | Values   |
| ------------------------------------ | -------- |
| Severity Weight                      | 0.4      |
| Accuracy Weight                      | 0.6      |
| Total Reward of Methodology Checkers | 100 USDC |



Subsequently, all judges provide **Severity** and **Accuracy** Scores for the question. The **median** of these scores is used.

<table><thead><tr><th width="303.3333333333333">Methodological Issues</th><th width="232">Median of Severity Scores</th><th>Median of Accuracy Scores</th></tr></thead><tbody><tr><td>MI1</td><td>6</td><td>7</td></tr><tr><td>MI2</td><td>8</td><td>8</td></tr><tr><td>MI3</td><td>5</td><td>7</td></tr></tbody></table>

The general score is calculated for all the methodological issues.

{% hint style="info" %}
General Score = (Median of Severity Scores × Severity Weight) + (Median of Accuracy Scores × Accuracy Weight)
{% endhint %}

_General Score MI1 = \[(6 x 0.4) + (7 x 0.6) ] = 6.6_

_General Score MI2 = \[(8 x 0.4) + (8 x 0.6) ] = 8_

_General Score MI3 = \[(5 x 0.4) + (7 x 0.6) ]  = 6.2_

_**Total Score = 6.6 + 8 + 6.2 =**_** 20.8**\


{% hint style="info" %}
Reward Per Methodology Checker = (General Score / Total Score) x Total Reward of Methodology Checkers
{% endhint %}

Methodology _Checker 1 Reward = (6.6 /_ 20.8 _) x 100 = $_31.730

Methodology _Checker 2 Reward = (8 /_ 20.8 _) x 100 = $_38.4615

Methodology _Checker 3 Reward = (6.2 /_ 20.8 _) x 100 = $_29.8076

\
The final distribution of Methodology Checker Rewards is as follows:

<table><thead><tr><th width="312.3333333333333">Methodology Checkers</th><th>General Score</th><th>Reward</th></tr></thead><tbody><tr><td>Methodology Checker 1 </td><td><em>6.6</em></td><td>31.730</td></tr><tr><td>Methodology Checker 2 </td><td><em>8</em></td><td>38.4615</td></tr><tr><td>Methodology Checker 3</td><td><em>6.2</em></td><td>29.8076</td></tr></tbody></table>

### **1.2. Judges Reward**

To participate in the Judging Panel, each Judge must stake a certain amount of funds. Judges must either use funds obtained through the funding mechanism that are currently locked in the protocol or stake their own funds. The amount they stake depends on the initial amount the content contributor staked in the article.

Judges are rewarded for each methodological issue (MI) based on the **proximity** of their **accuracy score** to the **median** of all judge's accuracy scores. The use of median ensures that rewards are distributed based on a score that is resilient to outliers.

The Judging Reward is calculated using the following formulas:\


$$\boxed{S_P=P_{max}\, − ∣J_A−M_J∣}$$\
\
$$S_{P}\, = \, Proximity \,Score$$\
$$P_{max}\, = \, Max \,Proximity$$\
$$J_A\, =  \, Judge's \, vote\, on \, Accuracy \,Score$$\
$$M_J\, = \, Median \,of \,All \, Judges's \, Accuracy \,Score$$

The **Proximity Score** reflects how close a judge's score is to the **median**, which is the middle score of all judges' scores when sorted. The closer a judge's score to the median, the higher their Proximity Score will be.\


$$\boxed{ S_{P_{total}} = \, \displaystyle\sum_{i=1}^N ( S_{Pi})}$$\
\
$$S_{P_{total}} = \, Total \, Proximity \,Score$$\


The Total Proximity Score is the sum of all individual Proximity Scores from each judge.\


$$\boxed{R_{Ji}=  ​\frac{S_{Pi}}{S_{P_{total}}}  × R_{J_{total}}}$$

\
$$R_J\, = \, Judge's \,Reward$$\
$$R_{J_{total}} \, = Total\,Reward \, available \, for \, Judges$$\
\
\
Each Judge's Reward is calculated by taking their individual Proximity Score and dividing it by the Total Proximity Score, which is then multiplied by the Total Reward available for the methodological issue.

{% hint style="info" %}
When all the judges vote with the same accuracy score, they get back their original staked amount.
{% endhint %}

### **1.2.1 Example Judging Reward Calculation**

In this example, we use a panel of 5 judges, though actual panels may have more judges. Each judge stakes $10 to evaluate a particular methodological issue(MI) in an article.

| Variables    | Values              |
| ------------ | ------------------- |
| Total Judges | 5                   |
| Total Reward | $50 ($10 Per Judge) |

The following table shows the distribution of accuracy scores for a specific methodological issue, indicating judge's confidence in the statement's accuracy.\


| Judges | Accuracy Scores Given By Judges |
| ------ | ------------------------------- |
| J1     | 10                              |
| J2     | 8                               |
| J3     | 4                               |
| J4     | 3                               |
| J5     | 2                               |



The reward calculation process for Judges consists of the following steps:

*   **Establishing the Median Score:**\


    We sort the given accuracy scores and determine the median value. The median represents the middle value when there is an odd number of observations.\




    {% hint style="info" %}
    Median(Odd) = (n+1)/2th data point
    {% endhint %}

    \
    _Sorted Scores: 2, 3, **4**, 8, 10_

    _Median Score = 4_\

*   **Calculating Proximity Score for Each Judge:**\


    {% hint style="info" %}
    Max Proximity(Max Score - Min Score) = 10 - 0 = 10\
    Proximity Score = Max Proximity - |Judges Score - Median Score|
    {% endhint %}

    \
    _Judge 1 Proximity Score = 10 - |10 - 4| = 10 - 6 = 4_\
    \
    _Judge 2 Proximity Score = 10 - |8 - 4| = 10 - 4 = 6_\


    _Judge 3 Proximity Score = 10 - |4 - 4| = 10 - 0 = 10_\


    _Judge 4 Proximity Score = 10 - |3 - 4| = 10 - 1 = 9_\


    _Judge 5 Proximity Score = 10 - |2 - 4| = 10 - 2 = 8_\

* **Calculating the Total Proximity Score:**\
  _Total Proximity Score = 4 + 6 + 10 + 9 + 8 = 37_\

*   **Calculating Each Judge’s Reward:**

    Assuming a total reward pool of $50($10 Per Judge)



    {% hint style="info" %}
    Reward = (Proximity Score / Total Proximity Score) x Total Reward
    {% endhint %}

    \
    _Judge 1 Reward = (4 / 37) × $50 ≈ $5.41_\


    _Judge 2 Reward = (6 / 37) × $50 ≈ $8.11_\


    _Judge 3 Reward = (10 / 37) × $50 ≈ $13.51_\


    _Judge 4 Reward = (9 / 37) × $50 ≈ $12.16_\


    _Judge 5 Reward = (8 / 37) × $50 ≈ $10.81_

The final distribution of Judge Rewards is as follows:

| Judges | Proximity Score | Reward |
| ------ | --------------- | ------ |
| J1     | 4               | $5.41  |
| J2     | 6               | $8.11  |
| J3     | 10              | $13.51 |
| J4     | 9               | $12.16 |
| J5     | 8               | $10.81 |

### 1.3 Content Contributor Reward

Content Contributors in Olas have the opportunity to apply for funds through periodic funding rounds. In these rounds, they receive donations from active donors. The amount of donations each contributor receives plays a significant role in the quadratic funding mechanism, which determines the funds matched to each contributor. Upon securing these funds, contributors' accounts will have these funds **locked**. \
\
A unique feature of Olas is that contributors stake an amount on each article they write, using their **locked funds**. This staking process represents a commitment to the **quality** and **reliability** of their content, as it involves a direct financial stake in the success and **accuracy** of the article. Alternatively, contributors can choose to stake their **own** money instead of participating in funding rounds. This can enhance their reputation within the protocol and improve their chances of achieving better results in future funding rounds.

\
The reward for Content Contributors is calculated based on the following factors:

**Article Score:** The article score is calculated by summing the median of accuracy scores of all methodological issues and then dividing it by the maximum possible accuracy score. For instance, with accuracy scores of 9, 7, and 2, the article score is 18 out of a maximum of 30(assuming max possible accuracy score is 10), resulting in a score of 0.6, which equates to 60%.

\
$$\boxed{S_{AR} = \frac{{\sum_{i=1}^N ( \, M_{A_{MI_{i}}})}}{{N \,\times \,S_{A_{max}}} }}$$\
\
$$S_{AR}\, = \, Article \,Score$$\
$$M_{A_{MI}}\, = \,Median \, of \,the\,Accuracy \, Scores \,for \,a \, Methodological \,Issue$$\
$$N\, = \, Number \,of \, Methodological \, Issues$$\
$$S_{A_{max}}\, = \, Maximim \,Possible \, Accuracy \,Score$$\


**Deferred Payout:** Irrespective of the article's score, content contributors are guaranteed 20% of their staked amount as a Deferred Payout. This ensures that contributors receive a fixed portion of their stake regardless of the article score. For example, if a contributor stakes $100, the deferred pay is $20 (20% of the staked amount).

\
**Evaluated Stake Payout:** After the **deferred payout**, the remaining **80%** of the staked amount is subject to the article's score evaluation. This part of the stake is dependent on the **article score.** For instance, if a contributor stakes $100 on an article and receives a score of 70%, then 70% of the remaining $80 stake, which is $56, is unlocked and made accessible to the contributor.



**Tips Payout**: Contributors receive a **portion of the tips**, given by readers to their articles. The allocation of tips is dependent on the article score. For instance, if an article scores 70%, 70% of the tips go to the contributor, while the remaining 30% is directed to the global pool.\


The total reward for a Content Contributor is calculated using this formula:

$$\boxed{{R_C}= P_D +S_{AR} \, \times \, ( \, P_{E} \, + \, P_T \, )}$$\
\
$$R_C= Total\,Content \, Contributor\, Reward$$\
$$P_D\, = \, Deferred \,Payout$$\
$$S_{AR}\, = \, Article \,Score$$\
$$P_{E}\, = \, Evaulated \,Stake \, Payout$$\
$$P_T\, = \, Tips \, Payout$$

### **1.3.1 Example Content Contributor Reward Calculation**

Let's consider the reward calculation for a content contributor who has invested $200 in their article. Additionally, this article has earned $50 in tips from the tippers. The Judging Panel reviews the article and assigns it a score of 70%.&#x20;

| Article Score(%) | Staked Amount | Tips |
| ---------------- | ------------- | ---- |
| 70%              | $200          | $50  |

We determine the total payout for the contributor by using this simple formula:\


{% hint style="info" %}
Deferred Payout + Article Score x (Evaluated Staked Payout + Tips Payout)
{% endhint %}

\
First, we calculate the Deferred Payout:

_Deferred Payout (20% of Staked Amount) = 0.20 × 200 = $40_

\
Next, we calculate the evaluated stake payout:\
\
_Evaluated Stake = 80%(predefined by the protocol) of Staked Amount_\
\
_Evaluated Stake Payout = 0.80 × 200 = $160_\
\
_Content Contributor's Reward =  40 + 0.7 x (160 + 50)  = $187_

From the entire $250 reward, the contributor earns $152 (deferred payout + evaluated stake payout) from the locked balance and $35 in tips. The global pool will receive $48, which is 30% of the evaluated stake, and $15, which is 30% of the tips.
