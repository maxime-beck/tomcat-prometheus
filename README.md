# Openshift - Monitoring Tomcat JMX Metrics with Prometheus
The purpose of this repository is to demonstrate how to monitor Openshift Tomcat Containers using Prometheus. It contains a deployable pre-configured, Prometheus enabled, Tomcat Sever.

## Quick Start
To deploy the pre-configured Tomcat Container, start by logging into your Openshift Server with a `cluster-admin` user and run the following commands:
```
oc new-project tomcat-prometheus
oc create -f deploy-project.yaml
oc create -f deploy-operator.yaml
```
Then, simply go to http://prometheus-operated-tomcat-prometheus.router.default.svc.cluster.local/graph to access your Prometheus UI.