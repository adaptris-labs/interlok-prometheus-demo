# interlok-prometheus-demo

## What is this

This is a complete interlok instance show-casing generated metrics being fired into Prometheus and then viewed in a Grafana dashboard.
Containers installed in this demo;
 - Interlok
 - Prometheus Pushgateway
 - Prometheus Engine
 - Grafana

## Quickstart

* You'll need java of course because gradle is the build system.
* Docker of course
* Either run `docker-compose up` or `./gradlew dockerComposeUp`

## Resources

A full guide can be found here;

* https://interlok.adaptris.net/interlok-docs/advanced-profiler-prometheus.html

Other resources;

* https://hub.docker.com/r/prom/prometheus
* https://hub.docker.com/r/grafana/grafana

## Gradle flags

You can control some behaviour by passing in project properties in the form *-PpropertyKey=value*

Property Key | Default Value | Description | Notes
------------ | ------------- | ----------- | -----
releaseVersion|latest|The docker tag version ||
dockerImageName|adaptrislabs/interlok-solace| The docker image name||
buildEnv|docker|Change it to anything else to drive local properties from your hostname| This directly affects the way property files are sourced, by default it will be `variables.propertes.{buildEnv}`|


