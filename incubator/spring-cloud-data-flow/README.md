# Spring Cloud Data Flow Chart

[Spring Cloud Data Flow](http://cloud.spring.io/spring-cloud-dataflow/) is a toolkit for building data integration and real-time data processing pipelines.

Pipelines consist of [Spring Boot](http://projects.spring.io/spring-boot/) apps, built using the [Spring Cloud Stream](http://cloud.spring.io/spring-cloud-stream/) or [Spring Cloud Task](http://cloud.spring.io/spring-cloud-task/) microservice frameworks. This makes Spring Cloud Data Flow suitable for a range of data processing use cases, from import/export to event streaming and predictive analytics.

## Chart Details
This chart will provision a fully functional and fully featured Spring Cloud Data Flow installation 
that can deploy and manage data processing pipelines in the cluster that it is deployed to. 

MySQL and Redis are used as the stores for Spring Cloud Data Flow state and RabbitMQ is used for the pipelines' messaging layer.

For more information on Spring Cloud Data Flow and its capabilities, see it's [documentation](http://docs.spring.io/spring-cloud-dataflow/docs/current/reference/htmlsingle/).

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ cd charts
$ helm dep update incubator/spring-cloud-data-flow
$ helm install --name my-release incubator/spring-cloud-data-flow
```

Note that this chart pulls in many different Docker images so can take a while to fully install. 
