---
layout: page
title: Research
permalink: /research/
---

## Feasibility and Challenges of Automatic Software Building

<p align="justify" style="max-width:800px">

Despite the advancement in software build tools such as Maven and Gradle, human involvement is still often required in software building. To engage in large-scale advanced program analysis and data mining of software artifacts, software engineering researchers need to have a large corpus of built
software, so automatic software building becomes essential to improve research productivity. We present the first feasibility study on automatic software building. Particularly, we first put state-of-the-art build automation tools (Ant, Maven and Gradle) to the test by automatically executing their respective default build commands on top 200 Java projects from GitHub. Next, we focused on the 86 projects that failed this initial automated build attempt, manually examining and determining correct build sequences to build each of these projects. We present a detailed build failure taxonomy from these build results
and show that at least 57% build failures can be automatically resolved.</p>


## HireBuild

<p align="justify" style="max-width:800px">
Advancements in software build tools such as Maven reduce build management effort, but developers still need specialized knowledge and long time to maintain build scripts and resolve build failures. More recent build tools such as Gradle give developers greater extent of customization flexibility, but can be even more difficult to maintain. According to the TravisTorrent dataset of open-source software continuous integration, 22% of code commits include changes in
build script files to maintain build scripts or to resolve build failures. Automated program repair techniques have great potential to reduce cost of resolving software failures, but the existing techniques mostly focus on repairing source code so that they cannot directly help resolving software build failures. To address this limitation, we propose HireBuild: History-Driven Repair of Build Scripts, the first approach to automatic patch generation for build scripts, using
fix patterns automatically generated from existing build script fixes and recommending fix patterns based on build log similarity. From TravisTorrent dataset, we extracted 175 build failures and their corresponding fixes which revise Gradle build scripts. Among these 175 build failures, we used the 135 earlier build fixes for automatic fix-pattern generation and the more recent 40 build failures (fixes) for evaluation of our approach. Our experiment shows that our approach
can fix 11 of 24 reproducible build failures, or 45% of the reproducible build failures, within comparable time of manual fixes.</p>


## Build Prediction Model

<p align="justify" style="max-width:800px">
Continuous Integration(CI) is a widely used development practice where developers integrate their work after submitting code changes at central repository. CI servers usually monitor central repository for code change submission and automatically build software with changed code, perform unit testing, integration testing and provide test summary report. If build or test fails developers fix those issues and submit the code changes. Continuous submission of code modification by developers and build latency time creates stalls at CI server build pipeline and hence developers have to wait long time to get build outcome. We proposed build prediction model that uses TravisTorrent data set with build error log clustering and AST level code change modification data to predict whether a build will be successful or not without attempting actual build so that developer can get early build outcome result. With the proposed model we can predict build outcome with an average F-Measure over 87% on all three build systems (Ant, Maven, Gradle) under the cross-project prediction scenario.</p>