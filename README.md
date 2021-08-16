# mqtt

## comparison to http

smaller packet size than http 

min battery loss, min bandwidth 

## acronym 

MQ telemetry transport 
NOT message queue 

## recommended version 

MQTT 5 

## pub/sub pattern 

decouples client that sends messages (publisher) from client that receieves messages (subscribers) 
adds broker layer (sits between publisher and subscriber)

more scalable than client-server
scale broker with cluster of nodes 

time decoupling - pub/sub don't need to run at same time

synchronization decoupling - no blocking between pub/sub when publishing or receiving

space decoupling - pub and sub don't need to make a connection (ip address, port)

message filtering - 3 ways - 
1.  subject/topic
2.  content
3.  type (Obj oriented)

## vs message queues 

mq: queue stores message until consumed 
mqtt: depends on if there is subscriber 

mq: message only consumed by one client
mqtt: broadcast to every subscriber

mq: queue named and must be created explicitly 
mqtt:  can be created on the fly 