# Different types of Feature selection methods

## 1) Filter methods
- Include simple statistical tests like Anova or chi-square test.
- Independent of the ML algorithm.
- Discriminate features based only on the feature characteristics.

### Advantages 
- Quick feature removal
- Model agnostic
- Fast computation

### Disadvantages
- Does not capture redundancy
- Does not capture Feature interaction
- Poor model performance.

## 2) Wrapper methods
- Takes into consideration of ML algorithms.
- Evaluate group of features.

### Advantages 
- Considers feature Interaction.
- Best performance
- Best feature subset for a given algorithm.

### Disadvantages
- Not model agnostic ( The features for one model will not be best for different ML models)
- Computationally expensive ( ML model for each feature combinations )
- Often impracticable when the data is large.

## 3) Embedded methods
- Feature selection during training of ML algorithm

### Advantages 
- Good model performance
- Capture feature interaction
- Better than filter methods
- Faster than wrapper methods

### Disadvantages
- Not model agnostic
