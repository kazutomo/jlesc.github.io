---
layout: page_project
title: OpenMP for FPGA
date: 2016-05-01
updated:
navbar: Research
subnavbar: Projects
project_url:
status: starting
topics: 
  - architectures
keywords: 
  - FPGA
  - compilation
  - OpenMP4
  - optimizations
head: cappello_f
members: 
  - finkel_h
  - yoshii_k
  - alvarez_c
---

## Research topic and goals
The end of the Moore's law poses a significant challenge for scientific computing: from the mid 2020s, performance will not improve any more from the CMOS technology progress. Reconfigurable computing presents the unique opportunity of allowing performance progress by customization while still serving a large variety of applications, offering a true co-design vehicle. However, its adoption in scientific computing still faces the lack of high-level parallel programming abstraction and the extreme difficulty of achieving high performance with existing compilation stacks.

We focus on node-level parallelism; and our objective is to demonstrate, for a set of JLESC applications parallelized with OpenMP 4, significant performance/watt improvement compared with CPUs and GPUs of the comparable technology. 

We follow a co-design approach. Because the community is investing significantly in OpenMP 4 for node-level parallelism, we will first provide a path to compile OpenMP 4 applications for high-end field-programmable gate arrays (FPGAs). Second, we explore, design, and develop new mechanisms to optimize the FPGA performance of scientific computing: (i) compiler-level optimizations; (ii) dynamic memory optimizations; and (iii) code transformation and additional, non-OpenMP 4, directives to help generate efficient computing and memory interface structures. Our co-design approach synergistically affects the programming interface and the hardware configuration.

## Results for 2015/2016
We organized an international workshop on FPGA for scientific simulation and data analytics, at Argonne on January 2016, that attracted application developers, researchers in computer science and applied mathematics, the main FPGA vendors (Xilinx and Altera), and HPC application users. 

## Visits and meetings
{% person cappello_f %} will visit BSC for two weeks in July 2016.


## Impact and publications

{% person cappello_f %}, Internal report on HPC trends: focus on Reconfigurable Architecture. ANL technical report. As part of the EDF contract for the JLESC.
The team is submitting a proposal to DOE on this topic.

{% bibliography --cited --file jlesc.bib %}


## Future plans

We will study performance portablity and code optimization techniques on selected application kernels using the latest generation FPGA platforms such as Intel Arria10 and possibly submit results to relevent venues. We will also evaluate the Merlin compiler, the best commercial compiler for FPGA accelerators, for a comparison perpose.

## References

{% bibliography --file external/fpga_project.bib %}
