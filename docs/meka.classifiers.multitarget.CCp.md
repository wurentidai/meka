## Synopsis
CC method with probabilistic output (CCp).
This version includes probabilistic output in the distributionForInstance, like other MT methods.
i.e.: y[j+L] := P(y[j]|x) (this is usefull when used in an ensemble).

## BibTeX
```
@article{JesseRead2011,
   author = {Jesse Read, Bernhard Pfahringer, Geoff Holmes, Eibe Frank},
   journal = {Machine Learning Journal},
   number = {3},
   pages = {333-359},
   title = {Classifier Chains for Multi-label Classification},
   volume = {85},
   year = {2011}
}

@inproceedings{JesseRead2009,
   author = {Jesse Read, Bernhard Pfahringer, Geoff Holmes, Eibe Frank},
   booktitle = {20th European Conference on Machine Learning (ECML 2009). Bled, Slovenia, September 2009},
   title = {Classifier Chains for Multi-label Classification},
   year = {2009}
}
```
## Options
* `-S <value>`

    The seed value for randomizing the data.
    (default: 0)

* `-W <classifier name>`

    Full name of base classifier.
    (default: weka.classifiers.trees.J48)

* `-output-debug-info`

    If set, classifier is run in debug mode and
    may output additional info to the console

* `-do-not-check-capabilities`

    If set, classifier capabilities are not checked before classifier is built
    (use with caution).

* `-num-decimal-places`

    The number of decimal places for the output of numbers in the model (default 2).

* `-batch-size`

    The desired batch size for batch prediction  (default 100).

**Options specific to classifier weka.classifiers.trees.J48:**

* `-U`

    Use unpruned tree.

* `-O`

    Do not collapse tree.

* `-C <pruning confidence>`

    Set confidence threshold for pruning.
    (default 0.25)

* `-M <minimum number of instances>`

    Set minimum number of instances per leaf.
    (default 2)

* `-R`

    Use reduced error pruning.

* `-N <number of folds>`

    Set number of folds for reduced error
    pruning. One fold is used as pruning set.
    (default 3)

* `-B`

    Use binary splits only.

* `-S`

    Do not perform subtree raising.

* `-L`

    Do not clean up after the tree has been built.

* `-A`

    Laplace smoothing for predicted probabilities.

* `-J`

    Do not use MDL correction for info gain on numeric attributes.

* `-Q <seed>`

    Seed for random data shuffling (default 1).

* `-doNotMakeSplitPointActualValue`

    Do not make split point actual value.

* `-output-debug-info`

    If set, classifier is run in debug mode and
    may output additional info to the console

* `-do-not-check-capabilities`

    If set, classifier capabilities are not checked before classifier is built
    (use with caution).

* `-num-decimal-places`

    The number of decimal places for the output of numbers in the model (default 2).

* `-batch-size`

    The desired batch size for batch prediction  (default 100).
