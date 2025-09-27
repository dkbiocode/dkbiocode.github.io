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

As genomic data analysis becomes increasingly AI-driven, experience with conventional statistics helps me understand the limitations, and the potential, of the new innovative practices. 

The following examples highlight hypothesis-driven statistics that test the interrelation between two molecular phenomena, transcription factor occupancy and gene expression. We mentally idealize these processes to match the cartoons in our textbooks, but large datasets tell a different story. 

<img src="/assets/images/ELT2-ridgeplots.png" alt="Ridgeplots and Tukey HSD">
[Learn more about this analysis](#tukey-honest-significant-differences)

## Multivariate/Multifactor Analysis

Big data has the implicit challenge of deriving meaning from multiple different factors. I used the following methods to conceptualize and explore associations between groups
of transcription factor binding, *C. elegans* developmental stage, gene expression level, and genetic modification.

These methods go beyond repeating simple statistical tests for all group levels and comparisons. They have a full concept of the data and the statistical question, do not exclude groups unconsidered in our framing of the question, and account for multiple comparisons.

### Sankey 

**Question**: Do promoters/genes change activation status through developmental time?

This is not a statistic, but a visualization of data cohesion.

<img src="/assets/images/sankey_plot_ELT2.png" alt="Sankey Analysis">

### Mosaic plot

**Question**: What are the profiles of ELT-2 binding with regard to life stage and genetic effect?

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

### Correspondance analysis

### Categorical regression

### Clustering

**Question:** What other transcription factors might explain gene expression in the intestine?

The search continues for explanatory transcription factors. In <i>C. elegans</i>, there is a well-curated set of transcription factors. Many of these are known
to be expressed in the intestine, and many were studied in the modENCODE project with ChIP-seq. This analysis identifies genome-wide patterns of binding.

<img src="/assets/images/Other_TFs.png" alt="Heatmap of other transcription factors">


