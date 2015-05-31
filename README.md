Galeb
===========================

[**http://galeb.io**](http://galeb.io) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Build Status](https://travis-ci.org/galeb/galeb.svg)](https://travis-ci.org/galeb/galeb)
[![Circle CI](https://circleci.com/gh/galeb/galeb.svg?style=svg)](https://circleci.com/gh/galeb/galeb)
<img src="https://codeship.com/projects/edcc4d90-e9b2-0132-feb9-32dfa18a9fce/status?branch=master" height="18px">
<br/><br/>
**Galeb** is a dynamic software router/load balance L7 built on **JBoss Undertow** and **XNIO**.<br/><br/>
It's a massively parallel routing system running a shared-nothing architecture.

Its main features are:
* Open Source
* API REST (management)
* Allows dynamically change routes and configuration without having to restart or reload
* Highly scalable
* Masterless (SNA - Shared nothing architecture)
* Sends metrics to external counters (eg statsd)
* Webhooks, SPDY & HTTP2 support (draft)

Quick Start
-----
See [Galeb Now](https://github.com/galeb/galeb-now)


Diagram
-----
![Galeb cluster diagram](https://raw.githubusercontent.com/galeb/galeb/master/docs/static/diagram.png)

Requisites
-----
- Java 8
- Maven 3.3.x

Buildind & Install
-----

```bash
$ mvn clean install
```
Using Router
-----
```bash
cd galeb-router && \
mvn exec:exec < /dev/null > /dev/null 2>&1 &
```

Using API (Router)
-----
```bash
cd galeb-api && \
mvn exec:exec < /dev/null > /dev/null 2>&1 &
```

Using HealthChecker
-----
```bash
cd galeb-healthchecker && \
mvn exec:exec < /dev/null > /dev/null 2>&1 &
```

Using Metrics
-----
```bash
cd galeb-metrics && \
mvn exec:exec < /dev/null > /dev/null 2>&1 &
```

# License

```Copyright
Copyright (c) 2014-2015 Globo.com - ATeam All rights reserved.

 This source is subject to the Apache License, Version 2.0.
 Please see the LICENSE file for more information.

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
