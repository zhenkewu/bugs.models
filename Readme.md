What is in here?
-----------------
This repository contains several `.bug` files that are used in Bayesian inference for the package `nplcm`. They are required files in WinBUGS. We recommend calling WinBUGS or other Bayesian softwares from R, e.g. `R2WinBUGS`. We will soon incoporate either R-self-sustained inference program or incorporate `OpenBUGS` or `RJAGS` that can be run reliably on OS X.

Note to user
------------
Current implementation requires that if there are pathogens with both
Bronze-standard (BrS) and Silver-Standard (SS) measurements, the number is at least 2; 
if there are pathogens with SS only measurements, the number is also at least 2. 
The reason is that the matrices or vectors specified in `.bug` files will not be compiled if the column of matrix or the vector length is 1.

Otherwise, we need to write new code.

