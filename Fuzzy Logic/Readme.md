## Fuzzy logic
Fuzzy logic is the process of converting the results from a binary output to a range of values between the absolute false and absolute true.

- The set of rules we define is based upon experiences. For example we are making a loan approval system based on the credit score. We need to have a set rules to determine the credit score vs the risk of loan approval.
- If we are deciding Good credit score as 750 and above, 650- 750 as Neutral and below 650 as bad. These values will be different for different banks as their criteria. We actually need some functions that can take a set of values than the crisp values for determing
  whether a person is having good, neutral and bad credit score. These functions are called **membership function** in fuzzy logic.

<div align="center"><img src="https://github.com/nelson123-lab/my-Data-Science-learnings/blob/1d89495ff6e0c5a2a02e9da679158731a9ad6bb0/Fuzzy%20Logic/Fuzzy%20Inference%20system.png" width="900"/></div>

- The above image shows the steps in the fuzzifization and the process involved.
<div align="center"><img src="https://github.com/nelson123-lab/my-Data-Science-learnings/blob/1d89495ff6e0c5a2a02e9da679158731a9ad6bb0/Fuzzy%20Logic/Fuzzification.png" width="900"/></div>

- Applying membership function on the crisp output converts it into fuzzy variables. This process is known as fuzzification.

<div align="center"><img src="https://github.com/nelson123-lab/my-Data-Science-learnings/blob/1d89495ff6e0c5a2a02e9da679158731a9ad6bb0/Fuzzy%20Logic/Fuzzy%20logic%20rules.png" width="900"/></div>

- We apply fuzzy rules on the fuzzy variables to determine the range of the output.
<div align="center"><img src="https://github.com/nelson123-lab/my-Data-Science-learnings/blob/1d89495ff6e0c5a2a02e9da679158731a9ad6bb0/Fuzzy%20Logic/Defuzzification.png" width="900"/></div>

- Now from the range of the values we need get the crisp output. Applying defuzzification, we get the crisp output. Here, Centroid of the common area is used to
  determine the crisp output.

References:

- [What Is Fuzzy Logic? | Fuzzy Logic, Part 1](https://youtu.be/__0nZuG4sTw)
