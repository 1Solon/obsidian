## Nearest Neighbour Algorithm (k-NN)
---
![[Pasted image 20240201120844.png]]
> * Have a set of training instances and a query to be classified * Steps: * lterate across the training instances in memory and find the instance(s) that is/are the most similar (shortest distance) to the query instance in the feature space * Make a prediction for the query instance based on the target values of the nearest neighbour(s) of the query instance * 1-NN - use the most similar/closest training instance * k-NN - use the k most similar/closest training inm

### Example
![[Pasted image 20240201120903.png]]
![[Pasted image 20240201120913.png]]

### Example: 1-Nearest Neighbour
![[Pasted image 20240201120937.png]]
> * Compute distance (using selected distance measure) of query to each training instance * Rank all instances based on calculated distance * See which is the closest to query Remember: lowest distance = highest similarity D P D A DRA Di ID SPEED AGILITY DRAFT Dist. 18 7.00 4.25 es 1.27 11 2.00 2.00 no 4.85 12 5.00 2.50 no 1.82 19 750 8.00 yes 5.06 10 4.25 3.75 no 2.61 3 2.25 5.50 no 5.15 20 7.25 5.75 yes 2.80 1 2.50 6.00 no 5.20 9 4.00 4.00 no 2.93 13 825 8.50 no 5.70 6 450 5.00 no 3.01 2 3.75 8.00 no 5.83 8 3.00 3.25 no 376 14 575 8.75 yes 584 15 4.75 6.25 yes 3.82 5 2.75 7.50 no 6.02 7 350 5.25 no 3.95 4 325 8.25 no 6.31 16 550 6.75 yes 395 17 525 9.50 yes 667

### Example 3-Nearest Neighbours
---
![[Pasted image 20240201121013.png]]
![[Pasted image 20240201121027.png]]
> * Compute distance of query to each training instance * Rank all instances based on distance * Choose the k nearest neighbours * Determine predicted target by majority vote of target of the k nearest neighbours D PEED A DRA Di ID SPEED AGILITY DRAFT Dist. 12 5.00 2.50 no 1.82 19 7.50 8.00 yes 5.06 10 4.25 3.75 no 2.61 3 2.25 5.50 no 5.15 0 - A yes 80 1 2.50 6.00 no 5.20 9 4.00 4.00 no 2.93 13 8.25 8.50 no 5.70 6 4.50 5.00 no 3.01 2 3.75 8.00 no 5.83 / 8 3.00 3.25 no 3.76 14 5.75 8.75 yes 5.84 7 Sk 52 h a9 4 sz e no oo e 16 550 6.75 yos 395 17 525 9.50 yos 667 DysBl Wyi/d bout 4§NN?\

## K-NN Algorithim
---
![[Pasted image 20240201122647.png]]
> * k nearest neighbours algorithm predicts the target class with the majority vote from the set of k nearest neighbours to the query q: k Mg(q) = argmax Z Ot; e c€classes(t) ;4 classes(t) is the set of target classes t; is the target class for instance i di,; is Kronecker’s delta 0 = { 0 XhZE Z 2 j DUBLIN - / ‘\ \ -

## Weighted k-NN Algorithm
---
![[Pasted image 20240201122801.png]]
> * In distance weighted k Nearest Neighbour algorithm some neighbours get higher weight than others . My (q) = arg max Zwi X 0t e c€classes(t) i=1 * Instead of a binary vote of 1 for the class of the neighbour, closest neighbours (those that are most similar to the query) get a higher weighting when deciding the prediction for the query * Remember: similarity = inverse of distance 1 Wi = ——————~ dist(q,d;) A