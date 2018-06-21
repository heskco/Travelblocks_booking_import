# Booking Import

This is the repo for handling import of travel bookings for TravelBlocks.

### Architecture

![](./Bookings-arch.png)

### Stack
We’ll use a simple NodeJS service with a MongoDB for our backend.
- NodeJS 7.5.0
- MongoDB 3.4.2
- Docker for Mac 1.13.0

### Microservices

- [Movies Service example](./movies-service)
- [Cinema Catalog Service example](./cinema-catalog-service)
- [Booking Service example](./booking-service)
- [Payment Service example](./payment-service)
- [Notification Service example](./notification-service)
- [API Gateway Service example](./api-gateway)

### How to run the cinema microservice

We need to have docker installed previously.

```
$ bash < kraken.sh
```

This will basically install every microservice and setup the docker swarm cluster

and deploy every docker service in the swarm.

To monitor the cluster in a graphic mode we can go and visit the following url: `http://192.168.99.100:9000`

and this will give us the rancherOS web interface.

