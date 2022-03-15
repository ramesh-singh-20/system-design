## system-design

### Understand difference between Relational and NOSQL databases

Horizontal scaling is more desirable for large scale applications due to the limitations of
vertical scaling.

Introduce load balancers before your servers to evenly distribute the load and provide more fault tolerant
and highly available systems.

On database end, we can implement master/slave database replication strategy. Since most applications
have more ratios of read operations than write operations, master DB can be used for create/update/delete 
and multiple slaves can be used for read operations.

To improve load response time introduce cache and move static contents to a content delivery
network or CDNs (such as Amazon's CloudFront).

When saving data in cache (such as Memcache) you can define the time for which this data should remain in cache.
Think about cache eviction strategies also such LRU, LFU, FIFO.

APIs should be stateless so that they can scale better. Store states in a shared resource such as NOSQL databases.

GeoDNS service is DNS service that resolves domain names to IP addresses based on the location of the user.

Think if your system needs messaging queues.

Logging: Aggregate logs from different servers to visualize them better.
CI/CD Automation:
Metrics

### Database scaling
Database scaling can be horizontal or vertical.
Horizontal scaling also known as sharding, each time a database request comes, we can calculate the hash of the 
key to go to the correct shard.
When choosing a sharding key, one of the most important criteria is to choose a key that can evenly distributed data.







