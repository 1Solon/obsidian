![[Pasted image 20240129162544.png]]
> * Divide the Data into Smaller Partitions and Distribute * Instead of growing a single database until it reaches capacity on a server divide into smaller partitions that are less than capacity. If we want to grow create new partitions. So good for scalability. * Can replicate Partitions so get reliability etc * Options Horizontal and Vertical

## Horizontal Partitioning
---
![[Pasted image 20240129162607.png]]
> Different rows of a table at different sites * Advantages - — Data stored close to where it is used . efficiency — Local access optimization . better performance — Only relevant data is available . security — Unions across partitions . ease of query * Disadvantages — Accessing data across partitions . inconsistent access speed — No data replication . backup vulnerability

## Vertical Partitioning
---
![[Pasted image 20240129162626.png]]