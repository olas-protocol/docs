---
description: Overview of the Olas Identity Layer.
---

# Identity Layer

The Identity Layer is a fundamental aspect of Olas, dedicated to ensuring unique identification, verification, and role assignment for each user within the ecosystem. This layer underscores the importance of **user authenticity, role-based access control,** and the **option for pseudonymity**.

<figure><img src="../.gitbook/assets/Olas Identity Layer (1).png" alt=""><figcaption><p>Figure : Olas Identity Layer Architecture</p></figcaption></figure>

While Olas is open for reading by anyone, active participation and access to certain functionalities require users to demonstrate their _uniqueness and humanness_. To safeguard against [Sybil attacks](https://en.wikipedia.org/wiki/Sybil\_attack) and ensure a trustworthy platform, Olas employs mechanisms such as Proof Of Unique Human (PoUH) or [Proof Of Personhood (PoP)](https://en.wikipedia.org/wiki/Proof\_of\_personhood). These protocols verify the distinct identity and humanness of users, thus fostering secure and authentic community engagement within the Olas ecosystem.

### Users that must be Verified

Certain roles require a unique humanity verification to maintain the integrity of the system:

[**Content Contributor**:](../participants/content-contributor.md) Verified users who produce content for the platform undergo a thorough verification process before they can begin contributing.

[**Active donor**:](../participants/donor.md#donor-classification) Users who can donate to content contributors via Olas funding rounds. Their donations may be magnified via the Quadratic Funding mechanisms, which allocate funds based on both the amount of funding and the number of donors.&#x20;

[**Fact-checker**:](../participants/fact-checker.md) Responsible for identifying inaccuracies in contents, rewarded based on their findings. They undergo a unique human verification process before completing registration.

[**Judge**:](../participants/judge.md) Evaluates the inaccuracies raised by fact checkers and determines the validity of the issues submitted. Judges are rewarded based on their participation in the judging panel. Fact-checkers with high reputation scores may participate in judging panels as **Super Forecasters**, along with **randomly** selected **content contributors (Judges)**.&#x20;

### Olas User Registry

Post-verification, users (Journalists, Donors, Fact Checkers) are enlisted in the "Olas User Registry". This registry maintains a list of all the verified users, their roles, and associated details, ensuring a structured management of user profiles while adhering to privacy standards.

### Pseudonymity & Privacy

Olas upholds users' privacy rights, offering an option for pseudonymity, thus encouraging open expression without fear for their safety. Users will always have the choice to maintain their pseudonymity on the platform.&#x20;
