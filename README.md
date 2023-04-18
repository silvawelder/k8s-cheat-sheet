# k8s-cheat-sheet

## Teory

### Understanding Kubernetes Resource (CPU and Memory) Units

Kubernetes is an open-source container orchestration platform that allows you to deploy, manage, and scale containerized applications. It provides abstractions for defining and managing resources, such as CPU and memory, for containers running on a cluster of machines. In Kubernetes, CPU and memory units are used to specify the amount of computing resources that can be allocated to a container.

#### CPU Units in Kubernetes:

CPU units in Kubernetes are represented using a numeric value followed by a unit suffix. The unit of CPU in Kubernetes is "CPU cores". The CPU cores represent the processing power of a single physical or virtual CPU core. For example, the following are some common CPU unit suffixes used in Kubernetes:

m: Represents milli-CPU, which is 1/1000th of a CPU core. For example, 100m represents 0.1 CPU core.

CPU core: Represents a whole CPU core. For example, 1 represents 1 CPU core.

#### Memory Units in Kubernetes:

Memory units in Kubernetes are also represented using a numeric value followed by a unit suffix. The unit of memory in Kubernetes is "bytes". However, for practical reasons, memory units in Kubernetes are usually expressed using base-2 units, such as MiB, GiB, and TiB, instead of the traditional base-10 units, such as MB, GB, and TB. For example, the following are some common memory unit suffixes used in Kubernetes:

Ki: Represents kibibyte, which is 2^10 bytes or 1024 bytes.

Mi: Represents mebibyte, which is 2^20 bytes or 1,048,576 bytes.

Gi: Represents gibibyte, which is 2^30 bytes or 1,073,741,824 bytes.

Ti: Represents tebibyte, which is 2^40 bytes or 1,099,511,627,776 bytes.

It's important to note that when specifying CPU and memory resources for containers in Kubernetes, you need to consider the actual CPU and memory capacity of the nodes in your cluster to avoid overprovisioning or underprovisioning of resources, which can impact the performance and stability of your containerized applications.
