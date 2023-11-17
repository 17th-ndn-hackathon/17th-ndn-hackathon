---
layout: page
title: Hacks Proposals
---
{::options toc_levels="2,3" /}

* TOC
{:toc}


## 1.NDNts documentation and tutorial


**Project Lead:**
- Xinyu Ma

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People new to NDN

**How does your proposal benefit NDN?**
- Make NDNts easier to use

**Briefly describe the tasks**
- Document functions in a more detailed way
- Write examples for frequently used classes
- Write tutorials for basic applications

**Any specific tools or language**
- TypeScript, TSDoc

**Expected outcomes**
- More detailed documentation at https://ndnts-docs.ndn.today/

## 2. Improving NDN Workspace Application with OpenIDConnect


**Project Lead:**
- Tianyuan Yu

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with previous NDN experience

**How does your proposal benefit NDN?**
- The NDN Workspace users currently obtain their application certificates via proving they own a NDN Testbed certificate. Since NDN Workspace is a web application, a more intuitive approach is to utilize users' existing web identities to authenticate users. OpenIDConnect is a good fit in this case.

**Briefly describe the tasks**
- Implement the following process: the user asks for their web identity provider for authentication, obtain the token (or equivalent) from the provider, sends it to Workspace CA/server, then the CA/server validates the token, assigns name, and issue certificate.

**Any specific tools or language**
- TypeScript, Python

**Expected outcomes**
- A Github PR


## 3. OpenAPI Equivalent over NDN


**Project Lead:**
- Xinyu Ma

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with previous NDN experience

**How does your proposal benefit NDN?**
- Provide general API for application use.

**Briefly describe the tasks**
- Explore the possibilities of implementing OpenAPI equivalent over NDN. It consists of two parts: the serialization with protobuf or JSON (with schema), and the RPC with SVS or modified RICE.

**Any specific tools or language**
- TypeScript, Python

**Expected outcomes**
- Prototype of OpenAPI over NDN and future development plan.



## 4. NDN Workspace Development


**Project Lead:**
- Xinyu Ma

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with previous NDN experience

**How does your proposal benefit NDN?**
- Further development of a (basically) usable NDN web app.

**Briefly describe the tasks**
- Discuss and solve on GitHub issues of the NDN workspace app.

**Any specific tools or language**
- NDNts and SolidJS

**Expected outcomes**
- Discussions and PRs on GitHub


## 5. Testbed-in-a-box


**Project Lead:**
- Varun Patil

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with previous NDN experience

**How does your proposal benefit NDN?**
- Make it easy to run an NDN network

**Briefly describe the tasks**
- Containerize NDN components and make it easily configurable

**Any specific tools or language**
- Docker, python3 or another scripting language

**Expected outcomes**
- An NDN testbed, in a box


## 6. Define NDN Services in Extensible Markup Language


**Project Lead:**
- Tianxing Ma

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with previous NDN experience

**How does your proposal benefit NDN?**
- A quick solution to bulld NDN services

**Briefly describe the tasks**
- Explore the possibility to define NDN service interfaces (input, output, and their data structures) in a standard format(xml), and explore the possibility to create a code generator to generate runnable code from these definitions. Also, think about its security. To begin with, the input and out would be defined as MAVlink messages in a xml file.

**Any specific tools or language**
- C++, NDNCXX, MAVlink, XML, NAC-ABE

**Expected outcomes**
- Some experience, maybe a standard to define the services


## 7. Containerize all the things!


**Project Lead:**
- Davide Pesavento

<!-- Project Members: TBD -->
**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with previous NDN experience

**How does your proposal benefit NDN?**
- Make the NDN stack easier to run on your machine and/or to deploy on a network of nodes.

**Briefly describe the tasks**
- Write a Dockerfile for NFD. Write a Dockerfile for a sample application (e.g., ndnpingserver). Write GitHub Actions workflows to build and publish the container images. Make sure other NDN applications can transparently use a containerized NFD. Write a sample docker-compose.yml that showcases how to integrate NFD with other services/applications.

**Any specific tools or language**
- docker, docker-compose, github actions

**Expected outcomes**
- A set of Dockerfiles and CI pipelines to automatically build and publish container images of the core NDN software.