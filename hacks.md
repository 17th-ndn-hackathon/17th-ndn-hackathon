---
layout: page
title: Hacks Proposals
---
{::options toc_levels="2,3" /}

* TOC
{:toc}


## 1. Integration of mmWave with NDN/CCN using NS3 apps

**Project Lead:**
- Kundan Kanti Saha

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- mmWave is one of the technologies anticipated with 6G. It extends the current bandwidth utilisation of EM spectrum for network communication.
- By integrating ICN with mmWave, two of the most anticipated developments of 6G can be combined to meet the changing demands of internet usage.

**Briefly describe the tasks**
- The tasks for the project are based on ndnSIM and NYUSIM apps of NS3 simulation tools.
- The participants will have to combine ndnSIM and NYUSIM to create a hybrid app which can test any protocol/scheme based on ndnSIM to analyse its feasibility in 6G spectrum.

**Any specific tools or language**
- ndnSIM & NYUSIM (NS3 based apps)

**Expected outcomes**
- Test the outcome of simulating any existing/new protocol or scheme in the hybrid app developed by combining NYUSIM and ndnSIM in NS3.

## 2. Chat on NDN Workspace

**Project Lead:**
- Xinyu Ma

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People new to NDN development

**How does your proposal benefit NDN?**
- Enable people using NDN Workspace to replace slack.

**Briefly describe the tasks**
- Implement chat functionalities in NDN workspace. Need a data model and mostly the front end.

**Any specific tools or language**
- TypeScript

**Expected outcomes**
- A Chat page in NDN Workspace.

## 3. Workspace VSCode Plugin

**Project Lead:**
- Xinyu Ma

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- Improve the usability of the NDN Workspace.

**Briefly describe the tasks**
- A VSCode plugin connecting to NDN Workspace, allowing editing files in the Workspace directly.
- Need to implement the FileSystemProvider interface to let VSCode read Workspace files, and also watch VSCode document's TextDocumentChangeEvent to publish local editor changes to the Workspace in real time.
- We can start from hard coded connection. There are some code snippets to copy from.

**Any specific tools or language**
- TypeScript

**Expected outcomes**
- A prototype of VSCode plugin connecting to NDN Workspace.

## 4. Web of Trust Model for NDN Workspace

**Project Lead:**
- Yekta Kocaoğullar

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- This project is a continuation to ongoing efforts of adding functionalities to NDN Workspace, aiming to convert the current trust model of the application to Web of Trust.

**Briefly describe the tasks**
- Fetch stranger certificate by keylocator
- Request POR certificate issued by every other known (authenticated) user
  - If my cert store has N other users, send N interests for each
  - If not getting at least one POR, request an ID Token Data
  - If ID Token Data not valid or non exist, abort as data verification failure
- Cross-sign stranger public key as POR certificate
- Putting POR certificate into cert store
- Notify the POR subject a new POR is generated, let it fetch by name
- POR subject serves all POR it received"

**Any specific tools or language**
- NDNts library, TypeScript

**Expected outcomes**
- The NDN Workspace application should now use cross signed certificates for inter-trust zone communications.

## 5. Dockerizing NDN

**Project Lead:**
- Nidhi Panchal

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- Dockerization makes it easy to run NDN services, without needing to spend time installing dependencies etc.

**Briefly describe the tasks**
- Learn Docker if no relevant experience
- Create Dockerfile for each service
- Create Docker compose that will start up sample service (i.e. NLSR + NFD)
- Create image for build

**Any specific tools or language**
- Docker

**Expected outcomes**
- Starting up new NDN services will be efficient and easy. Modification for the environment is also made simpler, since only a few lines in the Dockerfiles need to be updated.

## 6. SDN + NDN with mini-NDN

**Project Lead:**
- Ziyang Xing

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- Expanding the application scope of NDN is beneficial for achieving more functions

**Briefly describe the tasks**
- Expanding the application scope of NDN is beneficial for utilizing the controllers in SDN to operate NDN

**Any specific tools or language**
- python, shell, java

**Expected outcomes**
- In the SDN environment, achieving producer to consumer distribution of content,

## 7. NDN Traffic Trace: stateful analysis & replay

**Project Lead:**
- Junxiao Shi

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- gain insights into NDN network usage; more faithfully replay traffic, making the trace useful

**Briefly describe the tasks**
- Write a program to perform Interest-Data matching from the packet traces and glean RTT information.
- Enhance the NDN Trace Replay tool - support all Interest/Data fields available in the .ndjson trace.

**Any specific tools or language**
- NDNgo/python-ndn; ndn-cxx + ndnSIM

**Expected outcomes**
- RTT report from traffic traces; enhanced NDN Trace Replay tool

## 8. Beastify NFD

**Project Lead:**
- Junxiao Shi

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- cleanup NFD codebase

**Briefly describe the tasks**
- NFD Feature #5207 autoconfig: allow NDN-FCH service over HTTPS
- NFD Task #4972 migrate WebSocket face to Boost.Beast

**Any specific tools or language**
- C++ & Boost.Beast

**Expected outcomes**
- changes submitted to Gerrit

## 9. Dynamic Rule Inference for Automating NDN Certificate Chain Validation

**Project Lead:**
- Adriana Viriato Ribeiro

**Prefered Team Size:**
- 2-4

**Targeted participant**
- People with NDN code development experience

**How does your proposal benefit NDN?**
- Facilitates NDN's remote secure bootstrapping, by automating the trust schema validation rules generation through dynamic rule inference.

**Briefly describe the tasks**
- Integrate certificate issuing and chain with the trust schema, in order to synchronize both tasks to avoid errors.
- Also, optimize trust schema validation rules to allow fast certificate chain verification.

**Any specific tools or language**
- The participants are encouraged to use C++, ndn-cxx and NDNCERT to assemble their solutions.

**Expected outcomes**
- Provide an easy to use tool that integrates certificate generation and signing with the trust schema
- Optimize remote secure bootstrapping performance
- Design a tool or set of tools that mitigate human errors in the trust schema design, so that it conforms to the current NDN certificate chain.

<!--
## 1.

**Project Lead:**
-

**Prefered Team Size:**
- 2-4

**Targeted participant**
-

**How does your proposal benefit NDN?**
-

**Briefly describe the tasks**
-

**Any specific tools or language**
-

**Expected outcomes**
- -->
