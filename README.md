Galeb
===========================
[![Build Status](https://travis-ci.org/galeb/galeb.svg)](https://travis-ci.org/galeb/galeb)

**Galeb** is a dynamic software router/load balance L7 built on **JBoss Undertow** and **XNIO**.<br/><br/>
It's a massively parallel routing system running a shared-nothing architecture.

Its main features are:
* Open Source
* API REST (management)
* Allows dynamically change routes and configuration without having to restart or reload
* Highly scalable
* Masterless (SNA - Shared nothing architecture)
* Sends metrics to external counters (eg statsd)
* Webhooks, SPDY & HTTP2 support

Diagram
-----
![Galeb cluster diagram](https://raw.githubusercontent.com/galeb/galeb/master/docs/static/diagram.png)

Building & Install
-----

```bash
$ mvn clean install
```
Using Router
-----
```bash
cd galeb-router && \
mvn exec:exec
```

Using API (Router)
-----
```bash
cd galeb-api && \
mvn exec:exec
```

Using HealthChecker
-----
```bash
cd galeb-healthchecker && \
mvn exec:exec
```

Using Metrics
-----
```bash
cd galeb-metrics && \
mvn exec:exec
```
