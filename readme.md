# rank-maxrank

## Basic

* Dimension over R = 16
* Dimension over F2 = 16
* Number of precision digits = 32

## Point set generation

* Basis for 10000 digital nets are randomly selected.

## WAFOMs

* WAFOM values for c = -2, -1, 0, 1, 2 are calculated.
* Point sets are ordered by WAFOM values:
   * W(P[0]) < W(P[1]) < ... < W(P[9999]).

## Errors

* QMC integration error for cos(2^cΣx_i) are calculated.
* The rank of the errors are calculated:
    * R[i] := #{j : W(P[j]) < W(P[i])}.
* The max-rank is plotted:
    * M[i] := max{R[j] : j <= i}.

## Files

* If the first/second digit of the name of a file is i, the c-value for WAFOM/integrand is i-2.
