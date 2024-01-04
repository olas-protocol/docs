---
description: Overview of Olas Citation Systems
---

# Citation Systems

Olas employs a robust editorial management system that utilizes **attestation IDs** to manage article references, enabling the fair and transparent distribution of retroactive royalty payouts.

Content contributors who wish to submit their work to Olas must first sign an attestation transaction using the wallet keys associated with their unique decentralized identifier (DID). This process serves two critical functions:

* **Authenticity Verification:** Verify the originality of the submitted content, ensuring that all works published on Olas are genuine and traceable to their source.
* **Reference Attestation:** Recognizes the use of references, creating an intellectual contribution chain.

This transaction creates a unique Attestation ID which is irrevocably tied to the article. This ID is essential for the subsequent tracking and validation of citations used across the platform as well as facilitating retroactive royalty fee payments to the author.

### Royalty Earnings Via Citations

When an article Attestation ID is cited, the originating author receives a predetermined royalty fee, promoting the generation and use of credible content. In other words, every time an attestation ID is referenced by other content contributors, the original author automatically earns a set royalty fee.

### Citation Engine

Following the closure of an information market, the citation engine is updated with the market results, including content scores and Attestation IDs, for archival and future reference. The Citation Engine assigns royalties to content contributors depending on various factors.

<figure><img src="../../.gitbook/assets/Olas Citation System.png" alt=""><figcaption><p>Figure 10. Citation System</p></figcaption></figure>

## Royalty Fee Algorithms

Contributor royalty fees are calculated using a proprietary algorithm developed by Olas. When an article submission includes references, the associated Attestation IDs tied to each reference trigger an automatic royalty fee payment, directly benefiting the original content contributor. Royalty payments are contingent upon a fixed citation price range established by the Olas protocol. Depending on the outcome of a given information market, these royalties are paid out by the beneficiary of the winning side of the market i.e. the content contributor or the Olas matching pool.

### Total Royalty Fee Payout

The total royalty fee that must be paid out by either the contributor or the Olas matching pool (depending on the winning side of the market) can be determined as follows:



$$\boxed {TRF\ =\ NC\ *\ CP}$$



$$TRF = Total\ Royalty\ Fee\ Owed$$

$$NC = Total\ Number\ of\ Citations\ Used$$

$$CP = Citation\ Price\ Per\ Article$$



**Example:**

Bob submits his article to an information market on Olas. Once the market settlement deadline is reached, the 'Yes' side of the market wins. Bob has taken up a position on the Yes side of the market and is, therefore, liable to pay the reference royalty fees from his winnings. Bob's royalty fee payout can be determined using the following information:

$$Citation\ Price\ Per\ Article\ (CP):\ $3.00$$

$$Total\ Number\ of\ Citations\ Used\ (NC):\ 15$$



Using this information we can calculate the '**Total Royalty Fee Owed**' (TRF) as follows:

$$TRF\ =\  $3.00\ * 15$$

$$TRF\ =\  $45.00$$

As we can see from the above calculations, Bob must pay **$45.00** in royalty fees to the authors he cited in his article. This fee is automatically deducted from Bob's payout.

### Earned Royalty Fees

A content contributor's earned royalty fees accrued from each article published on Olas can be calculated using the following formula:



$$\boxed {ERF\ =\ TCA\ *\ CP}$$



$$ERF = Earned\ Royalty\ Fees\ Per\ Article$$

$$TCA = Total\ Number\ of\ Citations\ Per\ Article$$

$$CP = Citation\ Price\ Per\ Article$$



**Example:**

Alice publishes an article on Olas. Her article has become very popular and her article attestation ID has been cited in 35 articles published on Olas. Alice wants to calculate the total amount of royalty payouts she has received from her peers citing this article. Alice's **total earned royalty fees** (ERF) are determined as follows:

$$Citation\ Price\ Per\ Article\ (CP):\ $3.00$$

$$Total\ Number\ of\ Citations\ Per\ Article\ (TCA):\ 35$$



Using this information, we can calculate Alice's **total royalty payout**:

$$ERF\ =\ 35\ *\ $3.00$$

$$ERF\ =\ $105.00$$

Alice's total royalty fee payout from her article is **$105.00**. This fee is automatically paid out to Alice on an ad-hoc basis as authors publish articles that cite Alice's article attestation ID.

