### High Performance Computing Carpentry Overview

This document outlines the idea of HPC Carpentry training. This conceptual model has been started by Martin Callaghan (@callaghanmt) from Advanced Research Computing (ARC) at Leeds University. ARC offers [HPC training](http://arc.leeds.ac.uk/training/) for the Leeds students and research staff.

The training should start with introducing case studies that are accessible to people from a wide range of research areas.

These examples should allow discussion of typical HPC uses cases:
* High Performance Computing
* High Throughput Computing
* Many Task Computing
* Big Data Analyses

1. An embarrasingly parallel problem, for example a parameter sweep data analysis using R and a suitably large data set.

2. A simple gridded finite element problem (ie. one where the problem is solved by processes communicating with each other). This introduces a problem that is best solved through parallelism.

3. A text analysis/ machine learning example using a sufficiently large data set (~ several GB, larger than might be stored in-memory on a typical desktop PC)

4. A bioinformatics example, such as multiple alignment or multiple current BLASTs
