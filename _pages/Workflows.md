---
layout: single
permalink: /Workflows/
class: wide
header:
  overlay_image: # some/path
title: "HPC and Workflows"
#tagline: ""
read_time: true

---

<img src="/assets/images/pipeline_dag_color.png" alt="Pipeline workflow figure">

## HPC facilitation

In addition to my own analysis work, I served as the guru for HPC helping labs, courses, and collaborators implement their pipelines at CURC.

**Selected Highlights**

* Added tools to [Java Genomics Toolkit](https://github.com/timpalpant/java-genomics-toolkit/compare/master...meekrob:java-genomics-toolkit:master?expand=1#commits_bucket)
* Hisat2 required [isolating collisions](https://github.com/erinosb/DSCI512_RNAseqAnalyzers/commit/0ae11a186533f7649a91b19c4b29b28866132ad4) when working in parallel
* My approach for [seeding pseudoreplicate](https://github.com/meekrob/onish-summit-pipelines/blame/f15580ccd4b9ba5b8e09a97710afe6e344181bc7/ENCODE3/2c_self-pseudoreplicates.sbatch#L36) sampling was adopted by ENCODE
* [I fixed a bug ](https://github.com/deeptools/deepTools/pull/1394) in deepTools that failed to invoke their cluster diagnostics plot

### modENCODE

* Adapted modENCODE peak caller installation to run on CURC Summit; [changes](https://github.com/hms-dbmi/spp/compare/master...meekrob:spp:master?expand=1#commits_bucket)
* Implemented entire modENCODE ChIP-seq analysis pipeline (ENCODE3) on Summit HPC; [code](https://github.com/meekrob/onish-summit-pipelines/tree/master/ENCODE3)

Containerized workflow for processing reads to counts for [mouse genome analysis](https://github.com/erinosb/RNAseq_pipeline_mouse/compare/master...dkbiocode:RNAseq_pipeline_mouse:master?expand=1#commits_bucket).
Reframed [RNA-seq analysis workflow](https://github.com/dkbiocode/DSCI512_RNAseqAnalyzers) workflow for array processing 
[changes](https://github.com/erinosb/DSCI512_RNAseqAnalyzers/compare/master...dkbiocode:DSCI512_RNAseqAnalyzers:master?expand=1#commits_bucket).

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

## Adapted from literature

* [HyperTRIBE](https://github.com/rosbashlab/HyperTRIBE/compare/master...meekrob:HyperTRIBE:master?expand=1#commits_bucket); workflow for finding modifications in mRNA transcripts.
* [Java Genomics Toolkit](https://github.com/timpalpant/java-genomics-toolkit/compare/master...meekrob:java-genomics-toolkit:master?expand=1#commits_bucket). Genomic analysis like bedtools, picard tools.

