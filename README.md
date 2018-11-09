# Polynomial Magic

## Showing how to get whatever radius you like from a single set of charge form factor pseudo data. 

Testing whether from a single randomly generated set of data one can always find the proton radius you want if you scan with
high order polynomials.  The radius is determined by taking the slope of the function at zero as it done with charge form
factor data.

code outline

* generate ONE set of equal spaced random data with 1000 points from 0.01 to 10 fm$^{-2}$ using standard dipole and 0.003 random errors
* ask user to pick a proton radius from 0.70 to 0.92 fm
* loop over polynomial functions to see if we find the result we want
* it fails, drop one low q2 data point and try again
* repeat until we find at polynomial that will give the answer we want

bonus code

* float the normalizing of the "rejected" low q2 data and then show all the data now gives a great fit
