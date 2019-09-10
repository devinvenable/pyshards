# pyshards

Automatically exported from code.google.com/p/pyshards   

This was the final note I left on the project:

Pyshards is a python and MySQL based horizontal partitioning and sharding toolkit. Horizontal partitioning is a data segmenting pattern in which distinct groups of physical row-based datasets are distributed across multiple partitions. When the partitions exist as independent databases and when they exist within a shared-nothing architecture they are known as shards. (Google apparently coined the term shard for such database partitions, and we've adopted it here.) The goal is to provide big opportunities for database scalability while maintaining good performance. Sharded datasets can be queried individually (one shard) or collectively (aggregate of all shards). Pyshards uses a hash/modulo based algorithm to distribute data.

One of the goals for this project was to provide a way to reasonably add polynomial capacity (number of original shards squared) without requiring re-balancing (re-sharding). Another goal for the project was to provide a web-based shard monitoring tool, one that would allows admins to keep an eye on resource capacity.

Pyshards is no longer under development, but many of its core functions are implemented and are stable. There are a number of other projects that provide similar functionality, but their goals and/or implementations are quite different. Here are a few:

http://www.sqlalchemy.org/ SQLAlchemy

http://couchdb.apache.org/ CouchDB

http://incubator.apache.org/cassandra/

To see what the Project Owner is up to now, visit http://www.devinvenable.com/
