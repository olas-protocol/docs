---
description: Overview of the Olas Identity Layer.
---

# Identity Layer

The Identity Layer is a fundamental aspect of Olas, dedicated to ensuring unique identification, verification, and role assignment for each user within the ecosystem. This layer underscores the importance of **user authenticity, role-based access control,** and the **option for pseudonymity**.

<figure><img src="../.gitbook/assets/Olas Identity Layer (1).png" alt=""><figcaption><p>Figure 1. Olas Identity Layer Architecture</p></figcaption></figure>

While Olas is open for reading by anyone, active participation and access to certain functionalities require users to demonstrate their _uniqueness and humanness_. To safeguard against [Sybil attacks](https://en.wikipedia.org/wiki/Sybil\_attack) and ensure a trustworthy platform, Olas employs mechanisms such as Proof Of Unique Human (PoUH) or [Proof Of Personhood (PoP)](https://en.wikipedia.org/wiki/Proof\_of\_personhood). These protocols verify the distinct identity and humanness of users, thus fostering secure and authentic community engagement within the Olas ecosystem.

### Roles & Responsibilities

[**Content Contributor**:](../participants/content-contributor.md) Verified users who produce content for the platform. They undergo a thorough verification process before they can begin contributing.

[**Active donor**:](broken-reference) Users who can donate to content contributors via Olas funding rounds. Their donations may be magnified via the Quadratic Funding mechanisms, which allocate funds based on both the amount of funding and the number of donors. Active Donors must undergo a robust verification process.

[**Fact-checker**:](broken-reference) Content Contributors with expertise in identifying inaccuracies in Olas content. They are rewarded based on the validity of their findings as determined by the judging panel. They undergo a unique human verification process before completing the registration process.

**Super Forecaster**: Successful Fact-checkers who have acquired a good reputation score can apply for judging panel duties.

[**Judge**:](broken-reference) Evaluates the inaccuracies raised by fact checkers and determines the validity of the issues submitted. Judges are rewarded based on their participation in the judging panel. Fact-checkers with high reputation scores may participate in judging panels as **Super Forecasters**, along with **randomly** selected **content contributors (Judges)**. No additional registration is required for Fact-checkers to participate.

[**Reader**:](broken-reference) Users who access the platform to consume content.

[**Passive Donor**:](broken-reference) Users or entities that wish to contribute funds to the global pools that are used during Quadratic Funding rounds on Olas. These funds are distributed to the content contributors in accordance with outcomes in the quadratic funding markets populated by active donors.\


### Unique Humanity Verification

Certain roles require a unique humanity verification to maintain Olas' integrity, thwart misuse, and prevent Sybil attacks. Unique humanity verification is mandatory for **Content Contributors, Donors,** and **Fact-checkers**. This ensures that a genuine human creates each unique user profile on Olas. \


### Olas User Registry

Post-verification, users (Journalists, Donors, Fact Checkers) are enlisted in the "Olas User Registry". This registry maintains a list of all the verified users, their roles, and associated details, ensuring a structured management of user profiles while adhering to privacy standards.\


### Judging Panel

The integrity of judging panel is vital to the quality of output on the platform. Content Contributors are selected, based on their expertise and reputation scores, to become Judges. This ensures impartial and informed evaluations of the content published on the platform.



### Pseudonymity & Privacy

Olas upholds users' privacy rights, offering an option for pseudonymity, thus encouraging open expression without fear for their safety. Users will always have the choice to maintain their pseudonymity on the platform.&#x20;
