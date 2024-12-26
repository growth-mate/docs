# Ad Campaign Selection System
This document outlines how our ad serving system selects which campaigns to show. The system aims to balance multiple factors to ensure optimal campaign performance while maintaining fairness in the auction process.

## Campaign Selection Factors
Our system considers multiple aspects when choosing which ad to serve:
1. **Campaign Performance**  
We evaluate how well each campaign matches the current context, including factors like relevance and predicted performance.

2. **Bidding System**  
We use a modified [perturbed](https://www.perplexity.ai/search/what-is-a-perturbed-auction-OfXn2l9UQ8mea_1B_vhbtw#01)-[second-price](https://en.wikipedia.org/wiki/Generalized_second-price_auction) auction system that:
- Ensures advertisers never pay more than their maximum bid
- Encourages honest bidding: Second-price auctions incentivize participant to bid their true value, as well as reduce [winner's curse](https://en.wikipedia.org/wiki/Winner%27s_curse). Perturbations prevent some price manipulations, such as "spiteful-bidding". 
- Maintains a minimum floor price to ensure alignment with publishers.

3. **Campaign Progress**  
The system monitors campaign progress to ensure delivery goals are met, considering:
- Remaining budget
- Campaign timeline
- Targeting goals

4. **Fair Distribution**  
To maintain a healthy advertising ecosystem, our system includes mechanisms to:
- Prevent any single campaign from dominating the available inventory
- Ensure fair competition between different types of campaigns
- Balance delivery across all active campaigns

## Best Practices for Advertisers

1. **Set Realistic Bids**
    - Bid your true value
    - Our auction system reduces your chance to overpay
    - Consider using different bids for different audience segments based on their value to your campaign


2. **Campaign Setup**
    - Clearly define your target audience
    - Set appropriate campaign durations based on your budget and goals.
    
    ```admonish tip

    We recommend to:
    - Create your campaign at least 24 hours before your expected start date
    - Minimum campaign duration of 1 week
    ```

    - Use relevant targeting criteria that align with your objectives


3. **Optimization Tips**
    - Focus on improving ad relevance and quality rather than trying to game the system
    - Monitor performance metrics to understand what works best for your audience


## Campaign Types
Our system supports different campaign optimization goals:
- **Conversion:** For advertisers focusing on reaching only some specific and well-defined audience.
- **Reach:** For advertisers aiming to reach the broadest relevant audience.

Each type has its own bidding considerations and best practices that our system automatically accounts for.

```admonish tip
Our system excels at discovering untapped audiences for Reach campaigns, often finding valuable users at competitive prices. For advertisers looking to expand their audience efficiently, Reach campaigns can be particularly cost-effective.
```