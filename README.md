## system-design

### Understand difference between Relational and NOSQL databases

Horizontal scaling is more desirable for large scale applications due to the limitations of
vertical scaling.

Introduce load balancers before your servers to evenly distribute the load and provide more fault tolerant
and highly available systems.

On database end, we can implement master/slave database replication strategy. Since most applications
have more ratios of read operations than write operations, master DB can be used for create/update/delete 
and multiple slaves can be used for read operations.

To improve load response time introduce cache and move static contents to a content delivery network or CDNs.






