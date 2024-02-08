 # CUDA Parallel Prefix Sum Scan on vectorized Images 
 
 A Project I did for course of GPU Architechures and Programming.


 I had written a CUDA program that implements a work efficient exclusive scan as in [GPU Gems 3, Chapter 39](https://developer.nvidia.com/gpugems/gpugems3/part-vi-gpu-computing/chapter-39-parallel-prefix-sum-scan-cuda) and Executed it on a large vector of integers.

 ---

### Achievements
 - Implemented Block scanning
 - Full scan for large vectors (second and third level scan support)
 - Bank conflict avoidance optimization (BCAO)

 ---
 
## Tests

The block size for the tests was 128 and the vector size was 10000000.

 - Block scan without BCAO = 1.10294 msecs
 - Block scan with BCAO = 0.47206 msecs
 - Full scan without BCAO = 1.39594 msecs
 - Full scan with BCAO = 0.76058 msecs

### Machine:
 - CPU - Intel® Core™ i5-10300H CPU @ 4.50GHz × 12
 - GPU - GeForce RTX 1650
