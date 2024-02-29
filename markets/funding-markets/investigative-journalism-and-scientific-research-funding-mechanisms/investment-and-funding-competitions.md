---
description: Funding High Cost, High Value Public Goods
---

# Investment and Funding Competitions

The relatively large funding costs for these types of contributions require a stronger incentive system than charity to encourage money to flow into the system. Although the economic model will still be based on charity, we believe the significance of the discoveries in this sector will result in large amounts of donations in the form of tips subsequent to publication and evaluation. This in turn will enable contributors to offer investors the chance to share in these donations and make a profit from their investment. Further, given the highly specialised knowledge required for these topics, as well as the fact discoveries in this sector benefit everyone and not just concentrated interests, there is no need for a quadratic funding mechanism to guard against the influence of big money.&#x20;

In light of this we propose a hybrid system analogous to the public-private partnerships we often see in many industries today. As in the other information sectors, Olas will make a pool of funds available for Investigative Journalism and another available for Scientific Research every quarter. There will also be funding rounds. However, unlike the other sectors, funding will only be granted once a market has given a research project a score. Further, the payout will be from a shared global pot rather than a pot that has been set aside for a specific contributor. This increases greater uncertainty of funding from Olas as central funding is somewhat outside of each project's control. The number of other projects, their scores and their cost base are significant factors that determine a project's payout. However, since contributors get access to the funds in advance, in contrast to the other markets, the risk is not borne by them. It is borne by their funders. The reward for this risk, as stated above, is the possibility of making a profit on investment. This is a much more suitable system for this sector given the relative costs and possible rewards.

Here is the chronology of the fund raising process:

* The process begins with an investigative journalist or scientist (or groups of either) making a proposal for research.&#x20;
* They will state a budget and what percentage of the profit they are willing to share for a raise that covers the budget. They will also state a timeline for the research and project milestones. A deadline for the raise must be set so that funders who commit funding can receive it back within a certain timeframe rather than it being indefinitely committed to a project that isn't reaching its target. However, if funders agree, they can roll their funds over to a new raise on deadline day.&#x20;
* If the target is met, a tranche of funds will be released to start the project. Researchers will constantly have to update funders on their work and funders will vote by simple majority to release more funds when requested by the researchers.&#x20;

<div data-full-width="true">

<figure><img src="../../../.gitbook/assets/Backup - All the diagrams (4) (1).png" alt=""><figcaption><p>Figure 1. Investment &#x26; Funding Market Overview</p></figcaption></figure>

</div>

* Once the research is completed, it'll be given a score and a costs award by a [review market](../../quality-control-markets/academic-research-markets/review-markets.md). This costs award may be lower than the declared budget.&#x20;
* At the end of that quarter, the project will receive funding from the Investigative Journalism Funding Pool or the Scientific Research Funding Pool based on its score, its costs award and also the respective scores and awards of everyone else competing for the quarterly payout.&#x20;

<div data-full-width="true">

<figure><img src="../../../.gitbook/assets/Backup - All the diagrams (2).png" alt=""><figcaption><p>Figure 2. Quarterly Funding Pool Payout Mechanism</p></figcaption></figure>

</div>

### Quarterly Funding Pool Payout&#x20;

The quarterly funding allocation to contributors is determined by a formula designed to assess each project's merit and financial needs within the competitive landscape of the funding pool. This approach ensures that the distribution of funds is both fair and aligned with the objectives of the funding body. Key to this process is the evaluation of each project's score and cost award, alongside the application of a **Penalty Factor for Budget Discrepancy (PBD)** to discourage unrealistic budget declarations. PBD  is applied to reduce the funding amount received by a project if its declared budget significantly exceeds its cost award. This penalty helps ensure that projects are incentivised to only declare realistic budgets and that the allocation of funds is done more equitably.

**Key variables explained:**

1. $$Si​$$ = Score of project $$i$$.
   * Represents the project's quality or merit as determined by a review process. It reflects the project's potential impact and alignment with the funding body's goals
2. $$Ci​$$ = Costs award for project $$i$$.
   * Signifies the financial valuation of the project's necessary expenses as adjudicated by a review market. It aims to cover the realistic costs needed to bring the project to fruition.
