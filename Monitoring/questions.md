### Monitoring and Alerting

57. Which actions must be taken to monitor a Kafka cluster's performance effectively? (Select two)
- [ ] Increase the number of consumer groups
- [ ] Enable message compression 
- [ ] Analyze broker log files regularly
- [ ] Monitor consumer group lags

**Answer:** Analyze broker log files regularly, Monitor consumer group lags

**Explanation:** To monitor a Kafka cluster's performance effectively, you should analyze broker log files regularly to identify any issues or anomalies. Additionally, monitoring consumer group lags can help ensure that consumers are processing messages efficiently and not falling behind.

58. What are the key factors to monitor in a production Kafka cluster?
- [ ] Under-replicated partitions
- [ ] Producer ID
- [ ] Consumer lag
- [ ] Log.retention.ms

**Answer:** Under-replicated partitions, Consumer lag

**Explanation:** Key factors to monitor in a production Kafka cluster include under-replicated partitions, which can indicate potential data loss or unavailability, and consumer lag, which can impact real-time processing of messages.

59. Which of the following tools is used to monitor Kafka's performance?
- [ ] ZooInspector
- [ ] Kafka-Logs Viewer  
- [ ] Kafka-Monitor
- [ ] Kafka Offset Manager

**Answer:** Kafka-Monitor

**Explanation:** Kafka-Monitor is a tool used to monitor Kafka's performance, including metrics related to brokers, topics, and partitions. It provides insights into the health and performance of a Kafka cluster.

60. Which Kafka tool is most commonly used to monitor consumer lag in real-time?
- [ ] Confluent Control Center
- [ ] Kafka Streams
- [ ] Kafka Connect
- [ ] Kafka MirrorMaker

**Answer:** Confluent Control Center
**Explanation:** Confluent Control Center is a tool commonly used to monitor consumer lag in real-time in a Kafka cluster. It provides visibility into consumer group offsets and lag, allowing for efficient monitoring and troubleshooting.