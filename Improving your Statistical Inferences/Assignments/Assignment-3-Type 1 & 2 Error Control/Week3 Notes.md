# Notes from Week 3

## Type 1 Error Rate Control

- Type 1 Error : Saying that there is something, when there is nothing
- Typical Type 1 Error Rate α = 0.05 - in the long run, you are expected to commit a Type 1 error 5% of the time.
- In Physics, the Type 1 error rate is set to 5 sigma level - 0.0000003
- Type 1 Error Rate Inflation : multiple tests
    - Example: In a 2x2x2 ANOVA, there are 7 tests (three main effects, three 2-way interactions, one 3-way interaction.)

    - In this case the Type 1 error rate is 1 - (0.95 ^ 7) = 30%

-  [Bonferroni Correction](https://en.wikipedia.org/wiki/Bonferroni_correction) ideated by Prof. Dunn.
    - So how Bonferroni correction works is simply divide the overall α by the number of tests.
    - Or  p-value * number of tests

- Familywise error rate : Set the α to the number of tests you are interested in , not all the tests that are possible in your experiment.

- [Holm Correction](https://en.wikipedia.org/wiki/Holm%E2%80%93Bonferroni_method) : A bit flexible than the Bonferroni Correction.

- Optional Stopping - look at your data and collect more data if a test is not significant
    - Collecting data until p < 0.05 inflates the Type 1 error
    - If not used correctly, a user can always obtain a significant result
    - Use Sequential Analysis which controls Type 1 error
        - Pocock Boundary - divide the α-level by the number of analyses

- Recent approaches control the false discovery rate, not the family-wise error-rate - See [Benjamin and Hochberg](http://www.stat.purdue.edu/~doerge/BIOINFORM.D/FALL06/Benjamini%20and%20Y%20FDR.pdf)

## Type 2 Error Rate Control

- Type 2 Error : Saying there is nothing, when there is something
- Take a look at Power Graphs (Sample Size vs Power) when you design the studies
- Type 2 error rate is 1 - Power
- Studies with high power (low Type 2 error) are 'severe' tests. They are very good test of your hypothesis.
- Design for studies with high power.
- Increase power by :
    - Decreasing measurement error
    - Using within designs (when within-measure correlation > 0.5)
    - Increasing variability (e.g., use 7 or 9 instead of 3 or 5 item scales)
    - Use one-sided tests (if you have a directional prediction)
    - Increase Sample Size (very difficult and in many cases expensive)

- As long as replications are performed, Type 1 errors will be corrected. Type 2 errors might be more severe.
