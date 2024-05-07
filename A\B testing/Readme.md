## A/B Testing
- A/B Testing is necessary when a trained machine learning model is deployed online to the users. Even though the models that performed well
in the pre-deployment (offline deployment) might not provide expected results in post-deployment (Online deployment).
- This is similar to testing models on Real-world data after testing on Test data.

The concept of A/B testing relates closely to the statement "Making decisions is easy — what’s hard is making the right decisions." This connection can be understood in several ways:

1. **Data-Driven Decision Making**: A/B testing provides empirical data that helps in making informed decisions. While it's easy to make a choice based on intuition or subjective opinion, A/B testing facilitates the process of making the right decision by backing it up with concrete evidence.

2. **Reducing Subjectivity**: In the absence of data, decisions are often made based on personal biases, assumptions, or incomplete information. A/B testing helps to minimize this subjectivity by presenting clear comparisons between different options.

3. **Validating Assumptions**: A/B testing is particularly effective in challenging and validating assumptions. A decision might seem right based on a prevailing belief or trend, but A/B testing can reveal whether those assumptions hold true in practice.

4. **Risk Mitigation**: The 'right' decision is often the one that balances benefits with risks. A/B testing allows organizations to test changes on a smaller scale before fully implementing them, thereby reducing the risk associated with making the wrong decision.

5. **Continuous Learning and Improvement**: The process of A/B testing encourages continuous learning. By consistently testing and learning from the outcomes, organizations can make increasingly better decisions over time.

6. **User-Centric Decisions**: Especially in user experience and marketing, the 'right' decision is often the one that aligns best with user preferences and needs. A/B testing ensures that decisions are made with a clear understanding of user responses.

7. **Objective Analysis Over Gut Feeling**: While making a decision is straightforward, ensuring it is the correct one involves careful analysis and consideration of facts. A/B testing replaces gut feeling and speculation with objective analysis.

In summary, A/B testing embodies the principle that while decision-making might be straightforward, ensuring the decisions are correct is more complex. It provides a structured, data-driven approach to discerning the most effective choice among alternatives, aligning perfectly with the ethos of making the 'right' decisions.

## When not to use A/B Test

1) Lack of proper infrastructure - Having a data engineering infrastructure is reliable ( Smaller companies won't have the dedicated infrastructure to conduct complex A/B Tests).
2) Lack of Impact - Is the benefit or the profit it's gonna get way more than the time and resources to conduct the test?
3) Lack of traffic - We won't be able to conduct an A/B Test without having enough users using a feature.
4) Lack of Conviction - Different variations of the same feature might be required in the testing process when we are doing A/B testing for a high-traffic and high-value feature. ( Add to cart, Buy now buttons in most of the top e-commerce platforms.)
5) Lack of isolation - An isolation is required for a test to work properly.
