# Lecture notes W4D1

## Feature selection technique 
 - Filter methods:
 
    - Measure relavance of feature by correlation with dependent variable
    - if feature is correlated within target, keep. Otherwise discard
    - Advantages: Fast, no training involved
    - Disadvantages: Ignores feature combinations and keeps redundant features.

 - Wrapper methods:

    - Train ML model with different subsets of feature
    - if feature improves perforamnce, keep. Otherwise discard
    - Applied during traing ML model
    - Most popular wrapper method: Recursive Feature Elimination
