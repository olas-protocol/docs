---
description: More democratic markets
---

# Quadratic Funding Competitions

Quadratic funding is a radically new funding mechanism that not only seeks to create private markets for public goods to improve outcomes, but seeks to do so in a way that more accurately reflects broader community preferences than vanilla market mechanisms do. It achieves this by establishing a matching pool for donations to competing projects and by using a formula that gives more weight to the number of people that donate than the amount of money donated when matching individual donations with the pooled funds. In this sense it's akin to a middle ground between democracy (one person, one vote) and markets (one dollar, one vote).&#x20;

Here is a diagram explaining the difference between a theoretical centralised vanilla funding competition and an open quadratic funding competition in the Olas protocol:

<figure><img src="../../../.gitbook/assets/Funding Mechanism Comparisons (1).png" alt=""><figcaption><p>Figure 5. Traditional Funding Mechanism vs Quadratic Funding Mechanism</p></figcaption></figure>

Instead of a committee allocating funds to projects in an X-Factor style competition prone to corruption, funds from donors are matched against available funds in a matching pool. The matching pool for each individual competition represents funds allocated to a given topic by the [subsidy allocation mechanism](subsidy-allocation-mechanism.md). Therefore contributors that propose to write on the same topics compete with each other to raise funds from topic pools. Donors will likely pay a lot of attention to how the journalists have previously performed with their written output, bringing market competition to the provision of these public good (free) articles. The expectation is that this will vastly improve journalists' output - especially given that the [information markets](../../../introduction/information-markets-overview.md) are structured to reward quality.   &#x20;

The way quadratic funding is a better representation of the wishes of the broader community than a vanilla market more prone to the influence of the wealthy is via its implementation of a quadratic rule. The formula for calculating each competitor's share in a competition is:&#x20;

`∑i√ci)2`

This formula dictates that the amount received by the project from the matching pool is proportional to the square of the sum of the square roots of contributions received. The consequences of this is that projects that receive money from many donors are favoured for matching pool funds over those that receive money from fewer donors even in many cases if the latter receive more money.&#x20;

Let's understand this with the help of a diagram:

<figure><img src="../../../.gitbook/assets/Competition Between Content Contributors for Funding .png" alt=""><figcaption><p>Figure 6. Competition between Content Contributors For Funding</p></figcaption></figure>

If there is insufficient funds in the matching pool to match the funds to meet the requirements of the quadratic funding formula, each contributor will receive a reduced payout in proportion to the relative claims over the matching pool.&#x20;

### Qualifying Applicants

The quadratic funding competitions, although relatively open, will have limited spaces and are subject to qualifying criteria. The number of spaces available will be dictated by the amount of matching funds allocated to the topic from the global pool. Further contributors that have earned greater than a certain threshold on Olas will be barred from entering quadratic funding competitions. They will be reserved for contributors starting out or in need of the funds because they write on niche topics that garner few tips. This is in line with Olas' third priority of fostering a plurality of voices on the protocol.&#x20;
