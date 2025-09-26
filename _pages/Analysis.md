---
layout: single
permalink: /Analysis/
class: wide
header:
  overlay_image: # some/path
title: "Analysis"
#tagline: ""
read_time: true

---

Data analysis is the funnest part of research.  It goes from mystery to discovery, even if that process ends at an exploratory phase. In the current 

<img src="/assets/images/ELT2-ridgeplots.png" alt="Ridgeplots and Tukey HSD">
[Learn more about this analysis](#tukey-honest-significant-differences)

## Multivariate/Multifactor Analysis

Big data has the implicit challenge of deriving meaning from multiple different factors. I used the following methods to conceptualize and explore associates between groups
off transcription factor binding, *C. elegans* developmental stage, gene expression level, and genetic modification.

These methods go beyond repeating simple statistical tests for all group levels and comparisons. They have a full concept of the data and the statistical question, do not exclude groups unconsidered in our framing of the question, and account for multiple comparisons.

### Sankey 

**Question**: Do promoters/genes change activation status through developmental time?

This is not a statistic, but a visualization of data cohesion.

<img src="/assets/images/sankey_plot_ELT2.png" alt="Sankey Analysis">

### Mosaic plot

**Question**: Are there classes of transcription factor binding 

When looking for associations among multiple factors, a Chi-sq test can be used to determine if any combinations are represented more or less than 
expected.  However, the &chi;<sup>2</sup> test only gives an overall *p-value*. There are methods to study the &chi;<sup>2</sup> residuals in order to see where the 
data deviate from random expectation.

<img src="/assets/images/mosaic_plot.png" alt="Mosaic Plot">

### Tukey Honest Significant differences

**Question**: Does transcription factor binding correlate with gene expression level?

<img src="/assets/images/ELT2-ridgeplots.png" alt="Ridgeplots and Tukey HSD">

With ANOVA, ask whether groups better explain the data. Our data has groups of many levels, and therefore must apply multiple tests, and corrections, to control statistical rigor.
This analysis did not find the ELT-2 bound genes to be higher expressed. Most of the genes are known to be ELT-2 dependent, therefore this result suggests that the dependence is
qualitative, not quantitative.

### Adapted from literature

* [HyperTRIBE](https://github.com/rosbashlab/HyperTRIBE/compare/master...meekrob:HyperTRIBE:master?expand=1#commits_bucket); workflow for finding modifications in mRNA transcripts.
* [Java Genomics Toolkit](https://github.com/timpalpant/java-genomics-toolkit/compare/master...meekrob:java-genomics-toolkit:master?expand=1#commits_bucket). Genomic analysis like bedtools, picard tools.

