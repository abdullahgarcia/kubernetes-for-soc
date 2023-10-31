# Threat Model

## Instructions

1. Download [draw.io](https://www.drawio.com).
2. Load the latest version of the threat model.
3. Read the assumptions table and keep them in mind as they shape the threat model. You can decide to look straightaway at the official Kubernetes documentation for concepts within the assumptions, but I recommend you to do it perhaps after you have completed the rest of the instructions.
4. Explore the threat model by leveraging the draw.io layers, following the order implied by the rest of the document sections.

## About components

- **kube-apiserver**: the kube-apiserver is like the control center of a Kubernetes cluster. It's where you send your instructions for managing all the containers and applications in your cluster. This component listens to your commands and ensures that the right actions are taken to keep everything running smoothly. It acts as the central coordinator for your Kubernetes cluster, making it easier to manage and control your applications in a consistent and organized manner.
- **kube-controller-manager**: the kube-controller-manager is like the caretaker of a Kubernetes cluster. It constantly watches over the cluster's desired state and makes sure it matches the actual state. It does this by running various control loops, each responsible for different tasks like maintaining the right number of pod replicas, managing storage, and handling node-related issues. Essentially, it ensures that your cluster stays in a healthy and desired state by taking corrective actions when needed, like starting or stopping pods, maintaining resource quotas, and more. It's like the cluster's automated guardian, keeping everything in order according to your instructions and cluster policies.
- **kube-scheduler**: the kube-scheduler is like the traffic cop of a Kubernetes cluster. Its main job is to decide where new workloads, like pods, should run within the cluster. When you want to deploy a new application or scale up existing ones, the kube-scheduler selects the best node (a server in the cluster) for these workloads based on factors like resource availability and constraints. It ensures that workloads are distributed efficiently and that the cluster's resources are used wisely, helping with load balancing and optimal performance. Think of it as the cluster's smart decision-maker, directing traffic to the right destinations to keep things running smoothly.
- **etcd**: etcd is like the secret diary of a Kubernetes cluster. It's a key-value store that keeps track of all the important information about the cluster's configuration, state, and decisions. Think of it as the memory of the cluster, storing details about which applications are running, their configurations, and even information about nodes and network policies. etcd ensures that the cluster has a consistent and reliable record of everything that's happening, and it's essential for maintaining the cluster's reliability and recovery in case of failures. So, it's like the cluster's hidden librarian, preserving all the critical knowledge needed for smooth operation.
- **kube-proxy**: the kube-proxy is like the traffic guard of a Kubernetes cluster. It manages network communication between different applications and services running in the cluster. kube-proxy ensures that requests to access your applications reach the right destination by setting up network rules and routes. It handles tasks like load balancing, routing traffic to the correct pods, and managing network policies. Think of it as the cluster's traffic cop, making sure that data flows smoothly and securely between all the applications and services within the Kubernetes environment, keeping everything connected and safe.
- **kubelet**: the kubelet is like the diligent worker in a Kubernetes cluster. It runs on each node (or server) in the cluster and makes sure that the containers (pods) are running as they should. The kubelet takes its orders from the control plane, which is like the management team, and ensures that the containers are healthy. It handles tasks such as starting, stopping, and monitoring containers, and it reports back to the control plane about the container's status. It's like the on-site operator that maintains and manages the containers, keeping them in good working order and reporting any issues to the central management.
- **container runtime**: the container runtime is like the magician's hat in a Kubernetes cluster. It's the essential component that makes the actual "container magic" happen. The container runtime is responsible for pulling container images (like Docker images) from a storage location, creating running instances of containers from those images, and managing their resources. It takes care of the low-level details of running containers, like setting up their file systems and network connections. Just as a magician's hat hides the secrets of a magic trick, the container runtime hides the complexities of running containers, making it possible for your applications to work seamlessly within Kubernetes.

## About trust zones / trust boundaries

- These exist almost anywhere you can argue for different privileges.

## About connections

- Make sure to note the protocol, the version, and the port, where applicable.

## About threats

- What can go wrong? Think about a person, people, event(s), weakness(es), behavior, and idea(s).

## About threat objects

- A threat object is the combination of:
  - things you want to protect
  - something a malicious entity wants to access, control, or destroy
  - stepping stones to either of these

## About threat actors

- It is important to shift your mindset: things can go wrong internally, not only externally.

## About attack vectors and attack paths

- An attack vector is the method that a malicious actor uses to carry out a cyberattack or any kind of malicious activity. Make sure to pay attention to each attack path and the trust zones it traverses.

## About controls

- These controls have a specific place in the threat model alluding to the component they relate to.
