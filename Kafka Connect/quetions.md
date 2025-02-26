### Kafka Connect

49. What are the advantages of using Kafka Connect distributed mode? (Select two)
- [ ] Automatic task rebalancing
- [ ] Higher availability
- [ ] Supports single-node deployment
- [ ] Real-time message transformation

**Answer:** Automatic task rebalancing, Higher availability

**Explanation:** The advantages of using Kafka Connect distributed mode include automatic task rebalancing, which allows for dynamic scaling and fault tolerance, and higher availability through distributed processing across multiple workers.

50. What is the role of Kafka MirrorMaker in a multi-data-center Kafka deployment?
- [ ] To mirror topic data from one Kafka cluster to another
- [ ] To balance partitions across brokers
- [ ] To enable compaction of log data
- [ ] To manage consumer offsets in the source cluster

**Answer:** To mirror topic data from one Kafka cluster to another

**Explanation:** Kafka MirrorMaker is used to mirror topic data from one Kafka cluster to another in a multi-data-center deployment. This helps replicate data across data centers for disaster recovery and data locality.

51. Which configuration is required for distributed mode in Kafka Connect?
- [ ] bootstrap.servers
- [ ] broker.id
- [ ] worker.address
- [ ] connector.type

**Answer:** bootstrap.servers

**Explanation:** The `bootstrap.servers` configuration is required for distributed mode in Kafka Connect. This setting specifies the list of Kafka brokers to connect to for distributed processing.

52. Which of the following modes can Kafka Connect run in?
- [ ] Replicated and Partitioned
- [ ] Standalone and Distributed
- [ ] Consumer and Producer
- [ ] Client and Broker

**Answer:** Standalone and Distributed

**Explanation:** Kafka Connect can run in standalone mode, where a single worker processes connectors, or distributed mode, where multiple workers collaborate to process connectors across a cluster.

53. Which of the following are core concepts of Kafka Connect? (Select two)
- [ ] FileStream
- [ ] Replication
- [ ] Connectors
- [ ] Offsets

**Answer:** Connectors, Offsets

**Explanation:** Core concepts of Kafka Connect include connectors, which define the data sources and sinks, and offsets, which track the progress of data processing.

54. Which Kafka Connect components are essential for handling data pipelines? (Select two)
- [ ] Replicators
- [ ] Partitions
- [ ] Connectors
- [ ] Tasks

**Answer:** Connectors, Tasks

**Explanation:** Connectors define the data sources and sinks in Kafka Connect, while tasks are responsible for processing the data pipelines defined by the connectors.

55. Which configurations are required to optimize throughput in a Kafka Connect cluster? (Select two)
- [ ] batch.size
- [ ] max.tasks
- [ ] linger.ms
- [ ] replication.factor

**Answer:** batch.size, linger.ms

**Explanation:** Configurations like `batch.size` and `linger.ms` can be adjusted to optimize throughput in a Kafka Connect cluster. Batching messages and controlling the time between batches can improve performance.

56. What is the primary purpose of Kafka Connect?
- [ ] To enable data compaction within Kafka topics
- [ ] To provide an API for building custom Kafka producers and consumers
- [ ] To integrate external systems with Apache Kafka
- [ ] To manage Kafka clusters across multiple data centers

**Answer:** To integrate external systems with Apache Kafka

**Explanation:** The primary purpose of Kafka Connect is to integrate external systems with Apache Kafka by providing a framework for building and running connectors that import/export data to/from Kafka.