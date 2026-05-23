## K8s Architecture

# What is Kubernetes?
Kubernetes is a container orchestration platform used to automate deployment, scaling, and management of containerized applications.

# Why Kubernetes?
Kubernetes solves major Docker limitations:
 - Single host limitation       vs     Cluster-based Architecture
 - No auto healing                     Auto Healing
 - No auto scaling                     Auto Scaling
 - Limited enterprise support          Enterprise-level Support



## Kubernetes Architecture
Kubernetes architecture is divided into two main parts:

1. Control Plane (Master Node)
2. Worker Node (Data Plane)

## [Control Plane Components]

### 1. API Server
- Entry point of Kubernetes
- Handles all incoming requests
- Communicates with other components

### 2. Scheduler
- Decides where pods should run
- Assigns pods to worker nodes

### 3. ETCD
- Kubernetes database
- Stores cluster information

### 4. Controller Manager
- Maintains desired state
- Handles auto healing

### 5. Cloud Controller Manager (CCM)
- Used for cloud integration
- Supports AWS, Azure, GCP



## [Worker Node Components]

### 1. Kubelet
- Ensures pods are running
- Communicates with control plane

### 2. Kube Proxy
- Handles networking
- Provides load balancing

### 3. Container Runtime
- Runs containers
- Example: containerd, CRI-O

---

## Pod Creation Flow
User Request
↓  
API Server  
↓  
Scheduler  
↓  
Worker Node  
↓  
Kubelet  
↓  
Container Runtime  
↓  
Pod Running


## Key Learnings
- Kubernetes is a container orchestration platform
- API Server is the heart of Kubernetes
- Scheduler decides pod placement
- ETCD stores cluster data
- Kubelet manages pod execution
- Kube Proxy handles networking

## What I Learned
Kubernetes helps solve Docker limitations by providing auto healing, auto scaling, and enterprise-level support.
