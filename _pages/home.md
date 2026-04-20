---
layout: single
permalink: / 
sidebar:
  nav: "docs"    
hidden: true
header:
  #image: /assets/images/house-first-summer.png
  #overlay_color: "#847a62"
  #overlay_image: /assets/images/fog_road.jpeg
  actions:
    - label: "View Publications"
      url: "/Publications/"
title: "Overview"
excerpt: "**Bio-coded code** — Research scientist at Colorado State University. Building scalable workflows for genomic analysis. [Learn more about my work.](/Publications/)"   
author_profile: true
classes: wide
   
feature_row1:
  - image_path: /assets/images/WGCNA_dendrogram.png
    alt: "A Card showing WGCNA module output in the merging phase"
    image_caption: "Applying Network-based clustering methods with WGCNA"
    excerpt: "Applying Network-based clustering methods with WGCNA"
    url: "https://github.com/dkbiocode/tf-module-analysis" 
    btn_class: "btn--inverse" # feel free to change the button style!
    btn_label: "Learn More"

  - image_path: "/assets/images/Other_TFs.png" 
    alt: Heatmap of other transcription factors
    image_caption: "Clustering based on promoter binding profile of 96 Transcription Factors"
    excerpt: "Clustering based on promoter binding profile of 96 Transcription Factors"
    url: "/Analysis/" # note that these can also be full urls that take people to other sites
    btn_class: "btn--inverse" # feel free to change the button style!
    btn_label: "Learn More"

  - image_path: /assets/images/ELT2-ridgeplots.png
    alt: "Visualization"
    image_caption: "Comparison of occupancy score distributions for different gene expression classes"
    excerpt: "Comparison of occupancy score distributions for different gene expression classes"
    url: "https://github.com/dkbiocode/dash-ma-plot"
    btn_class: "btn--inverse"
    btn_label: "Learn More"

feature_row2:
  - image_path: /assets/images/workflow-nf-screenshot-highcontrast.png
    alt: "A Card showing Nextflow DSL2 code integrating channels using metadata"
    #image_caption: "Nextflow DSL2 pipeline configured for HPC optimal throughput"
    excerpt: "Tumor-normal somatic variant calling in colorectal cancer — pipeline tracks variants at targeted loci in patients as tumors become treatment-resistant across time points."
    url: "https://github.com/dkbiocode/variant-caller-nf" 
    btn_class: "btn--inverse" # feel free to change the button style!
    btn_label: "Learn More"
  - image_path: /assets/images/RAG-screenshot.png # no quotes this time
    alt: "Analysis and Algorithms"
    #image_caption: "Retrieval Augmented Generation knowledgebase"
    excerpt: "Custom AI search tool for NGS diagnostic literature — query the evidence base for sensitivity, specificity, and methodology across published studies."
    url: "https://github.com/dkbiocode/AI-knowledge-synthesis" # note that these can also be full urls that take people to other sites
    btn_class: "btn--inverse" # feel free to change the button style!
    btn_label: "Learn More"
  
  - image_path: /assets/images/MA-dash-10fps-50pc.gif
    #image_caption: "Interactive MA plot dashboard for exploring differential expression data"
    excerpt: "A custom interactive interface to hosted data (Postgres). Supports selection and inspection of gene expression data."
    url: "/Visualization/"
    btn_class: "btn--inverse"
    btn_label: "Learn More"

feature_row3:
  - image_path: /assets/images/shell-novice-screenshot.png
    alt: "Instructional projects and resources"
    image_caption: "Shell scripting tutorial environment running in GitHub Codespaces"
    excerpt: "Interactive learning environments for bioinformatics and computational biology"
    url: "/Learning/"
    btn_class: "btn--inverse"
    btn_label: "Learn More"
---

David King is a computational biologist whose work centers on the genetic underpinnings of complex biological traits. He builds the pipelines and develops the analyses that advance the biological question at hand. Learn more about his background at [About Me](About).


---

# Featured projects

{% include feature_row id="feature_row1"  %}

# Recent Development

{% include feature_row id="feature_row2" %}


# Cloud computing 

{% include feature_row id="feature_row3" %}
