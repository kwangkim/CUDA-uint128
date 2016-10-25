# CUDA-uint128
A 128 bit unsigned integer class for CUDA.  Due to inefficiencies in
linking device code with nvcc, this is a header-only library.  The file
```uint128_t.cu``` is meant to be #included in source files, while
```uint128_t.cuh``` can be #included in header files that require declaration
of the uint128_t class.<br><br>

This library seeks to provide a convenient uint128_t type for use in CUDA 
code with most functions and operators defined.  Because I started this yesterday
there is still a ways to go.  Nonetheless, initial results are promising.  
So far, host and device functions for comparisons and arithmetic operations
have been defined, though division is strictly 128/64 -> 64 at this point.  
I greatly welcome input and/or collaboration on this.