3. $$Bi​$$ = Declared budget for project $$i$$.&#x20;
   * The budget initially proposed by the project, indicating its anticipated financial requirements. This figure is critical for evaluating financial planning and realism in budget declarations.
4. $$Ftotal​$$ = Total funding available.
   * The aggregate amount of funds set aside for distribution within either the Investigative Journalism Funding Pool or the Scientific Research Funding Pool for the quarter.
5. $$Fi​$$ = Funding received by project $$i$$.
   * The actual amount of funding awarded to the project, calculated based on the payout formula. It is a function of the project's evaluated merit, financial assessment, and adherence to budget realism.
6. $$PBD$$ = Penalty Factor for Budget Discrepancy.
   * A corrective measure applied to adjust the funding for projects whose declared budgets substantially exceed their awarded costs. This factor reduces the funding amount for a project if its declared budget significantly exceeds its cost award.&#x20;
   * PBD is calculated based on the declared budget $$Bi​$$, the cost award $$Ci​$$, a predefined Threshold, and a Penalty Rate. &#x20;
7. Threshold
   * Represents a predefined percentage that sets the acceptable limit for the discrepancy between a project's declared budget and its cost award without incurring a penalty.&#x20;
   * The Threshold is established to allow a certain degree of flexibility in budget declarations. It acknowledges that some variance between the declared budget and the cost award is normal and acceptable, reflecting uncertainties in project planning and assessment.
   * When the percentage difference between the declared budget and the cost award exceeds the Threshold, the penalty mechanism is triggered.&#x20;
8. Penalty Rate
   * Determines the severity of the reduction applied to the funding amount for discrepancies that exceed the Threshold. It quantifies how much the funding is decreased as the discrepancy between the declared budget and the cost award grows.
   * The Penalty Rate is designed to scale the penalty applied to projects based on the extent of their budget overestimation. It serves as a deterrent against significantly overstating project budgets.
   * The Penalty Rate is applied to the portion of the discrepancy that exceeds the Threshold. For each percentage point by which the discrepancy surpasses the Threshold, the Penalty Rate multiplies the effect on the funding reduction.

The following payout formulas calculate the funding for project $$i$$ based on a weighted sum of its relative score and costs award, adjusted for the penalty associated with significant discrepancies between the declared budget and the cost award, and then scaled by either the total funding available or the sum of the costs awards. This approach aims to distribute funding more fairly and encourage more accurate budget declarations. This ensures that projects are funded in proportion to their evaluated merit and financial needs, compared to the collective needs and merits of all projects competing for funds.

#### Funding Pool Payout Formula - Scenario 1&#x20;

If the total funding available for a given funding round is **less or equal to** the total sum of costs awarded to all participating projects (Total Funding ≤ Total Sum of Costs Awarded), the funding pool payout formula can be outlined as follows:

$$PBD = \max\left(0, \frac{B_i - C_i}{B_i} - \text{Threshold}\right) \times \text{Penalty Rate}$$

$$F_i = \left( \frac{S_i}{\sum_{j} S_j} \times W_S + \frac{C_i}{\sum_{j} C_j} \times W_C \right) \times (1 - PBD) \times F_{\text{total}}$$

#### Funding Pool Payout Formula - Scenario 2

If the total funding available is **greater** than the total sum of costs awarded to participating projects (Total Funding > Total Sum of Costs Awarded), the funding pool payout formula can be outlined as follows:

$$PBD = \max\left(0, \frac{B_i - C_i}{B_i} - \text{Threshold}\right) \times \text{Penalty Rate}$$

$$F_i = \left( \frac{S_i}{\sum_{j} S_j} \times W_S + \frac{C_i}{\sum_{j} C_j} \times W_C \right) \times (1 - PBD) \times {\sum_{j} C_j}$$

Where:

* $$∑j​Sj​$$ and $$∑j​Cj​$$ represent the sum of scores and the  total sum of costs awards (total amount owed to projects) for all competing projects $$j$$, respectively.
* $$Ws$$ and $$Wc​$$ are weights assigned to the score and costs award components, indicating their importance in determining the funding allocation. These weights must sum to 1  ($$Ws+Wc=1$$)  to ensure the formula fairly distributes the total available funding in the pool for a given quarter.

