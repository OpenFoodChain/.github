JuicyChain Installation and Onboarding

Welcome!

So you want to install our product but don’t know where to start, worry not, this is why we have this document, to guide you through the setup of our node. 

Prerequisites

First of all, can you run it? Well the prerequisites are not that demanding, let’s hope so.
Hardware requirements


JuicyChain nodes run on Ubuntu-based Linux machines. This guide assumes you will use Ubuntu 18.04 LTS or Ubuntu 20.04 LTS on a new, clean, virtual machine which is only used for your node.

Note: This document was not written as a comprehensive guide to run production-grade servers. It does not cover Linux security and privacy best practices in depth. Knowledge on subjects relating to how to run production grade servers are assumed on the reader's part.
Hardware requirements
The minimum hardware and network requirements for running a staging JuicyChain node are:
2 vCPUs 
30GB of storage
4GB memory
Data centre-level internet connectivity

The recommended hardware and network requirements for production-grade JuicyChain nodes are:
4 vCPUs 
60GB of storage
8GB memory
Data centre-level internet connectivity

Network requirements
JuicyChain exposes two APIs to interact with. Please allow incoming traffic to the machines for:

TCP port 8999 incoming - juicychain API
TCP port 8777 incoming - juicychain import API

JuicyChain also uses peer-to-peer traffic that starts as outgoing traffic. If outgoing traffic needs to be restricted, please allow for the following outgoing ports:

For STAGING:

TCP port 31677 outgoing - p2p batch data
TCP port 44260 outgoing - p2p address data

For PRODUCTION:

TCP port 16510 outgoing - p2p batch data
TCP port 49870 outgoing - p2p address data


Software requirements

The only software requirement is that you have docker on your machine, if not there is a guide at the end of this document. Or just google it.


Let’s start!
