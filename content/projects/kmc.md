+++
title = "kmc: kubernetes multi-cluster"
description = ""
date = "2019-08-21"
tags = ["projects"]
+++

kmc is a tool that makes it easy to provision a kubernetes cluster composed of nodes in arbitrary regions. kmc is especially useful for simulating an edge-computing environment, since nodes can be provisioned globally and are not limited to any single region, as kubernetes is usually deployed. 

As of now, kmc supports provisioning nodes through AWS EC2 instances and as such requires the user have an AWS account. The goal however is to have kmc be able to provision nodes across cloud computing providers (GCP, Azure, DigitalOcean etc.) and even allow arbitrary nodes to be able to be provisioned, such as any server with a public IP. kmc could then be used to manage kubernetes deployments across vendor imposed boundaries and to create a large kubernetes cluster as the backbone for multiple virtualized, logically seperate, kubernetes clusters.