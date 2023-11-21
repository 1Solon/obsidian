* "Real time, Main - Database"
* Present in RAM, low latency
* Orders of magnitude faster then hybrid database
* Hybrid defined by using disk and ram
* RAM is very expensive, limits availability
* Memory loss is a concern, as it is volatile
* Unexpected shutdown can result in database deletion
* Certain providers have greater safety
* Useful for caching, means that you do not use disk as often
* High throughput- can conduct larger reads and writes ???  `RAM is smaller then disk, how can it be bigger?`
* Real time analytics -> real time stuff
* Useful for bidding databases
* Oracle TimesTen is the example for this presentation
* Mid 90s created at HP labs
* company spun out and was eventually bought by Oracle
* ^(2005)
* TT classic is not supported currently, but refers to the old version before buyout
* Cache provides caching services to databases
* TT ScaleOut provides a system as a service TT
* TimesTen XE offers a cut-down service ??? `What is the benifit?`
* Setup seems very complicated
* TTISQL used to connect
* Seems to use standard SQL? ??? `What version of SQL does it support?`
* Hybrid databases use disk and ram elements
* Supports structured and unstructured data
* Useful in scenarios where rapid access is desired but large storage is also desired
* 