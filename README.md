# mantel_test
A python version of performing mantel test of two matrices. The original R version of mantel test is mantel.test.R, which is from the ape package (https://cran.r-project.org/web/packages/ape/index.html). 

## License
This package is free and open source software, licensed under GPL(>= 2).
 
## Usage
import mantel_test
import pandas as pd
x = pd.DataFrame({"a":[0,1,2], "b":[1,0,3], "c":[2,3,0]})
y = pd.DataFrame({"a":[0,2,7], "b":[2,0,6], "c":[7,6,0]})
mantel_test(x,y)

## Note
There may be a minor difference between the pvalue from R version and python version, which is caused by the random sampling process during permutation test.

## Contact information
wggucas@gmail.com
