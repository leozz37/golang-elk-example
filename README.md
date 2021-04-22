# Golang and ELK Stack Example

This is an example integrating a Golang application to Elastic stack.

## Quick Start

To get things started, you can use [docker-compose](https://docs.docker.com/compose/) to run everything:

```shell
$ docker-compose up
```

## Services

Every service on ELK stack (Elasticsearch, Logstash, Kibana and Beats) needs a container, so on `docker-compose.yml` you can check every config. In this example, we're logging into `log/go.log` file and reading it with Logstash.

For Golang, we're using [zap](https://github.com/uber-go/zap), the Uber's logging lib.
