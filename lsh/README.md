# P1

# Locality Sensitive Hashing
* Large scale similarity matching.
* used in recommendation and search.



# P2


# Smiliar Article (Toy Case)

d1 : “Who was the first king of Poland”

d2 : “Who was the first ruler of Poland”

d3 : “Egypt”

id|who|was|the|first|king|ruler|of|poland|egypt
--|---|---|--|------|----|-----|--|------|-----
1 | 1 | 1 | 1|  1   |  1|   0  | 1|   1  |   0|
2 | 1 | 1 | 1|  1   |  0|   1  | 1|   1  |   0|
1 | 0 | 0 | 0|  0   |  0|   0  | 0|   0  |   1|


suppose we have $N$ docuemnts.

find similar documents by similarity function

time complexity : $O(N^2)$
space complexity : $O(1)$

# P3

# time compleixty --> space compleixty ?

Yes! hashing!

<img src='./assets/lsh_1.png'></img>

[ref](https://towardsdatascience.com/understanding-locality-sensitive-hashing-49f6d1f6134)

the mathematician do the work.

the magic hash function - hash similar document to the same bucket **approximately**.

suppose we have $N$ docuemnts, $K$ hash buckets.

time complexity : $O(N)$

space complexity : $O(K)$

# P4

# Demo