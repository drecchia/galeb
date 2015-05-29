Galeb
===========================
[![Build Status](https://travis-ci.org/galeb/galeb.svg)](https://travis-ci.org/galeb/galeb)

Galeb is a dynamic software router built on JBOSS Undertow and XNIO.<br/>
It's a massively parallel routing system running a shared-nothing architecture.

Its main features are:
* Open Source
* API REST (management)
* Allows dynamically change routes and configuration without having to restart or reload
* Highly scalable
* Masterless (SNA - Shared nothing architecture)
* Sends metrics to external counters (eg statsd)
* Webhooks support

Building & Install
-----

```bash
$ mvn clean install
```
Using Router
-----
```bash
cd galeb-router
mvn exec:exec
```

Using API (Router)
-----
```bash
cd galeb-api
mvn exec:exec
```

Using HealthChecker
-----
```bash
cd galeb-healthchecker
mvn exec:exec
```

Using Metrics
-----
```bash
cd galeb-metrics
mvn exec:exec
```
