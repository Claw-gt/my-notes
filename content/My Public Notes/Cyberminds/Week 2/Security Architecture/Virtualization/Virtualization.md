# Introduction

**Mainframes** * dominated data centers of past decades

> [!info] Mainframes
> Powerful computers used primarily by large organizations for critical applications, bulk data processing, and large-scale transaction processing.

The **client/server** model emerged in the 1980s and 1990s

Now, most data centers leverage **virtualization technology**

<img src="https://www.cloud4u.com/upload/medialibrary/e69/what-is-a-virtualization-techology.png">
see [[Containers]]

---

# Virtualization

- Host machines run on physical hardware
- Host machines provide services to several virtualized guest machines
- The hypervisor (software that runs on host) tricks each guest into thinking it is running on dedicated hardware

### Types of Hypervisor

*TYPE 1*: baremetal
*TYPE 2*: physical machines runs a OS on its own

<img src="https://f0.holisticinfosecforwebdevelopers.com/images/HypervisorTypesHighLevel.png">

## Virtualization Security

#### Isolation problems

- Virtual machine **isolation** is critical
- Each server must have access to only its own memory and storage
- VM attempt to break out of the guest environment (*VM escape attack*)

##### Virtualization platforms must be patched against security vulnerabilities

#### VM Sprawl
Unused and unmantained servers --> Security risk

## Virtualization Benefits

#### Ephemeral Computing
Resources allocated for a short time

---

# Desktop and application virtualization

## Virtual Desktop Infrastructure (VDI)

--> Provides network-based access to a desktop computing environment

Virtualization to a desktop

## Application Virtualization
or Application Streaming

--> Streams applications to the user's desktop