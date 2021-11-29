# Gem5-Arch1  
### Info about System
* Minor CPU model
* 1Ghz at 3,3 V at line 100  
* ddr3 1600 8X8  
* 2 channel memmory
* 2gb memmory  

We can change the cpu frequency with --cpu-freq

l1 instruction cache l1data cache walk cach l2 cache 

#### Info about stats.txt
sim_seconds is Number of seconds simulated and its value was 0.000035  
sim_insts is Number of instructions simulated and its value was 5027  
host_inst_rate is the simulator instruction rate and its value was 19577  

IL1.miss 327  
DL1.miss 177  
L2.miss 424  
CPI = 6.316


### CPU types :  
* BaseSimpleCPU : basis of AtomicSimple and TimingSimple can't run on each own
* AtomicSimpleCPU : Derived from BaseSimple, atomic memory accesses
* TimingSimpleCPU : Derived from BaseSimple, timing memory accesses
* O3CPU
* TraceCPU : fast version of O3 cpu model for memory-system performance exploration
* Minor CPU Model : Fixed pipeline but configurable data structures and execute behavior

MinorCPU : 0.000034  
TimingSimpleCPU : 0.000039  

MinorCPU at 10Ghz : 0.000029
TimingSimpleCPU at 10Ghz : 0.000028

TimingSimpleCPU changes more with frequency

MinorCPU with DDR4_2400_16x4 memory : 0.000033
TimingSimpleCPU with DDR4_2400_16x4 memory : 0.000039  

CPUs don't seem to be effected by the change of memory type.  
The MinorCPU is slightly faster but it is within margin of error    



Source: [gem5 cpu models](www.gem5.org/documentation/general_docs/cpu_models)
