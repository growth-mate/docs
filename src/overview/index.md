![Banner](banner.png)

# Overview

Welcome to our GrowthMate docs!

## What is GrowthMate?

GrowthMate is a recommendation platform ...
We run a general purpose [Ranking API](../services/ranking/index.md) that powers our [Advertisements](../services/ads/index.md), and personalized [Discovery Feeds](../services/discovery-feed/).

## How does it work?

When a user logs into a webpage that integrates one of our services, an API request with the users wallet address goes out to our server. We fetch the public users transaction history from the chain and enrich it with additional data. Our propriatary AI model predicts certain aspects of the users next action with 80% accuracy. These include

- Project name
- Time until execution
- Amount of USD involved

Based on this prediction we serve our recommendations. ...

![Flowchart](flowchart.png)

## What data do we use?

We exclusively rely on data that is publicly accessible (transaction history, ip address, ...) and do not employ any client side tracking.