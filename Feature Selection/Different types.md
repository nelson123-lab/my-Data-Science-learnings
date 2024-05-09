# Different types of Feature selection methods

Sure, here's the information organized into a table format:

| Method           | Description                                                                                      | Advantages                                  | Disadvantages                                           |
|------------------|--------------------------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------------------------|
| Filter methods   | Utilize simple statistical tests like Anova or chi-square test. Independent of ML algorithm.    | - Quick feature removal                    | - Does not capture redundancy                           |
|                  | Discriminate features based only on the feature characteristics.                                | - Model agnostic                           | - Does not capture feature interaction                  |
|                  |                                                                                                  | - Fast computation                         | - Poor model performance                                |
| Wrapper methods  | Take into consideration ML algorithms. Evaluate groups of features.                             | - Considers feature interaction            | - Not model agnostic (features optimized for one model may not be best for others) |
|                  |                                                                                                  | - Best performance                         | - Computationally expensive (ML model for each feature combination) |
|                  |                                                                                                  | - Best feature subset for a given algorithm | - Often impracticable with large datasets               |
| Embedded methods | Feature selection during training of ML algorithms.                                               | - Good model performance                  | - Not model agnostic                                    |
|                  |                                                                                                  | - Capture feature interaction             |                                                         |
|                  |                                                                                                  | - Faster than wrapper methods             |                                                         |
|                  |                                                                                                  | - Better than filter methods               |                                                         |
