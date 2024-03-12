---
title: Running on a Cluster
description: Learn how to run Spin Operator on a Kubernetes cluster
categories: [Spin Operator]
tags: [Tutorials]
weight: 100
---

## Prerequisites

Please ensure that your system has all the [prerequisites]({{< ref "prerequisites" >}}) installed before continuing.

## Running on Your Kubernetes Cluster

This is the standard development workflow for when you want to test running Spin Operator on a Kubernetes cluster. This is harder than [running Spin Operator on your local machine]({{< ref "running-locally" >}}), but deploying Spin Operator into your cluster lets you test things like webhooks.

> Note that you need to [install cert-manager](https://cert-manager.io/docs/installation/) for webhook support.

To install cert-manager with the default config

```console
kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.14.3/cert-manager.yaml
```

Deploy the Manager to the cluster with the image specified by `IMG`:

```console
make deploy IMG=<some-registry>/spin-operator:tag
```

> **NOTE**: If you encounter RBAC errors, you may need to grant yourself cluster-admin
> privileges or be logged in as admin.

To create instances of your solution, apply the samples (examples) from the config/sample:

```console
kubectl apply -k config/samples/
```

> **NOTE**: Ensure that the samples has default values to test it out.

