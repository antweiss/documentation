---
title: Prerequisites
description: Prerequisites
weight: 1
categories: [Spin Operator]
tags: [Prerequisites]
---

The following prerequisites are required.

## Go

If building the Spin Operator from source or contributing to the development of Spin Operator then you will require [Go](https://go.dev/doc/install) version v1.22.0+ to be installed on your machine. Otherwise, please ignore this section, and move to the next prerequisite.

### TinyGo

Please also install the latest version of [TinyGo](https://tinygo.org/getting-started/install/)

## Docker

If you'd like to run Spin Operator locally, then please install [Docker](https://docs.docker.com/get-docker/) version 17.03+.

## Kubectl

If you'd like to manage your Spin applications with `kubectl`, then Spin Operator requires that you have [kubectl](https://kubernetes.io/docs/tasks/tools/) version v1.27.0+ installed.

## K3d

If running/deploying your Spin application involves the use of k3d, then the Spin Operator requires that you have [k3d](https://k3d.io/v5.6.0/?h=installation#installation) installed and that you have access to a Kubernetes v1.27.0 cluster.

## Helm

If running/deploying your Spin application involves the use of Helm, then the Spin Operator requires that you have [Helm](https://helm.sh/docs/intro/install/#helm) installed on your system.

## Spin

Please install the latest version of [Spin](https://developer.fermyon.com/spin/v2/install) on your local machine for creating Spin Apps.

## Bombardier

Installing [Bombardier](https://pkg.go.dev/github.com/codesenberg/bombardier) is **not** required to use Spin Operator. Bombardier is used in tutorials like [Scaling Spin App With Horizontal Pod Autoscaling](./scaling-with-hpa.md) to generate load to test autoscaling.

## Azure CLI

Installing [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli) is **not** required to use Spin Operator. Azure CLI is used to provision Azure Kubernetes Service (AKS) and necessary Azure resources as part of the [Running Spin Operator on Azure Kubernetes Service](./running-on-azure-kubernetes-service.md) tutorial.
