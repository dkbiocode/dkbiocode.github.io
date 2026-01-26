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

## Overview

I specialize in building reproducible, high-performance bioinformatics workflows for genomic analysis. My work bridges the gap between computational infrastructure and biological discovery, helping research teams scale their analyses efficiently while maintaining scientific rigor.

As an HPC workflow specialist at Colorado University Research Computing (CURC) and Colorado State University's Data Science Research Institute, I've supported labs, courses, and collaborators in implementing production-ready pipelines on Summit, Alpine, and Riviera HPC systems.

<img src="/assets/images/pipeline_dag_color.png" alt="Pipeline workflow figure">

## Key Achievements

### Community Impact
- **ENCODE Project Adoption**: My [seeding approach for pseudoreplicate sampling](https://github.com/meekrob/onish-summit-pipelines/blame/f15580ccd4b9ba5b8e09a97710afe6e344181bc7/ENCODE3/2c_self-pseudoreplicates.sbatch#L36) was adopted by the ENCODE consortium for their ChIP-seq pipeline
- **Open Source Contribution**: Fixed a critical bug in [deepTools](https://github.com/deeptools/deepTools/pull/1394) that prevented cluster diagnostic plots from rendering

### Technical Innovations
- **Parallel Execution Optimization**: Solved [Hisat2 collision issues](https://github.com/meekrob/DSCI512_RNAseqAnalyzers/commit/0ae11a186533f7649a91b19c4b29b28866132ad4) during parallel execution, enabling concurrent processing without data corruption
- **Workflow Scalability**: Designed strategies for parallelizing single-threaded tools through intelligent data chunking and merging

## Workflow Projects

### Nextflow Pipelines

**[split-run-nf](https://github.com/dkbiocode/split-run-nf)**
A Nextflow pipeline that parallelizes single-threaded bioinformatics tools by splitting large FASTQ files into chunks, processing them concurrently, and merging results. Ideal for dramatically reducing wall-clock time on tools that don't support native multi-threading.

### SLURM Orchestration

**[SLURM Scripting Pipelines](https://github.com/dkbiocode/slurm-scripting-pipelines)**
Advanced SLURM job arrays implementing branching and convergence patterns using native scheduler commands. Demonstrates efficient resource utilization and dependency management for complex multi-stage analyses.

### RNA-seq & ChIP-seq Workflows

**[RNA-seq Array Processing](https://github.com/dkbiocode/DSCI512_RNAseqAnalyzers)**
Redesigned an RNA-seq analysis workflow to eliminate directory collisions caused by Hisat2's temporary files during parallel SLURM array execution. This refactoring enabled multiple samples to be processed concurrently without interference, dramatically reducing total processing time for large datasets.

**[Mouse Genome RNA-seq Pipeline](https://github.com/erinosb/RNAseq_pipeline_mouse)**
Containerized end-to-end workflow processing raw sequencing reads to gene counts. Docker/Singularity containerization ensures consistent results across different computing environments and simplifies dependency management.

## ENCODE Pipeline Implementation

**[modENCODE ChIP-seq Pipeline](https://github.com/meekrob/onish-summit-pipelines/tree/master/ENCODE3)**
Complete implementation of the ENCODE3 ChIP-seq analysis pipeline on CURC Summit HPC, including:
- Adaptation of the modENCODE peak caller (SPP) for HPC environments ([changes](https://github.com/hms-dbmi/spp/compare/master...meekrob:spp:master?expand=1#commits_bucket))
- Quality control, peak calling, and reproducibility assessment
- Integration with SLURM scheduling for large-scale batch processing

## Adapted Research Tools

I've contributed to and adapted several published bioinformatics tools for HPC deployment:

**[HyperTRIBE](https://github.com/rosbashlab/HyperTRIBE/compare/master...meekrob:HyperTRIBE:master?expand=1#commits_bucket)**
Workflow for identifying RNA editing sites and modifications in mRNA transcripts.

**[Java Genomics Toolkit](https://github.com/timpalpant/java-genomics-toolkit/compare/master...meekrob:java-genomics-toolkit:master?expand=1#commits_bucket)**
Enhanced this genomic analysis toolkit (similar to bedtools and Picard) with additional functions to increase versatility.

## Philosophy

My approach to workflow development emphasizes:
- **Reproducibility**: Comprehensive version control tracking every project evolution
- **Transparency**: Well-documented code and clear dependency management
- **Reliability**: Rigorous testing ensures trustworthy data for downstream [analysis](/Analysis)
- **Scalability**: Designs that leverage HPC resources efficiently

This diligence in workflow engineering establishes a solid foundation for advanced biological discovery.

