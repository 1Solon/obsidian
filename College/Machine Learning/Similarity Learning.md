## Fundamentals
---
![[Pasted image 20240201110929.png]]
> * Feature Space - a D-dimensional coordinate system used to represent the descriptive features of the instances in the training data, with one axis for each feature * Similarity Metrics - the distance between instances in the feature space is a measure of the similarity of the instances

## Feature Space
---
![[Pasted image 20240201110953.png]]
> * Example: 20 college athletes and whether they were drafted by a professional team. * Descriptive features are Speed & Agility => 2-d feature space ID Speed Agility Draft ID Speed Agility Draft + 1 2.50 6.00 No 1 2.00 2.00 No + A 2 3.75 8.00 No 12 5.00 2.50 No © A + 3 2.25 5.50 No 13 8.25 8.50 No a 4 3.25 8.25 No 14 5.75 8.75 Yes + 5 2.75 7.50 No 15 4.75 6.25 Yes >0 A + 6 4.50 5.00 No 16 5.50 6.75 Yes ) a a + 7 3.50 5.25 No 17 5.25 9.50 Yes < a 8 3.00 3.25 No 18 7.00 4.25 Yes < A + 9 400 4.00 No 19 750 800 Yes A 2 10 4.25 3.75 No 20 7.25 5.75 Yes a “1 8 T uomme : ° ¢ Spseed ° ! R D U B !ﬁ‘ﬁ!ﬁ'ﬁ!ﬂ

* "Features and dimension of data are the same, so five features is the same as a five dimension table"

## Measuring Similarity
---
![[Pasted image 20240201111844.png]]
> * Similarity between instances is measured by the distance between the instances * Many distance metrics - no ‘best’ measure => problem dependent ID Speed Agility Draft ID Speed Agility Draft + 1 2.50 6.00 No 1 2.00 2.00 No 4 + 10 A 2 3.75 8.00 No 12 5.00 2.50 No © / a 3 2.25 5.50 No 13 825 8.50 No 5 4 3.25 8.25 No 14 575 8.75 Yes + 5 2.75 7.50 No 15 475 6.25 Yes >© a + 6 4.50 5.00 No 16 550 6.75 Yes ) a A + 7 3.50 5.25 No 17 525 9.50 Yes < a 8 3.00 3.25 No 18 7.00 4.25 Yes < A + 9 400 400 No 19 750 800 Yes a 16 10 425 3.75 No 20 725 5.75 Yes a o a T oo Tcveouams Athletes 4 and 5 are close to each other, low distance (high similarity) R D U é“”"l:“i'"N Athletes 10 and 19 are far from each other, high distance (low similiarity) Speed R ictesicr

## Distance Metrics
---
### Euclidian Distance

![[Pasted image 20240201112639.png]]
> * Mathematically a metric must conform to the following four criteria: 1. Non-negativity: metric(a,b) > 0 2. |dentity: metric(a,b) =0<=a=Db 3. Symmetry: metric(a,b) = metric(b, a) 4. Triangular Inequality: metric(a, b) < metric(a, ¢) + metric(b, c) * Most common distance metric is Euclidean distance which computes the length of a straight line between two points, a and b: m Euclidean(a,b) = , | Y (a[i] - b[i])® /\ pr DyBLIN R G

* Important concept: [[Euclidian Distance]]

### Manhattan Distance
![[Pasted image 20240201113623.png]]
> * Another, less well known distance measure is the Manhattan distance or taxi-cab distance Manhattan(a,b) = abs(ali] — bli]) 1=1 E ﬂf‘:, o ) (i 7 ;..5 ‘s , T uomme o Manhattan_______ ! gl N ricy DUBLJMN

* "Manhattan has a slight computational advantage over [[Euclidian Distance]]"
* [[Manhattan Distance]] 

### Minkowski Distance
![[Pasted image 20240201113919.png]]
> e Euclidean and Manhattan distances are special cases of Minkowski distance: 1 m P Minkowski(a,b) = (Z abs(ali] — b[i])p) i=1 * Different values of parameter p result in different distance measures ¢ Manhattan distance forp=1 ¢ Euclidean distance forp =2 * The larger the value of p the more emphasis is placed on features with large differences in values because these differences are raised to the power pT I < DuBLIN

* [[Minkowski Distance]] 

## Non-Numeric Data
---
![[Pasted image 20240201114134.png]]
> * Binary: Takes only two values - a boolean True/False decision e.g. married={True,False}, test result={Pass,Fail} * (Categorical (Nominal): A feature that takes values from a finite set of values, with no intrinsic ordering to the values e.g. blood group={A,B,AB,0}, nationality={French, Irish,Italian} * Ordinal: Similar to a categorical variable, but there is a clear ordering of the variables. e.g.grade={A,B,C,D,E,F}, dosage={Low,Medium,High} * Interval: Values that allow ordering and subtraction, but do not allow other arithmetic operations e.g date, time — o

