###Audiences for High Performance Computing Carpentry 

(initiall notes from email from Mario Antonioletti of EPCC)

**1. Audiences with knowledge of compiled languages.**

The staple HPC techniques at the moment are OpenMP and MPI.
Other things are:

   - Differences between compiled and interpreted languages.
   - Basic optimisation techniques, e.g. how to make the best use of
     memory. Cover things like array indecing; memory architectures
     e.g. NUMA. What caches are and how you should try to use them.
   - Baselining the code performance
   - Ensuring you have regression tests (your optimisations may make
     the code go faster but they may also break it)
   - Profiling the code - understanding where the performance bottle
     necks are.
   - How to make your code go faster on different architecutres:
     multi-core systems, shared memory systems, distributed memory
     systems and the different techniques you could use, e.g.
     OpenMP, multi-threading, MPI
   - Measuring performance (improvements): speed-up, parallel
     efficiency - the impact of Amdahl's Law (limits the maximum
     parallelism that can be obtained)
   - Debugging in parallel environments...


**2. Audience with backround in interpreted languages (Python, R)**

There is some support but always seems a little big clunky though can be done.

