[[Main memory]] is the general purpose storage that the [[Central Processing Unit|CPU]] can access directly. It is typically random access ([[Memory#Random Access Memory|RAM]]) and [[volatile]].   

User programs are usually stored in [[secondary memory]]. This requires them to be loaded into main memory before the CPU can execute them.

Often more than one program is in memory at any time. The [[operating system]] needs to manage what memory each process is using. To prevent processes from rewriting each others memory they should not be able to access another processes memory. The OS also protects its own memory from other user processes. Ensuring separate memory spaces is a way to achieving this. Each process is given a range of memory addresses it is allowed to access. 

# Base and Limit Registers
The base register is the smallest legal address a process can access. The limit register is the size of the memory range. So base + limit is the biggest address base is the lowest.

# Contiguous Memory Allocation


# Paging 
In paging the physical memory is divided into fixed sized blocks called frames. The virtual memory is divided into the same fixed size blocks as the physical memory.


## Demand Paging

The number of frames is limited by the size of the blocks and the size of the available memory. The number of pages for a process is not limited by memory size. But this means the entire virtual memory cannot be loaded into memory at the same time 