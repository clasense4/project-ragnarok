# Project Ragnarok

Project Ragnarok is an example of how High Availability infrastructure would be running. This project is divided into 4 services. And each service needs to handle a very high traffic, expecting 10k to 100k Requests per minute.

## Requirement

1. Production and non-production environment (prod, dev, staging and benchmark) infrastructure on AWS.
2. 4 Application Services. Each of them can communicate internally or externally.
3. 1 PostgreSQL Server to serve those Application Services.
4. Elastic IP for public instances, this is needed for IP whitelisting on some provider.
5. Centralized Application and Server monitoring.
6. EC2 instances and PostgreSQL can be accessed from outside of the network via VPN.
7. Attacker instances on benchmark environment.

## Application Services

Project Ragnarok will be using JWT as the token to interchange between all services.

1. Aldebaran

Aldebaran is the entry point of Project Ragnarok. It is served as the Authentication Service.

2. Prontera

Prontera is the center of Project Ragnarok. It is served as User Service.

3. Payon

Payon is the right wing of Project Ragnarok. It is served as Social Service.

4. Morroc

Morroc is the left wing of Project Ragnarok. It is served as Transaction Service.

