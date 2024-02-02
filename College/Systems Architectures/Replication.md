![[Pasted image 20240129162446.png]]
> * Multiple Copies (Replicas) of the Data Available * Advantages: — Reliability — Fast response — May avoid complicated distributed transaction integrity routines (if replicated data is refreshed at scheduled intervals) — Decouples nodes (transactions proceed even if some nodes are down) — Reduced network traffic at prime time (if updates can be delayed)

![[Pasted image 20240129162501.png]]
> * Disadvantages: — Additional requirements for storage space — Additional time for update operations — Complexity and cost of updating — Integrity exposure of getting incorrect data if replicated data is not updated simultaneously — Hard to manage especially in volatile environments

![[Pasted image 20240129162519.png]]
> * Data timeliness - high tolerance for out-of-date data may be required * DBMS capabilities - if DBMS cannot support multi- node queries, replication may be necessary * Performance implications - refreshing may cause performance problems for busy nodes * Network heterogeneity - complicates replication * Network communication capabilities - complete refreshes place heavy demand on telecommunications