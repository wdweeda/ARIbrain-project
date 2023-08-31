# All-Resolutions Inference Project

All-Resolutions Inference is a new statistical framework for the analysis of functional MRI data. The framework is based on closed testing methodology and allow users to analyse statistical brain maps from functional (and structural) MRI studies with unprecendented flexibility. There are already many implementations and improvements since the original [paper](https://doi.org/10.1016/j.neuroimage.2018.07.060) and this page aims to provide an overview of the latest status of these methods and give background information on the methodology. If you are new to the method, please read the [background] information. If you are ready to start analysing your data go the [implementation] section. For questions, reach out to [w].[d].[weeda]\@[fsw].[leidenuniv].[nl].

This page is work in progress...

### Background

The major problem of statistical inference in functional/structural MRI analysis is the multiple testing problem that emerges due to its massively univariate approach. The problem arises when a statisical test is perfomed on all elements of the statistical map (i.e. all voxels)
separately. Since at every test we allow a small amount of uncertainty (usually 5\%) of making a so-called false positive decision (rejecting the null hypothesis while in reality it is true), performing multiple tests greatly increases the family-wise error rate. That is, when performing multiple tests, the chances that we make at least one false positive decision increases dramatically. For example, when doing 1000 tests at 5\%, we expect 50 tests to be significant while they are actually not.

#### Standard correction methods
Explain Bonferroni, RFT, and FDR.

#### Closed-testing procedures
Explain closed-testing.

#### References

The original paper introducing ARI can be found [here](https://doi.org/10.1016/j.neuroimage.2018.07.060). The permutation based ARI method is explained [here](https://onlinelibrary.wiley.com/doi/full/10.1002/sim.9725).


### Implementation

-   ARIbrain R-package [[download](https://github.com/wdweeda/ARIbrain "ARIbrain R-package GitHub page")]
-   ARIbrain interactive R Shiny application [[download](https://github.com/wdweeda/ARIbrain-app "ARIbrain App GitHub page")]
