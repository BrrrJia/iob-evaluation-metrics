# IOB-evaluation-metrics

Implement an IOB-based evaluation system for sequence entities. Compare results using Precision, Recall, and F1 metrics in two variants: 

Variant 1: A predicted span counts as a true positive only if it matches the annotation exactly (in example 1 below, we expect exactly one true positive).

Variant 2: A prediction counts as a true positive if at least one token matches.

## Test examples:

Example 1: 

Gold: O B I I B I I O B O 

Prediction: O B I I B I O O O O O 

Example 2: 

Gold: O B I I B I I O B O 

Prediction: B O B B O B B B B O B 

Example 3: 

Gold: O B I I B I I O B O 

Prediction: B I I I I I I I I I I I 

Example 4: 

Gold: B I I I I I I I I I I 

Prediction: B B B B B B B B B B B B

## Packages used:

NLTK, more_itertools
