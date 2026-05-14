---
layout: default
title: Invited Speakers
filename: invited.markdown
permalink: /invited/
---

# Keynote Talks

## Table of Contents

  - [Conrad Watt at Nanyang Technological University Singapore](#conrad-watt-at-nanyang-technological-university-singapore)
    - [Title: The Bright Future of Verification Slop](#title-the-bright-future-of-verification-slop)
    - [Biography](#biography)
  - [Nobuko Yoshida at The University of Oxford](#nobuko-yoshida-at-the-university-of-oxford)
    - [Title: Resilient Distributed Intelligent Swarms and Safeguarded AI: Programming Models and Runtime Guarantees](#title-resilient-distributed-intelligent-swarms-and-safeguarded-ai-programming-models-and-runtime-guarantees)
    - [Keywords](#keywords)
    - [Biography](#biography-1)
  - [Cezary Kaliszyk at The University of Melbourne](#cezary-kaliszyk-at-the-university-of-melbourne)
    - [Title: Autoformalization Across Proof Assistants: Languages, Proof Styles, and Automation](#title-autoformalization-across-proof-assistants-languages-proof-styles-and-automation)
    - [Biography](#biography-2)

## [Conrad Watt](https://conrad-watt.github.io) at [Nanyang Technological University Singapore](https://www.ntu.edu.sg)

<a href="https://conrad-watt.github.io" target="_blank">
<img src="https://raw.githubusercontent.com/AIPV2026/aipv2026.github.io/main/assets/images/conrad_watt.jpg" style="height:170px; float:left; margin-right:15px;">
</a>

### Title: The Bright Future of Verification Slop

Computer science researchers have traditionally viewed formal verification as an artisanal pursuit, but recent advances in automation and AI agent capabilities raise the tantalising possibility that large-scale, low-effort verification projects may become commonplace. Such push-button verification is anticipated in some circles as a potential solution for the untrustworthiness of AI-generated code.

I argue that the credibility of past verification projects has come, in greater part than we like to admit, from the presumption that some scholarly humans considered the properties under verification important enough to dedicate significant effort to their proof. In a world where proof is cheap, I believe that the credibility of the average formal verification claim will therefore be significantly weakened. Analogous concerns have been raised in other disciplines where handcrafted contributions, presumed to be worthy of some attention, are becoming systematically displaced by AI-generated "slop".

Thankfully, the mathematical certainty of the properties we prove and the outcome-focussed nature of our verification efforts put us in a better position than most to benefit from this new paradigm of cheap-to-produce, expensive-to-consume material. Drawing from my experiences in trying to get members of WebAssembly's industrial standards community excited about formal verification, I reflect on where our field might end up in the next few years if we find ourselves enjoying an embarrassment of riches.

### Biography
Conrad Watt is an Assistant Professor at Nanyang Technological University, Singapore, working in formal methods and programming languages. He has made substantial contributions to theorem proving and mechanised verification, including formalising the WebAssembly specification, identifying specification issues, and developing verified interpreters and tooling adopted by the community. As Chair of the W3C WebAssembly Community Group, he has played a central role in the evolution and standardisation of WebAssembly and in the design of SpecTec, a domain-specific language and toolchain for WebAssembly specification. His work connects interactive proof, language design, and practical verification for real-world systems.

## [Nobuko Yoshida](https://www.cs.ox.ac.uk/people/nobuko.yoshida/) at [The University of Oxford](https://www.ox.ac.uk/)

<a href="https://www.cs.ox.ac.uk/people/nobuko.yoshida/" target="_blank">
<img src="https://raw.githubusercontent.com/AIPV2026/aipv2026.github.io/main/assets/images/nobuko_yoshida.png" style="height:170px; float:left; margin-right:15px;">
</a>

### Title: Resilient Distributed Intelligent Swarms and Safeguarded AI: Programming Models and Runtime Guarantees

This talk presents a framework for resilient distributed intelligent swarms built on safeguarded AI principles, focusing on the development of decentralised algorithms and protocols to support distributed swarm programming models at runtime. The approach targets large-scale, adaptive multi-agent systems operating under dynamic, uncertain, and adversarial conditions, where robustness, safety, and coordination are critical.

At the core of the framework is the use of multiparty session types (MPST) to formally specify and enforce correct communication patterns among distributed agents. MPST provide a rigorous foundation for ensuring protocol fidelity, deadlock-freedom, and liveness across heterogeneous swarm components. These guarantees enable type-safe, verifiable orchestration of decentralised interactions without reliance on centralised control.

The work advances decentralised algorithms and communication protocols that support adaptive coordination, fault tolerance, and self-healing behaviours. These include mechanisms for dynamic consensus under partial failure, and efficient message passing in resource-constrained environments. 

Safeguarded AI is embedded through formal verification, runtime assurance, and explainability mechanisms, addressing challenges such as adversarial interference, data integrity, and trust. The integration of distributed learning approaches—such as cooperative and federated learning—allows agents to evolve collectively while maintaining privacy and robustness.

### Keywords

multiparty session types (MPST), decentralised systems, distributed swarm programming, runtime verification, distributed algorithms, communication protocols, fault tolerance, self-healing systems, safeguarded AI, formal methods, cyber-physical systems, resilient swarms.

### Biography
Nobuko Yoshida is Christopher Strachey Chair of Computing at the University of Oxford. Her research focuses on programming languages, concurrency theory, and formal verification. She is known for her work on session types, behavioural types, and type systems for communication-based
software, contributing to the foundations of safe and structured interaction in distributed systems.

Her work combines semantic theory with system design, supporting the development of formally specified communication protocols for distributed and cyber-physical systems. She has led international research projects and collaborated with industry and interdisciplinary partners.

She is a recipient of Horizon TaRDIS project which develops programming language tools for distributed intelligent swarms, decentralised AI agents and the next generation of IoT systems, and ARIA funding for a project on safe-guarded AI, which investigates mathematically grounded methods for reliability and accountability in advanced AI systems. Her research connects type theory, concurrency, verification, and the design of trustworthy software systems.

## [Cezary Kaliszyk](https://ckaliszyk.github.io) at [The University of Melbourne](https://www.unimelb.edu.au)

### Title: Autoformalization Across Proof Assistants: Languages, Proof Styles, and Automation

Abstract: This talk compares several lines of LLM-assisted
autoformalization across Megalodon, Isabelle/HOL, and Mizar, spanning
different mathematical domains and proof-assistant cultures. The
Megalodon work studies decentralized proof development with multiple
LLM-based coding agents, using a simulated bounty marketplace in which
agents propose lemmas, assign proof obligations, invoke tactics,
inspect proof states, and compete to complete verified formal
developments. The Isabelle/HOL work emphasizes large-scale textbook
formalization using a sorry-first workflow and extensive automation,
while the Mizar work highlights declarative proof style, library
alignment, and the formalization of surreal numbers. Taken together,
these projects show that autoformalization is not a single uniform
task, but a family of workflows shaped by formal language, proof
style, automation, library structure, and the ways in which LLM agents
interact with proof assistants.

### Biography

Prof. Cezary Kaliszyk is a Professor in Theoretical Computer Science at The University of Melbourne, whose research focuses on automated reasoning, interactive theorem proving, and AI-assisted formal mathematics. Before joining Melbourne, he held positions at University of Innsbruck and contributed extensively to the European automated reasoning and formal methods communities. He is one of the long-standing organizers and driving forces behind the Conference on Artificial Intelligence and Theorem Proving (AITP) series, which has become a major venue connecting theorem proving, machine learning, and formalized mathematics research. His work on machine learning for theorem proving, premise selection, hammer systems, and large-scale formal mathematics has been supported through prominent international research collaborations and competitive funding programs, including projects connected to the European research ecosystem. He is widely recognized for helping bridge interactive and automated theorem proving across systems such as Isabelle, HOL4, Coq, and Mizar, and for advancing the practical use of AI techniques in formal verification and mathematical reasoning.

<img id="randomImage" src="" alt="Random Image">
