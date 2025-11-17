## What is Kubernetes?

Kubernetes or k8s is an orchestration platform for containers.
It helps you manage not just one container, but thousands of them across multiple machines.

Think of it as:

Docker → runs one container (or a few, manually)

Kubernetes → manages lots of containers automatically

## Why do we need it?

Docker alone is great for building and running containers. But when you need to run applications at scale, Docker by itself isn’t enough.

Problems without Kubernetes:
- How do you run the same container on multiple machines?
- How do you restart a crashed container automatically?
- How do you balance traffic between multiple containers?
- How do you scale up or down when demand changes?

Kubernetes solves all of this by providing:
- Orchestration → automatically runs containers across a cluster
- Scaling → increase or decrease replicas based on load
- Self-healing → restarts crashed containers, reschedules them if a machine fails
- Service discovery → provides stable addresses so containers can talk to each other