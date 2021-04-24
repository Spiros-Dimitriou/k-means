## K Means fast C implementation

A piece of code that implements the [K Means algorithm](https://en.wikipedia.org/wiki/K-means_clustering) in a number of vectors. The number of vectors, 
vector dimensions and final clusters are defined in compile time. Also the vectors are
randomly generated.

#### Why describe it as fast

This implementation takes advantage of multiple cores and vector processing. OpenMP and gcc
optimization is used respectively.

#### Compile

`gcc kmeans.c -o kmeans -O3 -fopenmp`

###### Todo:

- Load vectors from a file
- Initialize centers randomly (not needed for the time)
