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

![[Pasted image 20240201124258.png]]
> * Similarity based learning attempts to mimic a very human way of reasoning - this makes them more explainable - easy to interpret and understand * Can give people more confidence in the model * Lazy learning technique: Model is built at classification time rather than training time * Uses a set of local training instances to classify each query * Appropriate for heterogeneous data * Computationally more expensive as the number of training instances becomes larger * Easy to add new instances to training data for re-training to handle concept drift T oo * Important to normalise data (for all prediction algorithm NDUBUN

## Weighted k-NN Algorithm
---
![[Pasted image 20240201122801.png]]
> * In distance weighted k Nearest Neighbour algorithm some neighbours get higher weight than others . My (q) = arg max Zwi X 0t e c€classes(t) i=1 * Instead of a binary vote of 1 for the class of the neighbour, closest neighbours (those that are most similar to the query) get a higher weighting when deciding the prediction for the query * Remember: similarity = inverse of distance 1 Wi = ——————~ dist(q,d;) A

### Tuning for K
---
![[Pasted image 20240201124101.png]]
> ¢ Asimple 1-NN classifier is easy to implement. But it will be susceptible to “noise” in the data. A misclassification will occur every time a single noisy example is retrieved. * We might decide to vary the neighbourhood size parameter k to improve the predictive performance of k-NN. * Choosing between different settings of an algorithm is often referred to as hyperparameter tuning or model selection. Rod o ®. o + Using a larger k (e.g. k > 2) can sometimes & “ ° make the classifier more robust and . ° ° \q:\ « But when ks large (k=N) and classes are o2e8 “": O S unbalanced, we always predict the majority 0% % 0%06:8 : EBL” class. Foo o T

## Data Normalisation
---
![[Pasted image 20240201124121.png]]
> Consider the dataset listing salary and age information for customers and whether or not they purchased a pension plan. ID Salary Age Purchased o o 1 53700 41 No © 2 65300 37 No 2 + 3 48900 45 Yes 1o 4 64800 49 Yes 3 5 44200 30 No + 6 55900 57 Yes 0 2 +3 7 48600 26 No 2 8 72800 60 Yes Q Al 9 45300 34 No a0 10 73200 52 Yes 89 ao 2 What should the marketing dept 84 T expect for customer aged 35, with 9 & ‘ Dy Salary of 56,0007? 45000 55000 65000 5000 ,0007 Sala

![[Pasted image 20240201124146.png]]
> * Calculate distance using Euclidean distance: Salary and Age Salary Only Age Only ID Salary Age Purch. Dist. Rank. | Dist. Rank. | Dist. Rank. 1 53700 41 No | 2300.0078 2 2300 2 6 4 2 65300 37 No | 9300.0002 6 9300 6 2 2 3 48900 45 Yes | 71000070 3 7100 3 10 6 4 64800 49 Yes | 8800.0111 5 8800 5 147 5 44200 30 No |11800.0011 8 |11800 8 5 3 6 55900 57 Yes 102.3914 1 100 1 2 9 7 48600 26 No | 7400.0055 4 7400 4 9 5 8 72800 60 Yes |16800.0186 9 |16800 9 25 10 9 45300 34 No |107000000 7 |10700 7 101 10 73200 52 Yes |17200.0084 10 |17200 10 17 8 * Salary feature dominates the computation of distance, Age feature is virtually ignored * Due to the larger range in the Salary feature B

![[Pasted image 20240201124159.png]]

## Predicting Continuous Targets
---
![[Pasted image 20240201124233.png]]
