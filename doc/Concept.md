This document aims to align three tools for growing Kubernetes clusters in a local environment: Minikube, kind and k3d. The leather tool has its own characteristics and significance, which should be considered when choosing a PoC for the startup “AsciiArtify”.

Description of tools and their purposes
Minikube
Minikube is a local Kubernetes system running directly on a Kubernetes cluster on one computer. It allows developers to quickly fine-tune and test their additions in a local environment without the need to access the real world. Minikube is supported on Windows, macOS and Linux and has a set of useful tools for monitoring and cluster maintenance.

kind (Kubernetes IN Docker)
Kind is a tool that allows you to create local Kubernetes clusters in Docker containers. It uses Docker for developing a Kubernetes cluster, which allows you to quickly create a middle ground for testing and development. Kind is easy to use, but lacks the possibility of automation and additional functions such as monitoring.

k3d
K3d is a tool for creating local Kubernetes clusters in Docker containers running Rancher Kubernetes Engine (RKE). It allows you to easily create and test Kubernetes clusters in Docker containers, and also supports monitoring and clustering, making it an additional option for developers.

These three tools can be used to develop a local Kubernetes cluster for the PoC startup "AsciiArtify", which has its advantages and disadvantages, which should be considered before choosing.

Characteristics
| Tool     | Supported OS          | Supported architectures | Possibility of automation | Additional functions           |
|----------|-----------------------|-------------------------|---------------------------|--------------------------------|
| Minikube | Windows, macOS, Linux | x86_64, ARM64           | Yes                       | Monitoring, cluster management |
| kind     | Windows, macOS, Linux | x86_64                  | No                        | -                              |
| k3d      | Windows, macOS, Linux | x86_64                  | Yes                       | Monitoring, cluster management |

Advantages und disadvantages
| Tool     | Advantages                                                                                                                   | Disadvantages                                                                          |
|----------|------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| Minikube | - Easy to install and use. <br> - Has support for cluster monitoring and management.                                         | - Limited scaling capabilities.                                                        |
| kind     | - Easy to use.                                                                                                               | - There is no possibility of automation. <br> - There may be difficulty in setting up. |
| k3d      | - Quickly build and test Kubernetes clusters in Docker containers. <br> - Has support for cluster monitoring and management. | - There may be difficulty in setting up.                                               |

Demo of k3d
![Image](.data/demo.gif)