The funding each project receives is determined by a weighted sum of two main components, the PBD value, and the total funding available:

1. **Relative Score Contribution**: Calculates the project's score as a proportion of the total scores for all competing projects, multiplied by a weight reflecting the score's significance in the funding decision.
2. **Relative Cost Award Contribution**: Determines the project's cost award as a percentage of the total cost awards for all projects, multiplied by a weight that signifies the cost award's importance in the allocation process.
3. **Budget Discrepancy Adjustment (**_**PBD**_**)**: Applies a penalty for projects with declared budgets that significantly exceed their cost awards, encouraging more accurate financial forecasting. This is a function of the ratio between the declared budget and the cost award.
4. **Total Funding Available (**_**Ftotal) :**_Should the available funding not surpass the total awarded costs of all participating projects, allocation will occur on a pro-rata basis, factoring in each project's score and costs award, alongside penalties for budgetary discrepancies. Conversely, if the total available funding exceeds the combined costs awarded, each project will be funded based on its proportion of the total cost awards, whilst taking into account the project's relative score as well as penalties deducted for any discrepancies in budget projections above the acceptable threshold. Any remaining funds post-allocation are rolled over to the next funding cycle's pool.

### Case Study Example One: Project Alpha's Funding Pool Payout

**Project Alpha** is a groundbreaking initiative aiming to revolutionise renewable energy storage solutions. The project team has applied for funding from the Scientific Research Funding Pool, hoping to secure financial support for their research and development activities.

**Key Data:**

* **Score of Project Alpha**: 85 (out of a possible 100)
* **Costs Award for Project Alpha**: €200,000
* **Declared Budget for Project Alpha**: €250,000
* **Total Funding Available in the Pool**: €2,000,000
* **Threshold for Budget Discrepancy**: 10% (acceptable variance between declared budget and cost award)
* **Penalty Rate**: 5% (penalty applied per percentage point beyond the Threshold)

**Competing Projects:**

For simplicity, let's assume the total scores and costs awards for all competing projects, including Project Alpha, sum up as follows:

* **Sum of Scores of All Projects**: 1000
* **Sum of Costs Awards for All Projects**: €1,500,000
  * Sum of Costs Awards For All Projects **<** Total Funding Available In The Pool

**Calculating Project Alpha's Funding:**

1.  **Relative Score Contribution**:

    $$\text{Relative Score Contribution of Project Alpha} = \frac{85}{1000}$$
2.  **Relative Cost Award Contribution**:

    $$\text{Relative Cost Award Contribution of Project Alpha} = \frac{200,000}{1,500,000}$$
3. **Budget Discrepancy Adjustment (PBD)**:
   * Discrepancy between declared budget and cost award for Project Alpha: $$€250,000 -  €200,000/€250,000=0.2$$ or 20%
   * Since the discrepancy (20%) exceeds the Threshold (10%), the penalty is triggered on the 10% excess.
   * Excess Over Threshold: $$10$$%
   *   Given the Penalty Rate is 5%, and the excess discrepancy is 10%, PBD is calculated as follows:

       $$\text{PBD for Project Alpha} = 0.10 \times 0.05 = 0.005$$
4. **Final Calculation**:

Incorporating the proportional distribution based on available funds, each project's score and cost contributions, and adjustments for budget discrepancies:

$$F_{\text{Alpha}} = \left( \left( \frac{85}{1000} \times W_S + \frac{200,000}{1,500,000} \times W_C \right) \times (1 - \text{PBD}) \right) \times 1,500,000$$

Assuming equal weightings ($$WS​=WC​=0.5$$) and incorporating the PBD calculation:

$$F_{\text{Alpha}} = \left( \left( \frac{85}{1000} \times 0.5 + \frac{200,000}{1,500,000} \times 0.5 \right) \times (1 - 0.005) \right) \times 1,500,000$$

$$F_{\text{Alpha}} = \left( (0.085 \times 0.5 + 0.1333 \times 0.5) \times 0.995 \right) \times 1,500,000$$

