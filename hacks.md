---
layout: page
title: Hacks Proposals
---
{::options toc_levels="2,3" /}

* TOC
{:toc}

Project pitch slides: [https://drive.google.com/drive/folders/1-aUlcAtG3GlISRlzAnMaRMETX1fX7lth7LSI24WF-blX3IInQhWxp2t3ADt6bXPKktkSJm1Q?usp=sharing](https://drive.google.com/file/d/14RVLTJHmKixIMHD65FjlzsExqbjSnyHT/view?usp=sharing)



## 1. Excalidraw on Ownly

**Project Lead:**
- Xinyu Ma

**Preferred Team Size:**
- two

**Targeted Participants:**
- Someone new to NDN development

**Goal of the Project:**
- Add Excalidraw to ownly workspace. Allow shared figure drawing.

**Tasks of the Project:**
- Use iframe to hold a Excalidraw editor and communicate via broadcast channel.

**Specific Languages or Tools:**
- N/A




## 2. Select routers and profiles on Ownly

**Project Lead:**
- Xinyu Ma

**Preferred Team Size:**
- two

**Targeted Participants:**
- Someone with NDN code development experience

**Goal of the Project:**
- Allow users to connect to a different NDN node than SUNS, and have multiple profiles.

**Tasks of the Project:**
- Add corresponding Go API. Add frontend pages. Modify backend code to accept user configs

**Specific Languages or Tools:**
- Go




## 3. Git over Ownly

**Project Lead:**
- Xinyu Ma

**Preferred Team Size:**
- three

**Targeted Participants:**
- Someone with NDN code development experience

**Goal of the Project:**
- Verify the design of running git over Ownly. Provide a detailed design or prototype code.

**Tasks of the Project:**
- Brainstorm and verify the design. Implement a quick prototype if time allows.

**Specific Languages or Tools:**
- Git.




## 4. ScapyNDN

**Project Lead:**
- Ashlesh Gawande

**Preferred Team Size:**
- five

**Targeted Participants:**
- Someone with NDN code development experience

**Goal of the Project:**
- A feature-rich scapyndn library as polished/usable as possible

**Tasks of the Project:**
- Tasks
- Add documentation for current code [Covers all NDNv0.3 packets +
some tools similar to nfdc/ndndump]
     - Make public the existing code!
- Add (missing) NFD management spec
- Add NLSR packet/management spec + nlsrc like tool
- Add NDNCERT packet spec + a tool
- Add KeyChain - maybe look into using python-ndn’s
     - Basic KeyChain is there to sign using default key
     - Already uses python-ndn’s Face for send/rcv
- Polish, add more unit tests where necessary, test on Windows

**Specific Languages or Tools:**
- python, scapy, reading




## 5. File Server & WebTransport in NDNd

**Project Lead:**
- Junxiao Shi

**Preferred Team Size:**
- two

**Targeted Participants:**
- Someone with NDN code development experience

**Goal of the Project:**
- Submit file server and WebTransport implementations as Pull Requests to NDNd repository.

**Tasks of the Project:**
- 1. Implement ndn6-file-server protocol in NDNd codebase.
2. Implement WebTransport as a listener/face type in YaNFD.

**Specific Languages or Tools:**
- Go programming language, quic-go library




## 6. Migrating to CMake (and Conan)

**Project Lead:**
- Davide Pesavento

**Preferred Team Size:**
- two

**Targeted Participants:**
- Someone new to NDN development

**Goal of the Project:**
- Move to a more standard approach for building C++-based NDN software. Simplify dependency management. Make it easier to use NDN libraries (mainly ndn-cxx) in other projects.

**Tasks of the Project:**
- Convert at least two C++ projects to CMake.
Alternatively, convert one project + add dependency management to it via Conan.

**Specific Languages or Tools:**
- None




## 7. Standalone C++ Module for Interest-Based NDN Repo Insertion

**Project Lead:**
- Suravi Regmi

**Preferred Team Size:**
- two

**Targeted Participants:**
- Someone new to NDN development

**Goal of the Project:**
- This project addresses a limitation in earlier mGuard where data was inserted into the repo using bulk insert instead of Interest-based insertion. To support proper NDN workflows, a C++ version of the publisher API from ndn-python-repo was implemented inside mGuard.

The goal of this project is to decouple that logic from mGuard and turn it into a standalone, reusable C++ module that provides the same basic API as the Python-based publisher. The project involves extracting the existing logic, defining a clean C++ interface, and packaging it as a general-purpose component that can be used independently of mGuard or Python tooling.

**Tasks of the Project:**
- Extract publisher logic from mGuard and remove mGuard-specific dependencies.
Refactor and organize the code into a standalone module.
Add build support (e.g., with a CMake file or other setup).
Write minimal documentation for usage and integration.

**Specific Languages or Tools:**
- C++


## 8. NDNd Improvements

**Project Lead:**
- Varun

**Preferred Team Size:**
- two

**Targeted Participants:**
- Someone new to NDN development

**Goal of the Project:**
- 1. (re-)Implement ethernet face for NDNd
2. Implement FCH in NDNd

**Tasks of the Project:**
- https://github.com/named-data/ndnd/issues/70
https://github.com/named-data/ndnd/issues/117

**Specific Languages or Tools:**
- Golang


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
