#DVWA - Container image

This repository contains the required files to run the latest version [Damn Vulnerable Web Application](https://github.com/digininja/DVWA/) as a Docker container.

There are also some helper manifests to make it possible to run it on Kubernetes

**NOTE** YOU DON'T WANT TO RUN THIS IN PRODUCTION. YOU FOR SURE DON'T WANT TO RUN THIS ON ANY PUBLIC CLUSTER OR PUBLIC CLOUD

## Running via Docker Compose

Just do a `docker-compose up -d` and access localhost:8080

## Running in Kubernetes

Deploy the manifests inside kubernetes/ directory, then access the right NodePort

I recommend running this on a cluster that can provision a PV/PVC (KinD?), or changing the manifests to contain emptyPath and loose all data once the Pods are restarted

## First login
* User is `admin`
* Password is `password`