$$F_{\text{Alpha}} = (0.0425 + 0.0667) \times 0.995 \times 1,500,000$$

$$F_{\text{Alpha}} = 0.1092 \times 0.995 \times 1,500,000$$

$$F_{\text{Alpha}} = 162,931.25$$

In Summary:

$$F_{\text{Alpha}} = (( \frac{85}{1000} \times 0.5 + \frac{200,000}{1,500,000} \times 0.5) \times (1 - 0.005)) \times 1,500,000$$

Given the available funding exceeds the sum of cost awards, the formula ensures Project Alpha receives funding proportional to its needs and merit, totalling approximately €162,931.25. This careful calculation exemplifies the funding formula's role in ensuring equitable resource allocation across projects, promoting accurate budgeting, and managing excess funds responsibly by rolling them into the next funding cycle. Project Alpha, despite a budget overestimation, receives substantial support due to its high merit and significant financial need, slightly adjusted for the budget-cost variance beyond the accepted threshold.

### Case Study Example Two: Project Beta's Funding Pool Payout

**Project Beta** is an innovative project aimed at developing advanced AI algorithms for predictive analytics in healthcare. The project team has sought funding from the Scientific Research Funding Pool to help advance their research and prototype development.

**Key Data:**

* **Score of Project Beta**: 90 (out of a possible 100)
* **Costs Award for Project Beta**: €300,000
* **Declared Budget for Project Beta**: €350,000
* **Total Funding Available in the Pool**: €1,200,000
* **Threshold for Budget Discrepancy**: 10% (acceptable variance between declared budget and cost award)
* **Penalty Rate**: 5% (penalty applied per percentage point beyond the Threshold)

**Competing Projects:**

For this case study, let's assume the total scores and costs awards for all competing projects, including Project Beta, sum up as follows:

* **Sum of Scores of All Projects**: 1500
* **Sum of Costs Awards for All Projects**: €2,000,000 (Sum of Costs Awards exceeds the total funding available in the pool)

**Calculating Project Beta's Funding:**

1.  **Relative Score Contribution**:

    $$\text{Project Beta's score proportion} = \frac{90}{1500}$$
2.  **Relative Cost Award Contribution**:

    $$\text{Project Beta's cost award proportion} = \frac{300,000}{2,000,000}$$
3.  **Budget Discrepancy Adjustment (PBD)**:

    * Discrepancy between declared budget and cost award for Project Beta is 14% (since €350,000 is 14% more than €300,000), exceeding the threshold by 4%.

    $$\text{PBD} = 0.04 \times 0.05 = 0.002$$
4. **Final Calculation**: Given the total funding available is less than the sum of costs awards, the funding for Project Beta needs to be calculated based on the proportional distribution of available funds, taking into account its score, cost award, and the penalty for budget discrepancy.

$$F_{\text{Beta}} = \left( \left( \frac{90}{1500} \times W_S + \frac{300,000}{2,000,000} \times W_C \right) \times (1 - \text{PBD}) \right) \times \text{Total Funding Available}$$

Assuming equal weightings for simplicity ($$WS​=WC​=0.5$$):

$$F_{\text{Beta}} = \left( \left( \frac{90}{1500} \times 0.5 + \frac{300,000}{2,000,000} \times 0.5 \right) \times (1 - 0.002) \right) \times 1,200,000$$

$$F_{\text{Beta}} = \left( \left( 0.03 + 0.075 \right) \times 0.998 \right) \times 1,200,000$$

$$F_{\text{Beta}} = 0.105 \times 0.998 \times 1,200,000$$

$$F_{\text{Beta}} \approx \text{€125,736}$$

In Summary:

$$F_{\text{Beta}} = \left( \left( \frac{90}{1500} \times 0.5 + \frac{300,000}{2,000,000} \times 0.5 \right) \times (1 - 0.002) \right) \times 1,200,000$$

Project Beta's final funding, after considering its relative merit, financial need, and slight adjustment for the budget-cost variance beyond the accepted threshold, is approximately €125,736. This example demonstrates how the funding formula operates to allocate resources in a scenario where the sum of cost awards exceeds the total funding available, ensuring a fair distribution among competing projects while encouraging realistic budgeting practices.
