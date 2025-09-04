# Cloud Storage Types and Content Delivery Networks

## Overview
This lesson covers the four main types of cloud storage and introduces Content Delivery Networks (CDN).

## Four Main Types of Cloud Storage

### 1. Direct Attached Storage (Local Storage)
- **Definition**: Storage presented directly to a cloud-based server
- **Location**: Either within the host server chassis or within the same rack
- **Characteristics**: Closest physical proximity to the server

### 2. File Storage
- **Access Method**: Presented to compute nodes as a Network File System (NFS)
- **Connection**: Connected to compute nodes over standard ethernet network
- **Use Case**: Suitable for shared file access across multiple systems

### 3. Block Storage
- **Connection**: Presented to compute nodes using high-speed fiber connections
- **Provisioning**: Typically provisioned in volumes
- **Mounting**: Volumes are mounted onto compute nodes
- **Performance**: High-speed access due to fiber connections

### 4. Object Storage
- **Access Method**: Accessed via an API
- **Independence**: Doesn't require an underlying compute node
- **Capacity**: Offers infinite capacity - pay only for what you use
- **Performance**: Slowest read and write speeds compared to other storage types
- **Scalability**: Can continuously add files with usage-based pricing

## Storage Type Comparison
The four storage types differ in several key areas:
- **Access methods**: How they can be accessed
- **Capacity**: Storage limits and scalability
- **Cost**: Pricing models and cost structures
- **Data suitability**: Types of data they're best suited to store
- **Performance**: Read-write speed capabilities

## Content Delivery Network (CDN)
- **Definition**: A distributed server network that accelerates internet content delivery
- **Functionality**: Delivers temporarily stored or cached copies of website or media content
- **Location-based**: Content is delivered to users based on their geographic location
- **Purpose**: Improves content delivery speed and user experience
