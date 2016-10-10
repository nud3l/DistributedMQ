# DistributedMQ
## TU Delft/IN4391 Distributed Computing Systems
Tabster is an app focusing on easing the payment process as well as splitting the tab in the hospitality
business. Tabster uses the Command and Query Responsibility Segregation (CQRS) pattern to divide write
and read access. In this [paper](distributed-queuing-rabbitmq.pdf) an extension to the system is presented to transform the read store updater into a distributed system. Tabster is implemented with PHP framework Symfony2, the distributed message
broker RabbitMQ, the database MySQL and a search server cluster based on Elasticsearch. The objective
of this paper is to dynamically assign queues and consumers to update the read side as fast as possible.
In experiments it is shown that the distributed approach is able to handle bursty workloads better and
minimize the events stored in the queues compared to the old non-distributed approach.
