# ChampSim Simulator Enhancements
## Overview
This project involves enhancing the ChampSim simulator to improve the accuracy of hit rates in the Last Level Cache (LLC). We introduced a priority queue mechanism and mapping strategies to better manage cache blocks and instructions.

## Enhancements
Priority Queue for LFU Blocks
We implemented a priority queue to identify the least frequently used (LFU) blocks in the cache. This helps in efficiently replacing the least used blocks, thereby optimizing the cache hit rate.

## Instruction to Block Mapping
We maintained maps to associate instructions with different cache blocks. This mapping ensures that instructions are directed to the appropriate blocks, further improving cache management and hit rate accuracy.
