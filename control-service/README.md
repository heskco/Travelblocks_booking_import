# Control Service

This is the repo for Booking Imports Control Service. This service will run a scheduling service and will activate at a given 
(configurable) interval. For each interval, the control table will be read and all rows will be returned.

### Activity diagram

![](./Bookings-arch.png)

### Stack
We’ll use a simple NodeJS service with a MongoDB for our backend.
- NodeJS 7.5.0
- MongoDB 3.4.2
- Docker for Mac 1.13.0

### Control Table

ID
Import name
Service URL
3rd party URL
Credentials user
Credentials pw
Token
Parameters
Run start timestamp
Run finished timestamp
interval

### How to run the booking import microservices

We need to have docker installed previously.

```
$ bash < kraken.sh
```

This will basically install every microservice and setup the docker swarm cluster

and deploy every docker service in the swarm.

To monitor the cluster in a graphic mode we can go and visit the following url: `http://192.168.99.100:9000`

and this will give us the rancherOS web interface.
