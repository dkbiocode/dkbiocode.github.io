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

## Templates

Example, coordination and wrapper code for different strategies of HPC workflows.

### Nextflow

* [split-run-nf](https://github.com/dkbiocode/split-run-nf): Take a large fastq file, split into chunks and run a tool, merging the output at the end. Good for parallelizing a tool that doesn't support multi-threading.


### SLURM

* [SLURM scripting pipelines](https://github.com/dkbiocode/slurm-scripting-pipelines): Implement array branching and convergence using native SLURM commands.
