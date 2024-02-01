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