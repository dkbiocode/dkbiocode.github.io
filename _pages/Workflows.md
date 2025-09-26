---
layout: single
permalink: /Workflows/
class: wide
header:
  overlay_image: # some/path
title: "Workflows"
#tagline: ""
read_time: true

---

<img src="/assets/images/pipeline_dag_color.png" alt="Pipeline workflow figure">

## HPC facilitation

With my diverse technical background, I created a software system on HPC for use in the absence of a module system for bioinformatics packages. 

Before widely adopting conda, we tried different approaches, including 
Singularity containers and a local shared setup of installations that functioned like a virtual environment.

**Here are some examples:**

* Containerized workflow for processing reads to counts in [mouse](https://github.com/dkbiocode/RNAseq_pipeline_mouse); [changes](https://github.com/erinosb/RNAseq_pipeline_mouse/compare/master...dkbiocode:RNAseq_pipeline_mouse:master?expand=1).
* Reframed RNA-seq analysis workflow for array processing. Analyzed hisat2 discrepancies in [DSCI512 course repo](https://github.com/dkbiocode/DSCI512_RNAseqAnalyzers); [changes](https://github.com/erinosb/DSCI512_RNAseqAnalyzers/compare/master...dkbiocode:DSCI512_RNAseqAnalyzers:master?expand=1)
* Fixed a bug in deepTools; [pull request](https://github.com/deeptools/deepTools/pull/1394)

### modENCODE

* Adapted modENCODE peak caller installation to run on CURC Summit; [changes](https://github.com/hms-dbmi/spp/compare/master...meekrob:spp:master?expand=1)
* Implemented entire modENCODE ChIP-seq analysis pipeline (ENCODE3) on Summit HPC; [code](https://github.com/meekrob/onish-summit-pipelines/tree/master/ENCODE3)
    * Interesting note: My solution for seeding random variates was adopted by ENCODE: [function](https://github.com/meekrob/onish-summit-pipelines/blame/f15580ccd4b9ba5b8e09a97710afe6e344181bc7/ENCODE3/2c_self-pseudoreplicates.sbatch#L36)


## Workflows

Bioinformatic workflows and pipelines not only fosters analysis of big data, but version control tracks the evolution of a project. 
This ensures reproducibility, and understanding, of approaches that took time to mature, both in terms of code and mastery of the subject. 
 
My deligence with tracking changes in every project promotes the utmost reproducibility, best practice, and transparency. These qualities assure the reliability
of the data given to the [analysis phase](/Analysis), so that progress is not only efficient and advanced, but also completely trustworthy.
 
Here are several approaches designed to work on High Performance Computing clusters, namely Colorado University Research Computing (CURC) Summit and Alpine systems. I developed
recent pipelines on CSU's Riviera HPC associated with the Data Science Research Institute.



### RNA/ChIP-seq


* [split-run-nf](https://github.com/dkbiocode/split-run-nf): Take a large fastq file, split into chunks and run a tool, merging the output at the end. Good for parallelizing a tool that doesn't support multi-threading.


### SLURM

* [SLURM scripting pipelines](https://github.com/dkbiocode/slurm-scripting-pipelines): Implement array branching and convergence using native SLURM commands.
