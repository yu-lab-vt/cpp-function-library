# cpp-function-library
This repository is a library of frequently used cpp functions.

## Content
None

## File format
accept .hpp file only

### Candidate functions
#### The functions can be provided by Wei Zheng
##### functions requires openCV & designed for openCV data (have very specific design and some problems are not solved for save time, May not add to library)

###### image processing
1. 2D/3D Principal curvature (By CC, the edge is unreliable. I have a version with removed edge)
2. 2D/3D Gaussian smooth (By CC, the edge is unreliable. I have a version with removed edge)
3. Find 3D connected components (By CC, and he gave some additional way to edit it)
4. 3D morphological erode and dialate (By CC, but they both not work correctly on z direction, just an approximation. I have aother version for it based on different approximation method.)
5. 3D convolution with manually designed filter (By CC, the filter must be independent in different directions)
6. For cv::Mat, sub2ind & ind2sub (Mat uses different way to save data)
7. gap detection and refine( By CC, I don't use them and don't know how they work, should be based on Boyu's idea)

###### function for debug
1. histogram for vector<float> (I didn't optimize it, just readable)

##### functions not requires openCV

###### functions for statistic
1. Estimate gamma distribution (based on dichotomy. I found CC also have a version of it, but I haven't read it)
2. Estimate truncated Gaussian distribution (based on dichotomy)
3. t test (by CC, I don't use it)
4. get p value of z score (based on Fouries decomposition)

###### functions for images processing
1. 3D marker-based watershed (may be slower than Matlab when there are lots of cliff)

###### network flow
1. shortest path (based on dynamic programing)
2. min cost max flow (based on SSP)
3. max flow (based on modified SSP)
4. region grow from seed based on Boyu's idea (I didn't optimize it and it's slow)


###### general (small functions, maybe too small to add them to library)
1. calculate mean, median, std, min, max, sum of a vector
2. Get unique elements of a vector
3. Get intersection of 2 vectors
...
