# [kPow for Apache Kafka®](https://kpow.io)
[![Release to DockerHub](https://github.com/operatr-io/kpow-docker/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/operatr-io/kpow-docker/actions/workflows/release.yml)
![Docker Pulls](https://img.shields.io/docker/pulls/operatr/operatr)

## Evaluate locally with Docker Compose

The following steps will start a 3-node Kafka cluster on your machine with Docker Compose and connects the latest version of kPow to that Kafka cluster with a 30-day trial licence that you have [obtained from our site](https://kpow.io/try/).

See our [User Guide](https://docs.kpow.io) for full documentation, this is the simplest configuration to get up and running in minutes.

## kPow

![kPow in action](resources/kpow-ui.png)

## Prerequisites

* Install [docker-compose](https://docs.docker.com/compose/install/)
* A valid kPow license (click [here](https://kpow.io/try/) for a 30-day trial)

## Instructions

The main folder of this repository contains a functional docker-compose.yml file. Run the application using it as shown below:

```
$ git clone https://github.com/operatr-io/kpow-local.git
$ cd kpow-local
$ vim local.env # Add your LICENSE details here
$ docker-compose up
```

### Notes

* kPow's web UI is accessible on http://localhost:3000
* The Kafka brokers are accessible with bootstrap URL `127.0.0.1:9092,127.0.0.1:9093,127.0.0.1:9094` if you want to configure other services.

## Support

Any issues? Just [raise a ticket](https://github.com/operatr-io/community/issues) or view our [docs](https://docs.kpow.io).

Contact sales@operatr.io to upgrade your trial license to a fully featured 1-month Pro license if to evaluate User Authentication, Role Based Access Control, Data Policies, Prometheus Endpoints and more.

Looking to evaluate kPow outside of Docker? kPow will run with any Kafka Cluster from v1.0+ and is also [available as a JAR file](https://kpow.io/releases) for those without Dockerized environments.

## License

Copyright © Operatr.IO 2021.
