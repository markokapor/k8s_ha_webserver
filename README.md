# Kubernetes manifest files used of HA web server deployment

This repository contains YAML manifest files that can be used to deploy Highly Available webservers that host static content behind a HAProxy load balancer with Grafana used for cluster/HAproxy monitoring.

## Manifest files are divided in following categories:
* haproxy
** contains manifest files needed to deploy HAProxy and connect it to backend webservers and service to expose it to external network
* metallb
** provides LoadBalance services capability if Kubernetes is installed on-premise and doesn't provide this capability
* monitoring
** contains everything needed to setup Prometheus and Grafana for cluster/HAProxy monitoring
* namespaces
** manifest files used to create necessary namespaces
* network
** manifest file for calico network layer
* webserver
** contains manifest files needed to deploy webserver backend