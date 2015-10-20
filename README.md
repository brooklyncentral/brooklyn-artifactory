# brooklyn-artifactory

## Overview

This repository contains an Artifactory HA blueprint for Brooklyn.  The complete deployed system comprises:

* Artifactory master node and one or more secondary nodes
* MySQL DB server
* NFS server
* nginx load balancer

## Deploying Artifactory

To deploy Artifactory HA with Brooklyn, complete the following steps:

* Purchase Artifactory Pro (required for HA), one license per HA node
* Edit `catalog.bom` and add values for all fields with `*_HERE` (e.g. licenses, DB password)
* Add your edited `catalog.bom` to the Brooklyn catalog
* Deploy `artifactory-ha.yaml`

Once deployment is complete, you can access your Artifactory server in your browser by navigating to the load balancer's URL.
