# (Locally Debiased) Region Contrast Saliency

## 1. GENERAL

This package provides the implementation of the locally debiased region
contrast saliency algorithm. Furthermore, it also provides the original
region contrast algorithm and allows to set different optional center
bias integration schemes (min, max, linear, product).

Locally debiased region contrast saliency has the advantage that it is not
center biased, which makes it a perfect candidate as a salient object 
detection algorithm for, e.g., surveillance footage or robots (i.e., image
data that was not collected/generated by a photographer). However, you can
also bias the algorithm again, in which case the algorithm also provides
state-of-the-art performance on Achanta's salient object detection dataset.

If you use any of this work in scientific research or as part of a larger
software system, you are kindly requested to cite the use in any related 
publications or technical documentation. The work is based upon:

    B. Schauerte, R. Stiefelhagen, "How the Distribution of Salient Objects 
    in Images Influences Salient Object Detection". In Proceedings of the 
    20th International Conference on Image Processing (ICIP), 2013.

## 2. COMPILING

The code can be compiled using the *build.m* script. However, tt might be 
necessary to change some of the pathes in the script, depending on your
system configuration.

The code has been successfully compiled under Mac OS X and Linux.

## 3. DEMONSTRATIONS

Threee demonstrations/visualizations are included

1. *test_region_saliency_mex.m* calculates the visual saliency for several
  included algorithms. This is the best starting point, if you want to play
  with the code.
2. *visualize_region_contrast_distance_bias.m* demonstrates the bias in the
  original region contrast algorithm.
3. *visualize_theoretical_distance_bias.m* gives an overview of how different
  metrics lead to different biases.

## 4. AUTHOR INFORMATION

### 4.1 CONTACT

[Boris Schauerte](http://cvhci.anthropomatik.kit.edu/~bschauer/ "Boris Schauerte, Homepage")

### 4.2 CODE HOSTING

Development version, feel free to commit: [LDRC@GitHub](https://github.com/bschauerte/region_contrast_saliency "GitHub repository, if you want to contribute")

### 4.3 ACKNOWLEDGEMENTS

#### 4.3.1 INSTITUTIONS

Part of this work was/is supported by the German Research Foundation (DFG)
within the Collaborative Research Program SFB 588 "Humanoid Robots" and the
Quaero Programme, funded by OSEO, French State agency for innovation.
