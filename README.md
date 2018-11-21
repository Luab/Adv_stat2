# Introduction

This report contains summary of my findings after doing simulated
annealing assignment. Here I investigate the effects of cooling rate on
convergence of algorithm.

# Algorithm

Resulting algorithm is not different from proposed. I tried several
sampling functions.

1.  Generate some initial and initial temperature

2.  Generate new sample given some generator function

3.  Calculate acceptance rate. Generate random number and if this number
    \<= acceptance rate - pick new sample as main one. Otherwise discard
    it.

4.  Reduce temperature by some number

5.  Repeat 2-4 until cooled.

# Effects of cooling rate

I investigated three different cooling rates. The resulting speed of
convergence is presented on following graphs. It is evident, that for
lower cooling rates better results achieved. On the other it takes
longer to converge.

# Generator function

For this assignment I tried three different generator function.

1.  Randomly reshuffle our path

2.  Swap between two random cities (with 0.00111111111 probability to
    stay on same solution)

3.  Swap three random cities

Going for bigger "number of swaps" increased exploration of algorithm
with it reaching random search for random reshuffle function. Less
number of swaps promoted exploitation, allowing to find more efficient
local solution. As a trade-off it is easier to stuck in local minima for
this functions.


I used matplotlib to create mp4 videos with my solutions. Three examples
are attached with this report.
