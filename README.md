# Google-Cloud-VM-and-Networks-VPC-Features

# Key Features of Virtual Private Cloud (VPC)

![image](https://github.com/iahalkhatib/Google-Cloud-VM-and-Networks-VPC-Features/assets/170050432/e9f12a82-fc88-4f5a-bf3b-35a428a62556)

# Routing Tables

Built-in Routing Tables:

VPCs have built-in routing tables that automatically manage the forwarding of traffic.

They facilitate traffic movement within the same network, across subnetworks, or between different Google Cloud zones.

No need for external IP addresses for internal traffic.


![image](https://github.com/iahalkhatib/Google-Cloud-VM-and-Networks-VPC-Features/assets/170050432/95e2ac91-8a3f-450a-87e6-166359f6e8c0)

# Firewalls

Global Distributed Firewall:

VPCs include a global distributed firewall that controls both incoming and outgoing traffic.

Firewall rules can be easily defined using network tags on Compute Engine instances.

Network Tags:

Tags help manage firewall rules. For instance, tagging all web servers with "WEB" allows setting rules for ports 80 and 443, enabling consistent access management.


![image](https://github.com/iahalkhatib/Google-Cloud-VM-and-Networks-VPC-Features/assets/170050432/e956f180-2d24-469c-aa18-a621affd20d3)

# VPC Peering and Shared VPC

VPC Peering:

Establishes a relationship between two VPCs to allow traffic exchange.

Ideal for connecting VPCs within the same or different Google Cloud projects without exposing external IPs.

Shared VPC:

Allows multiple Google Cloud projects to share a common VPC.

Leverages Identity Access Management (IAM) for fine-grained control over who and what can interact with the VPC across projects.

# Key Terminology

Routing Tables: Tables that determine the path for forwarding traffic within the network.

Firewall Rules: Policies that control the flow of network traffic to and from VMs.

Network Tags: Labels assigned to instances for the purpose of applying firewall rules.

VPC Peering: A networking connection between two VPCs that allows traffic exchange.

Shared VPC: A VPC that is shared across multiple Google Cloud projects, using IAM for access control.

# What is a primary benefit of using network tags with VPC firewall rules?

A) Simplified billing
B) Easier management of access control
C) Increased network speed
D) Automatic load balancing

Correct Answer: B) Easier management of access control
Explanation: Network tags simplify the management of access control by allowing firewall rules to be applied consistently to all instances with the same tag.

# Which feature allows VPCs from different Google Cloud projects to communicate without using external IP addresses?

A) Shared VPC
B) VPC Peering
C) Network Tags
D) IAM Roles

Correct Answer: B) VPC Peering
Explanation: VPC Peering enables traffic exchange between VPCs from different projects without the need for external IP addresses.

# How does a Shared VPC benefit organizations with multiple Google Cloud projects?

A) It reduces network latency.
B) It centralizes network management and security.
C) It provides automatic cost allocation.
D) It simplifies the deployment of instances.
Correct Answer: B) It centralizes network management and security.
Explanation: Shared VPC centralizes network management and security by allowing multiple projects to share a common VPC and using IAM for access control.
