# Making dlib accessible in R
dlib is a C++ library by David E. King that contains (amongst other things) image processing and machine learning tools,
under the Boost Public License. This package makes it accessible within R, in the same way that the BH package
makes the boost header files accessible

## Installation

    devtools::install_github("ironholds/dlib")

## Inclusion in an Rcpp project

    //Example: including dlib arrays and making them available.
    #include <Rcpp.h>
    using namespace Rcpp;
    //[[Rcpp::depends(dlib)]]
    #include <dlib/array.h>
    
