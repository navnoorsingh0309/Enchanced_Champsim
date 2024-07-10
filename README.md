<h1 align="center"> ChampSim Simulator Enhancements </h1>

ChampSim is an open-source trace based simulator maintained at Texas A&M University and through the support of the computer architecture community. This repository is just an enhanced version of this simulator. 

# How to work with this?

`git clone github.com/navnoorsingh0309/Enhanced_Champsim`

## Compile

ChampSim takes five parameters: Branch predictor, L1D prefetcher, L2C prefetcher, LLC replacement policy, and the number of cores. For example, `./build_champsim.sh bimodal no no lru 1` builds a single-core processor with bimodal branch predictor, no L1/L2 data prefetchers, and the baseline LRU replacement policy for the LLC.

# Traces

Traces used for the 3rd Data Prefetching Championship (DPC-3) can be found here. [https://dpc3.compas.cs.stonybrook.edu/champsim-traces/speccpu/](https://dpc3.compas.cs.stonybrook.edu/champsim-traces/speccpu/) A set of traces used for the 2nd Cache Replacement Championship (CRC-2) can be found from this link. [http://bit.ly/2t2nkUj](http://bit.ly/2t2nkUj)

Storage for these traces is kindly provided by Daniel Jimenez (Texas A&M University) and Mike Ferdman (Stony Brook University). If you find yourself frequently using ChampSim, it is highly encouraged that you maintain your own repository of traces, in case the links ever break.

# What we have done?

This project involves enhancing the ChampSim simulator to improve the accuracy of hit rates in the Last Level Cache (LLC). We introduced a priority queue mechanism and mapping strategies to better manage cache blocks and instructions. This implementation helps us to identify the least frequently used (LFU) blocks in the cache and efficiently replacing the least used blocks, thereby optimizing the cache hit rate. We maintained maps to associate instructions with different cache blocks. This mapping ensures that instructions are directed to the appropriate blocks, further improving cache management and hit rate accuracy.
