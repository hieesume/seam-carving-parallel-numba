# SEAM CARVING GPU WITH NUMBA 

## TODO:
- [x] Sequentially version by numba no python mode.
- [x] Parallel version by numba cuda mode.
- [x] Optimize using shared memory and experiment with different block sizes for kernel functions

## Usage
### CPU Usage:
```bash
- seam_carving_cpu.py [-dx <seam_dx>] [-dy <seam_dy>] [-in <image_in>] [-out <image_out>] -test_time
```
+ dx: Number of horizontal seams to add (if positive) or subtract (if negative)
+ dy: Number of vertical seams to add (if positive) or subtract (if negative)
+ in: input image file path 
+ out: output image file path 
+ test_time: print time of each step in pipeline 

### GPU Usage:
```bash
- seam_carving_gpu.py [-dx <seam_dx>] [-dy <seam_dy>] [-in <image_in>] [-out <image_out>] -check_sum
```
+ dx: Number of horizontal seams to add (if positive) or subtract (if negative)
+ dy: Number of vertical seams to add (if positive) or subtract (if negative)
+ in: input image file path 
+ out: output image file path 
+ check_sum: use cpu's grayscale


## References
- https://andrewdcampbell.github.io/seam-carving
- https://github.com/kalpeshdusane/Seam-Carving-B.E.-Project
- https://avikdas.com/2019/07/29/improved-seam-carving-with-forward-energy.html
- https://numba.pydata.org/numba-doc/latest/cuda/index.html
