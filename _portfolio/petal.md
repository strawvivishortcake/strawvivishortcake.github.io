---
title: "PETAL Consortium"
excerpt: "A weekly notebook of my summer project at the Jain Lab"
collection: projects
---

Hi! Welcome to my personal notebook on my summer work at the PETAL Consortium. This summer I am working with Dr. Eric Liu and Dr. Makoto Iwasaki on characterizing transcription factor (TF) enrichment landscapes in a peripheral T-cell lymphoma (PTCL) cell line collection. Using ATAC-seq data, we have already generated TF enrichment profiles via chromVAR. My goal is to benchmark and compare these results against alternative TF enrichment methods (such as monaLisa) to understand how method choice shapes our view of chromatin accessibility and transcriptional regulation in PTCL. 

Week 0
=======
This week, I created this blog in order to keep track of the progress I am making with this project. In addition, I read the benchmark paper "On the identification of differentially-active transcription factors from ATAC-seq data" (doi: 10.1371/journal.pcbi.1011971). This paper talks about which transcription factors (TF) are differentially active by using Assay for Transposase-Accessible Chromatin with sequencing (ATAC-seq). The authors then utilized several computational methods across curated TF perturbation datasets and found that there is a tradeoff between precision and recall, so the best performing methods were chromVAR-limma and monaLisa because they are designed specificially for chromatin data. Since we have already generated the TF enrichment landscape from ATAC-seq in our PTCL cell line collection with chromVar, I can't wait to see how the TF enrichment landscape in this dataset may look like in other methods. Since I downloaded monaLisa, my goal for next week is to run it with RStudio and examine for any major patterns or trends.

Week 1-2
=======
These two weeks, I worked on creating individual heatmaps from monaLisa and HOMER on the ATAC-seq data through RStudio. I'm planning on assembling these TF enrichment score across samples and TF into a matrix as the input for heatmap plotting. My hope is to analyze the TF enrichment landscape across monaLisa and HOMER. 

Week 3-6
=======
I created combined TF heatmaps from monaLisa and HOMER on RStudio. I noticed there were many similarities between the results from HOMER and monaLisa to chromVAR. Now I plan on further analyzing the results in the PTCL cell line collection.
