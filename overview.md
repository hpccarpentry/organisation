### High Performance Computing Carpentry Overview

This document outlines the idea of HPC Carpentry training. This conceptual model has been started by Martin Callaghan ( @callaghanmt ) from Advanced Research Computing (ARC) at Leeds University. ARC offers [HPC training](http://arc.leeds.ac.uk/training/) for the Leeds students and research staff.

The training should start with introducing case studies that are accessible to people from a wide range of research areas.

These examples should allow discussion of typical HPC uses cases:
* High Performance Computing
* High Throughput Computing
* Many Task Computing
* Big Data Analyses

1. An embarrassingly parallel problem, for example a parameter sweep data analysis using R and a suitably large data set.

2. A simple gridded finite element problem (i.e.. one where the problem is solved by processes communicating with each other). This introduces a problem that is best solved through parallelism.

3. A text analysis/ machine learning example using a sufficiently large data set (~ several GB, larger than might be stored in-memory on a typical desktop PC)

4. A bioinformatics example, such as multiple alignment or multiple current BLASTs

#### Proposed training workflow:

##### 1. Motivation - case studies
The training should start with introducing case studies to demonstrate the application and advantages of using HPC for research. The case studies could be roughly divided into two types:

* HPC for complex computational problems (*HPC for software*);
* HPC for large data problems (*HPC for data*).


##### 1.1 The suggested case studies would be:

Computer parallel:

* Why do we want to parallelize (in this case)?
* Overwiev of how: 
		- (discuss threads, message passing) approach
		- present parallised code
	
|HPC for software | HPC for data|
|-----------------|-------------|
| Simple FE / GFD 'grid' parallel example (scaling).  | Bioinformatics data manipulation.|
| Text analysis; machine learning.  |Large scale data analysis in R (parameter sweep) |

These case studies is then used throughout the rest of the training to demonstrate how the end goal of analysing and breaking down the problem as well as writing parallelized algorithm, implementing it  and optimising the code can be achieved.


##### 2. Why start using HPC?

This part of training focuses on comparing the use of HPC solutions to working on a typical desktop machine. It helps students understand:

* what type of problems are relevant for HPC;
* what HPC is in terms of both hardware and software;
* what skills they need to use HPC.

A case study: Analysis with R

##### 3. Command line for HPC

This module teaches students basic to intermediate skills needed to operate in shell; which skills are also essential to work in HPC environments. It is particularly advised for students who only have used GUI environments to take this module. 

Students who already have intermediate knowledge of the command line can skip this module and move to the advanced module. 
A more advanced module on command line is available further down the training workflow. 
HPC Carpentry provides a self-assessment test allowing students to assess if they have the sufficient knowledge to skip a given module. 

##### 4. HPC Basics

This module teaches students some basic HPC concepts together with practical skills directly linked to these concepts. 

* Batch scheduler
* Data transfer
* HPC hardware architecture basics.

Typical HPC Workflows:

* Long running jobs
* Large memory jobs ("big data")
* Parameter sweeps ("bag of jobs"?)
* Parallel jobs

FIXME: Case studies for all above


##### 5. HPC Workflow management

Using scripting tools:

* [SWIFT](http://swift-lang.org/main/index.php)
* [RADICAL-Pilot](https://radicalpilot.readthedocs.org/en/stable/)


##### 6. HPC Hardware

Data transfer (see HPC Basics above)
Workflow management


##### 7. Metrics

* Scaling up
* Speeding up

Starting from a serial solution to the compute-parallel problems. Describe concepts of scaling up and speeding up. Measuring speedup for different core counts (1: serial; 2, 4, 8, 16, 32, 64 ...).

Does it scale up lineary and if not, why not? (often a "sweet spot" identified as a bottlenecks, eg. serial parts of code or I/O).

What does *time* actually mean? Wallclock time; system time etc.

##### 8. HPC vs The Cloud

HPC on the Cloud
