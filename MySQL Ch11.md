# Scaling MySQL

## Scalability

Difference between "scalability", "high availability", "capacity" and "performance":

"Performance" -> response time

"Scalability" -> the ability to add capacity by adding resources

"High availability" -> next chapter

Analogy with cars:

"Performance" -> how fast the car is

"Capacity" -> number of lanes time the maximum safe speed

"Scalability" -> the degree to which you can add more cars and more lanes without slowing traffic

## Scaling MySQL

"Scaling vertically" or "scaling up" -> buy more powerful servers

"Scaling horizontally" or "scaling out" -> divide work across many computers

### Scaling up

Scaling up is simpler than scaling out. There's never any question about consistency or which dataset is the authoritative one.

If you know your application will grow very large, recommend scaling out.

### Scaling out

Replication, partitioning, and sharding

The simplest and most common way to scale out is to distribute your data across several servers with **replication**
Then use the replicas for read queries.

## Load Balancing

Basic idea: to share the workload among a collection of servers.

Usual way: place a load balancer in front of the servers. It then routes incoming connections to the least busy available server.

Five common goals: scalability, efficiency, availablity, consistency




