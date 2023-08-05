Here we will put some ML algorithms as I learn them on the way.

## FFT :

## PageRank :
PR(A) = (1-d) + d (PR(T1)/C(T1) + ... + PR(Tn)/C(Tn))
where:

-   PR(A) is the PageRank of page A,
-   PR(Ti) is the PageRank of pages Ti which link to page A,
-   C(Ti) is the number of outbound links on page Ti and;
-   d is a damping factor which can be set between 0 and 1.

A particular page is ranked recursively depending on what other pages link to it.

## Monte Carlo :
This [important algorithm](http://ib.berkeley.edu/labs/slatkin/eriq/classes/guest_lect/mc_lecture_notes.pdf) is used to approximate solutions to numerical problems of unmanageable complexity by mimicking a random process. It relies on repeated random sampling to obtain a result - in effect using randomness to solve problems that might be deterministic in principle.


[[self-notes]]



## MM algorithm - minorize-maximize
