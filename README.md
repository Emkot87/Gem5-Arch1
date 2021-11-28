# Gem5-Arch1  
### Info about System
* 1Ghz @ line 100  
* ddr3 1600 8X8  
* 2 channel memmory  
* 2gb memmory  


l1 instruction cache l1data cache walk cach l2 cache 

#### Info about stats.txt
sim_seconds is Number of seconds simulated and its value was 0.000035  
sim_insts is Number of instructions simulated and its value was 5027  
host_inst_rate is the simulator instruction rate and its value was 19577  



### CPU types :  
* BaseSimpleCPU : basis of AtomicSimple and TimingSimple can't run on each own
* AtomicSimpleCPU : Derived from BaseSimple, atomic memory accesses
* TimingSimpleCPU : Derived from BaseSimple, timing memory accesses
* O3CPU
* TraceCPU : fast version of O3 cpu model for memory-system performance exploration
* Minor CPU Model : Fixed pipeline but configurable data structures and execute behavior


Source: [gem5 cpu models](www.gem5.org/documentation/general_docs/cpu_models)
