This file explains how the simulation tables in the paper "equential Estimation and Inference in Games of Incomplete Information with Non-separable Unobserved Heterogeneity" are generated.

Table I: "datagen_18.m" generates data used in this table. "mix_18_8_auto_all_usedata.m" generates all rows corresponding to l1=8,
"mix_18_9_auto_all_usedata.m" generates all rows corresponding to l1=9 and so on.

Table II: "datagen_27_05.m" generates data used in this table. "st27_la10_Delta1.m" generates all rows corresponding to Delta=1,
"st27_la10_Delta2.m" generates all rows corresponding to Delta=2 and so on.

Table III: Under folder "game1", matlab file "newSt18.m" generates time, CSR and MSE for game1 for a particular value of ns. Run this file 
for ns=250, 500, 750, 1000 generates all rows corresponding to Design1 in game1. Similarly, run files "newSt27.m", "newSt64.m" and "newSt100.m"
at these values of ns generates all rows corresponding to Design2-4, respectively. Under folder "game2", matlab file "x3_St24.m" generates time,
CSR and MSE for game 2 for a particular value of ns.Run this file for ns=250, 500, 750, 1000 generates all rows corresponding to Design1 in game2. 
Similarly, run files "x3_St36.m", "x3_St54.m" and "x3_St81.m" at these values of ns generates all rows corresponding to Design2-4, respectively.

Table IV: "datagenDelta_test500.m",...,"datagenDelta_test1250.m" computes null rejection probabiity for ns=500,...,1250 respectively under the first restriction using a supercomputer managed by slurm.
"datagenDelta_subtest500.m",...,"datagenDelta_subtest1250.m" computes null rejection probabiity for ns=500,...,1250 respectively under the second restriction using a supercomputer managed by slurm.

  
Table V: "cpowerm01_test500.m" computes the rejection probability for ns=500 and a negative deviation of 0.1 from the first null hypothesis on a supercomputer managed by slurm, where m in the name stands for the minus sign.
"cpowerp01_test500.m" computes the rejection probability for ns=500 and a positive deviation of 0.1 from the first null hypothesis on a supercomputer managed by slurm, where p in the name stands for the plus sign.
Similarly, for all other files whose name takes the form of "cpowerdev_testns.m".
"power500R2m01.m" computes the rejection probability for ns=500 and a negative deviation of 0.1 from the second null hypothesis on a supercomputer managed by slurm, where m in the name stands for the minus sign.
"power500R2p01.m" computes the rejection probability for ns=500 and a positive deviation of 0.1 from the second null hypothesis on a supercomputer managed by slurm, where p in the name stands for the plus sign.
Similarly, for all other files whose name takes the form of "powernsR2dev.m".

Note that the aforementioned files for creating Table IV and Table V only creates raw output from each node of the supercomputer. The raw outputs need to
be combined using a file "combine.m" to produce the final output. For details regarding job submission on a supercomputer, the slurm platform and the "combine.m" file,
please read "Guide on using slurm.txt" and "slurm_job_submission_file.txt".

         


