# Step 2: Core Concepts

Before we dive into YAML definitions, let’s build a mental model of Kubernetes.
We’ll keep it light, visual.

## Cluster and Nodes

A Cluster is the whole system.

It is made of Nodes:

Control Plane: the “brain” (schedules pods, manages state).

Worker Nodes: the “muscle” (actually run the containers).

## Pods

A Pod is the smallest deployable unit in Kubernetes.

It wraps one (or sometimes a few) containers together.

Containers inside a Pod share the same network and storage.

Analogy: A Pod = container(s) in a wrapper.

## Deployments

A Deployment is a higher-level object that manages Pods.

It ensures you have the right number of replicas, handles updates, and supports rollbacks.

Analogy: A Deployment = a blueprint for Pods.

## Services

A Service exposes Pods to the network with a stable address.

Even if Pods die and restart, the Service stays constant.

Analogy: A Service = stable door to access your blueprint.

## Namespaces

Namespaces help divide a cluster into isolated “spaces.”

Useful for separating teams, environments (dev/test/prod), or projects.
