# Naming Server for Subscriber Management System (SMS)

## Overview

The Naming Server is responsible for service discovery in the Subscriber Management System (SMS). It allows microservices to find and communicate with each other.

## Architecture

- **Spring Boot**: The core framework used to build the Naming Server.
- **Eureka Server**: Provides service discovery capabilities.

## Features

- **Service Discovery**: Allows microservices to register and discover each other.



## Configuration

Configuration for the Naming Server is done through `application.yml` or `application.properties`. Below is an example configuration in `application.yml`:

```yaml
server:
  port: 8761

spring:
  application:
    name: naming-server

eureka:
  client:
    registerWithEureka: false
    fetchRegistry: false
  server:
    waitTimeInMsWhenSyncEmpty: 0
