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