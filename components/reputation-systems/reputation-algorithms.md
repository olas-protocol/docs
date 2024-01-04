# Reputation Algorithms

## Content Contributor Reputation Model

#### Metrics:

1. **Total Number of Articles Published (N):** The cumulative count of articles a contributor has published in each Olas Information Market.
2. **Sum of all Outcome Scores given to Articles Written (AS):** The total of all outcome scores received for all the articles written by the contributor across all Information Markets.

#### Reputation Algorithm:

The **Reputation Score (RS)** for a Content Contributor is calculated using the following formula:

$$\boxed{ RS \,  = \, \,\dfrac{  AS }{ N } }$$

## **Fact-Checker Reputation Model**

#### **Metrics**:

1. **Total Number of Valid Issues Raised (V):** Cumulative count of valid issues identified by a fact-checker.
2. **Number of Valid Issues Submitted in Each Category of Severity (S):** Number of valid issues submitted, categorized by severity.
   * **Low Severity (LS):** Minor Issues that have less impact or are easily rectifiable.
     * **Multiplier Factor (M1):** 1.2
   * **Medium Severity (MS):** Issues that have a moderate impact or may require a moderate effort to rectify.
     * **Multiplier Factor (M2):** 1.5
   * **High Severity (HS):** Significant Issues that have a high impact or may require substantial effort to rectify.
     * **Multiplier Factor (M3):** 2
3. **Number of Unique & Valid Issues Submitted (UV):** Number of issues submitted that are both unique & valid.&#x20;
   * **Unique & Valid (UV):** Uniqueness is defined as an issue that was identified and submitted by only one Fact-Checker.
     * **Multiplier Factor (M4):** 2

#### **Reputation Algorithm**:&#x20;

The Reputation Score (RS) for a Fact-Checker is derived using a weighted sum formula. Each metric is multiplied by a corresponding weight, and the sum of these products forms the RS. The formula is articulated as follows:

$$\boxed{ Preliminary \, Score \,  = \, V \, + \, ( \,LS \, \times \, M1 \,) \, + \, ( \, MS \, \times \, M2 \, ) \, + \, ( \, HS \, \times \, M3 \, ) \,+ \, ( \, UV \, \times \, M4 \, ) }$$

$$\boxed{ Reputation \, Score \,  = \, \,\dfrac{  Preliminary \, Score }{ Total \, Number \, Of \, Issues \, Submitted } }$$

_**where:**_

* $$M1​, M2​, M3​,$$ and $$M4$$ are the weighting factors assigned to each metric based on its relative importance.

## **Judge Reputation Model**

#### **Metrics**:

1. **Total Number of Judging Panels Completed (JP):** The cumulative count of judging panels a judge has completed.
2. **Sum of all Voting Accuracy Scores Across All Votes Submitted in Judging Panels (VA):** The total of accuracy scores received for all votes submitted by the judge across various judging panels.

#### **Reputation Algorithm**:&#x20;

The **Reputation Score (RS)** for a Judge is computed using the following formula:

$$\boxed{ RS \,  = \, \,\dfrac{  VA }{ JP } }$$
