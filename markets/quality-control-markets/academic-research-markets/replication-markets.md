# Replication Markets

In the pursuit of scientific integrity, the Olas protocol introduces **replication** markets—a mechanism designed to enhance the credibility and reliability of scientific findings. It achieves this by incentivising independent efforts to replicate research findings, ensuring that scientific breakthroughs meet rigorous verification and replicability standards.&#x20;

The replication market operates on a simple yet powerful premise: market participants can place bets on whether they believe a piece of scientific research can be independently replicated.&#x20;

If there's a scientific breakthrough, profits from the review market can be staked on the long side of a replication market with a matching short side bet from Olas for starting liquidity. This market will give an excellent signal to the judging teams of the replication attempt(s).&#x20;

Below is a diagram illustrating the workflow of the replication market, from market creation and betting to outcome resolution and payout distribution. This visual guide demonstrates the interconnected processes and roles within the market.

<figure><img src="../../../.gitbook/assets/Academic and Research Market - Page 1 (5).jpeg" alt=""><figcaption><p>Figure 1. Replication Market Overview</p></figcaption></figure>

The replication market serves three fundamental purposes:

1. **Validate Scientific Research**: Encourage the independent verification of research findings to ensure their reliability and reproducibility.
2. **Incentivise Transparency and Integrity**: Create financial incentives that entice the scientific community to engage in replication efforts, promoting a culture of openness and rigour.
3. **Provide Signals to Stakeholders**: Offer valuable insights to researchers, investors, and the broader scientific community regarding the consensus confidence in the reproducibility of specific research findings.

## How It Works

### Market Creation

A replication market is initiated based on a significant scientific finding that the Olas community or a specific entity wishes to validate. The market is structured around a **binary** outcome:

* **Yes**: The research findings can be successfully replicated by independent parties.
* **No**: The research findings  cannot be replicated successfully.

### Betting Mechanism

Market participants can stake their bets on either outcome based on their assessment of the research's **replicability,** with odds fluctuating based on the total amount staked on each side. Each market leverages an escrow smart contract that is deployed at the point of market creation. This contract holds the bettors' stakes securely until the outcome is determined and the market resolves. Upon market resolution, winning bettors can claim their original bet amount plus their rewards.

### Resolution Criteria

After the market closes, the market outcome is determined once a consensus is reached by a panel of new expert judges in order to accurately verify the replication efforts.&#x20;

* **Replication Assessors**: Individuals who attempt to replicate research findings and point out successes or failures in replicating the research. They are akin to **Methodology Checkers** but focus on research replication specifics.
* **Verification Judges**: Independent **experts** who evaluate the claims made by Replication Assessors, determining the validity of each replication attempt. By rigorously assessing the results of replication attempts, these independent experts help uphold the standards of scientific inquiry, ensuring that only the most robust findings are recognised as reliable. The overall outcome of a given replication market hinges on the final judgement made by this panel of experts.

## Replication Market Reward Structure

Once the market resolves, payouts are calculated based on the following factors:

1. **Total Losing Pool Liquidity:** The total losing pool liquidity consists of all bets placed on the **losing** side of the market. The money in this pool will be redistributed to the winners.
2. **Total Winning Pool Liquidity:** The total winning pool liquidity consists of all bets placed on the **winning** side of the market.
3. **Bettor's Stake:** The total amount of funds staked by a bettor on a given side of the market.
4. **Payout:** The pool liquidity is distributed to the bettors who bet on the **winning** side of the market.

The payout for each **winning bettor** can be determined using the following formula:

$$\Large \text{Payout} = \text{Bettor's Stake} + \left( \text{Bettor's Stake} \times \frac{\text{Total Losing Pool Liquidity}}{\text{Total Winning Pool Liquidity}} \right)$$



This formula ensures that the payout is proportional to the amount staked by a bettor and the relative size of the winning and losing pools. It rewards bettors who take risks on less popular outcomes with potentially higher payouts due to a larger losing pool relative to the winning pool. This means that bets placed on outcomes deemed less likely—and thereby riskier—are rewarded more generously when they prove correct. Consequently, each bet is valued based on its merit and degree of risk involved.&#x20;

By offering greater rewards for less popular outcomes, our market mechanism doesn't just compensate for risk—it actively incentivises participants to explore and support hypotheses that may be overlooked or undervalued by mainstream scientific discourse. It encourages market participants to venture into uncharted territories of research, supporting underrepresented studies that could lead to groundbreaking discoveries.

### Example Market Scenario

To illustrate, consider the market based on the paper titled "**The First Room-Temperature Ambient-Pressure Superconductor**". The market will resolve to "**Yes**" if the results regarding LK99 are replicated at least two times by independent researchers unaffiliated with the original authors by a specified deadline. If this criterion is not met, the market resolves to "**No**".

This example illustrates how the payout of this market would work:

* **Total Staked on "Yes" (Winning Pool)**: €10,000
* **Total Staked on "No" (Losing Pool)**: €15,000

Assuming a bettor who placed €100 on "Yes":

1. **Bettor's Stake**: €100
2. **Total Losing Pool Liquidity**: €15,000
3. **Total Winning Pool Liquidity**: €10,000&#x20;

#### Applying the payout formula:

$$\text{Payout} = €100 + \left(€100 \times \frac{€15,000}{€10,000}\right)$$

$$=> \, €100+(€100×1.5)$$

$$=> \,€100+€150=€250$$



In this example, the bettor's payout would be €250. This includes their initial €100 stake plus an additional €150, which represents their share of the total losing pool liquidity, proportionate to their stake in the total winning pool.

## Protocol Benefits

Implementing a replication market within our protocol offers several advantages:

* **Enhanced Scientific Integrity**: By incentivising independent verification, Olas contributes to the advancement of science that is both reliable and universally trusted.
* **Economic Incentives**: Stakeholders can financially benefit from their knowledge and insights into the replicability of research, fostering a more engaged and proactive scientific community.
* **Decentralised Verification**: Through this market mechanism, Olas ensures a transparent, tamper-proof system where replication outcomes are determined by consensus, free from centralised biases.

As we chart new territories in the pursuit of scientific truth, the replication market stands as a testament to Olas' commitment to integrity and reliability. Through the use of societally aligned incentives, Olas aims to redefine the standards of scientific excellence.
