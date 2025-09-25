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

Bioinformatic workflows and pipelines not only fosters analysis of big data, but version control tracks the evolution of a project. 
This ensures reproducibility, and understanding, of approaches that took time to mature, both in terms of code and mastery of the subject. 

My deligence with tracking changes in every project promotes the utmost reproducibility, best practice, and transparency. These qualities assure the reliability
of the data given to the [analysis phase](/Analysis), so that progress is not only efficient and advanced, but also completely trustworthy.

Here are several approaches designed to work on High Performance Computing clusters, namely Colorado University Research Computing (CURC) Summit and Alpine systems. I developed
recent pipelines on CSU's Riviera HPC associated with the Data Science Research Institute.

## Templates

Example, coordination and wrapper code for different strategies of HPC workflows.

### Nextflow

* [split-run-nf](https://github.com/dkbiocode/split-run-nf): Take a large fastq file, split into chunks and run a tool, merging the output at the end. Good for parallelizing a tool that doesn't support multi-threading.


### SLURM

* [SLURM scripting pipelines](https://github.com/dkbiocode/slurm-scripting-pipelines): Implement array branching and convergence using native SLURM commands.
