# Reputation System Architecture

## Olas Reputation System Overview

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/Olas Reputation System.png" alt=""><figcaption><p>Figure 11. Olas Reputation System</p></figcaption></figure>

</div>

## Roles Within The Olas Reputation System

### Content Contributors

* Content Contributors are individuals who publish articles on their given areas of expertise within Olas Information Markets.
* **Reputation Score (RS) Impact:**
  * RS is crucial for acquiring external investment, receiving tips, and securing matching pool funds. Consequently, RS significantly impacts a Content Contributor's earning potential.
  * RS also affects how the funds raised are distributed between the Content Contributor and the Olas protocol, with both RS and final article score determining the total payout to the contributor.

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/Contributor Reputation.png" alt=""><figcaption><p>Figure 12. Contributor Reputation Process</p></figcaption></figure>

</div>

### **Judges**

* Judges are domain experts who participate in **Fact Reporting Markets**. Judges organize, review, and vote on **issues raised** by Fact Checkers regarding articles in their expertise area(s).
* **Reputation Score (RS) Impact:**
  * RS directly impacts a judge's earning potential as it determines whether a judge gains access to more exclusive and higher-paying judging panels.
  * Moreover, if a judge's RS falls below the acceptable RS threshold for judging panel participation, they are suspended from participating in judging panels and must regain access to judging by increasing their RS through other means such as submitting valid inaccuracies as a fact checker.

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/Judge Reputation 2.png" alt=""><figcaption><p>Figure 13. Judge Reputation Process</p></figcaption></figure>

</div>

### **Fact-Checkers**

* Fact-checkers are users who **identify inaccuracies** in content published within **Fact Reporting Markets** and submit them for review by the judging panel.
* They are rewarded for submitting valid inaccuracies and their reward scales in relation to the uniqueness and severity of the inaccuracies found.
* **Reputation Score (RS) Impact:**
  * RS determines a fact checker's earning potential via reward distribution and access to judging panel opportunities. The higher the fact checker's RS, the higher the rewards they are paid for submitting valid inaccuracies. Also, once a fact checker's RS score surpasses a set threshold, they become eligible to participate in judging panel opportunities.
  * Conversely, if their reputation score suffers a significant weekly drop, they will be frozen out of fact checking markets for a period.&#x20;

{% hint style="info" %}
Fact-checkers who submit a high volume of invalid issues over a short period (i.e. over a 1-2 week period) are banned from submitting issues for 1-3 weeks depending on the volume of inaccurate issues they have submitted during that period.
{% endhint %}

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/Fact Checker Reputation 2.png" alt=""><figcaption><p>Figure 14. Fact Checker Reputation Process</p></figcaption></figure>

</div>

## **Olas Reputation Engine**

* **Functionality:** Utilizes data derived from a user's interactions with the Olas protocol to compute a reputation score based on their selected role(s) within a given information market on the protocol.
* **Data Processing:**
  * Ingests user data and applies role-specific reputation algorithms to calculate RS for all roles assumed by the user in each of the information markets.
  * the reputation engine leverages Decentralized Identifiers (DIDs) to establish the association between a user and their RS.
  * Consequently, Olas requires users to have a unique DID for signing and encrypting data, ensuring data authenticity and security.
* **Reputation Score Updating:** When an RS update is triggered for a user, a request is sent with the relevant data to the reputation engine. The reputation engine applies a role-based reputation algorithm which is used to compute an updated RS based on the user's role(s) within a given information market and their updated data.

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/Olas Reputation System (1).png" alt=""><figcaption><p>Figure 15. Updates for User Reputation</p></figcaption></figure>

</div>
