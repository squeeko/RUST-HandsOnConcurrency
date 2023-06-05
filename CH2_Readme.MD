One well-known answer to this question is Amdahl's law. It states that the speedup of a
computation is proportional to the inverse of the percentage of time taken by the sequential
bit plus the percentage of the parallel time divided by the total new computation units, 1/(s
+ p / N). As N tends toward infinity, 1/s == 1/(1-p), in our example, 1/(1 - (23/24)) = 24. That
is, the maximum factor speedup you can ever hope to see is 24 times, with infinite
additional capacity. Ouch.

Amdahl's law is a touch pessimistic, as noted by John Gustafson in his 1988 Reevaluating
Amdahl's Law:
"At Sandia National Laboratories, we are currently engaged in research involving
massively-parallel processing. There is considerable skepticism regarding the
viability of massive parallelism; the skepticism centers around Amdahl's law, an
argument put forth by Gene Amdahl in 1967 that even when the fraction of serial
work in a given problem is small, say s, the maximum speedup obtainable from
even an infinite number of parallel processors is only 1/s. We now have timing
results for a 1024-processor system that demonstrate that the assumptions
underlying Amdahl's 1967 argument are inappropriate for the current approach to
massive ensemble parallelism."

HashMap - Implemented with "linear probing" which is a common was to implement associative arrays. Not so common is "linear probing with Robin Hood bucket stealing" which is as follows:

"If an insertion collides with an existing element, and that element's "probe
distance" (how far away the element is from its ideal location) is higher than how
far we've already probed, swap the elements."

"(Robin Hood Hashing) leads to a new search algorithm which requires less than
2.6 probes on average to perform a successful search even when the table is nearly
full. Unsuccessful searches require only O(ln n) probes."

How to benchmark functions in your code using Criterion 
Criterion crate - https://docs.rs/criterion/latest/criterion/
Crtierion Github - https://github.com/bheisler/criterion.rs

Let's Get Rusty - Criterion Usage - https://www.youtube.com/watch?v=eIB3Pd5LBkc