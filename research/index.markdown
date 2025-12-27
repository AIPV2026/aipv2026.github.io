---
layout: default
title: "Research"
filename: index.markdown
permalink: /research/
---

# Research

## Table of Contents
- [Objective](#objective)
- [System-Agnostic Approach for Proof Automation](#system-agnostic-approach-for-proof-automation)
- Projects
  - [Project List](#project-list)
  - [Project Dependency](#project-dependency)
  - [Research Fields](#research-fields)

## Objective

My mid-term research objective is to **achieve advanced proof automation** by leveraging techniques from various fields and applying this automation to **build trustworthy systems**. 
I pursue this goal for both theoretical and practical reasons.

On the theoretical side, theorem proving enables machines to fully capture the definitions of mathematical objects provided by users. 
This sharply contrasts with conventional machine learning techniques, which rely on inductive reasoning, leaving a degree of uncertainty in their conclusions. 
In theorem proving, however, the conclusions of mechanically proven theorems are 100% certain.

On the practical side, theorem proving is becoming the standard for reliable systems programming. 
Researchers use theorem provers to define specifications and prove that their implementations meet these specifications. 
Notable examples include the verification of the seL4 micro-kernel and the CompCert C-compiler. 
Theorem provers also play a pivotal role in formal scientific advancements, such as the mechanical proofs of famous mathematical conjectures like the Four Colour Theorem and the Kepler Conjecture.

In the long run, I envision large-scale **automation of scientific development** through automated reasoning. 
This is why I focus on expressive logics like higher-order logic, rather than less expressive ones: 
I believe expressive logics are the language of science, and my goal is to achieve robust automated reasoning within this framework. 
This would enable the automation of scientific development on a broad scale, extending beyond the specific domain of system verification in computer science.

## System-Agnostic Approach for Proof Automation

I have predominantly used Isabelle/HOL in my projects to leverage its existing toolsets, including powerful proof tactics and counterexample finders. 
However, **the concepts I develop are generally system-agnostic**.
In other words, I design techniques that are broad enough to be applied to most, if not all, modern theorem provers for expressive logics that incorporate proof tactics. 
I then implement these ideas within a specific prover, namely Isabelle/HOL. 
Consequently, I believe these techniques can be adapted for use with other tactic-based provers, such as The Coq (Rocq) Prover, Lean, and HOL (also known as HOL4), although some modifications may be required to address prover-specific nuances.

## Projects

### Project List

Here is a list of projects I am currently working on or have worked on. 
The acronyms correspond to the names used in the project dependency graph below.

- **Abduction**: [Proof By Abduction in Isabelle/HOL](https://yutakang.github.io/projects/proof-by-abduction-in-isabellehol)
- **TemplateBased**: [Template-Based Conjecturing for Automated Induction in Isabelle/HOL](https://yutakang.github.io/projects/template-based-conjecturing-for-automated-induction-in-isabellehol)
- **GeneticSyn**: [Genetic Algorithm for Program Synthesis](https://yutakang.github.io/projects/genetic-algorithm-for-program-synthesis)
- **SeLFiE**: [Definitional Quantifiers Realise Semantic Reasoning for Proof by Induction](https://yutakang.github.io/projects/definitional-quantifiers-realise-semantic-reasoning-for-proof-by-induction)
- **SmarterInduct**: [Faster Smarter Induction for Isabelle/HOL](https://yutakang.github.io/projects/faster-smarter-induction-for-isabellehol)
- **SmartInduct**: [Smart Induction for Isabelle/HOL (Tool Paper)](https://yutakang.github.io/projects/smart-induction-for-isabellehol-tool-paper)
- **SimpleDataset**: [Simple Dataset for Proof Method Recommendation in Isabelle/HOL](https://yutakang.github.io/projects/simple-dataset-for-proof-method-recommendation-in-isabellehol)
- **LiFtEr**: [LiFtEr: Language to Encode Induction Heuristics for Isabelle/HOL](https://yutakang.github.io/projects/lifter-language-to-encode-induction-heuristics-for-isabellehol)
- **TowardsEvo**: [Towards Evolutionary Theorem Proving for Isabelle/HOL](https://yutakang.github.io/projects/towards-evolutionary-theorem-proving-for-isabellehol-poster-only-paper)
- **PaMpeR**: [PaMpeR: Proof Method Recommendation System for Isabelle/HOL](https://yutakang.github.io/projects/pamper-proof-method-recommendation-system-for-isabellehol)
- **GoalOriented**: [Goal-Oriented Conjecturing for Isabelle/HOL](https://yutakang.github.io/projects/goal-oriented-conjecturing-for-isabellehol)
- **PSL**: [A Proof Strategy Language and Proof Script Generation for Isabelle/HOL](https://yutakang.github.io/projects/a-proof-strategy-language-and-proof-script-generation-for-isabellehol)
- **VerifyC**: [A framework for the automatic formal verification of refinement from Cogent to C](https://yutakang.github.io/projects/a-framework-for-the-automatic-formal-verification-of-refinement-from-cogent-to-c)
- **Refinement**: [Refinement through Restraint: Bringing Down the Cost of Verification](https://yutakang.github.io/projects/refinement-through-restraint-bringing-down-the-cost-of-verification)
- **VeriFile**: [Cogent: Verifying High-Assurance File System Implementations](https://yutakang.github.io/projects/cogent-verifying-high-assurance-file-system-implementations)

### Project Dependency

This graph summarizes the dependencies of the projects I worked on. 
You can view the details of each paper by **clicking on** the corresponding node.

<div class="mermaid" style="width: 100%; max-width: 1000px;">
flowchart LR
    VerifyC["VerifyC"]
    Refinement["Refinement"]
    VeriFile["VeriFile"]
    TowardsEvo["TowardsEvo"]
    GeneticSyn["GeneticSyn"]
    PSL["PSL"]
    GoalOriented["GoalOriented"]
    TemplateBased["TemplateBased"]
    LiFtEr["LiFtEr"]
    SeLFiE["SeLFiE"]
    SmartInduct["SmartInduct"]
    SmarterInduct["SmarterInduct"]
    PaMpeR["PaMpeR"]
    SimpleDataset["SimpleData"]
    Abduction["Abduction"]
    
    %% Style definitions
    classDef default fill:#f9f9f9,stroke:#333,stroke-width:2px;
    classDef futureWork fill:#fff,stroke:#333,stroke-width:2px,stroke-dasharray: 5 5;
    classDef highlighted fill:#ffff00,stroke:#333,stroke-width:2px;

    class Abduction futureWork;

    %% Clickable Nodes
    click Abduction "https://yutakang.github.io/projects/proof-by-abduction-in-isabellehol" "Proof By Abduction in Isabelle/HOL"
    click TemplateBased "https://yutakang.github.io/projects/template-based-conjecturing-for-automated-induction-in-isabellehol" "Template-Based Conjecturing for Automated Induction in Isabelle/HOL"
    click GeneticSyn "https://yutakang.github.io/projects/genetic-algorithm-for-program-synthesis" "Genetic Algorithm for Program Synthesis"
    click SeLFiE "https://yutakang.github.io/projects/definitional-quantifiers-realise-semantic-reasoning-for-proof-by-induction" "Definitional Quantifiers Realise Semantic Reasoning for Proof by Induction"
    click SmarterInduct "https://yutakang.github.io/projects/faster-smarter-induction-for-isabellehol" "Faster Smarter Induction for Isabelle/HOL"
    click SmartInduct "https://yutakang.github.io/projects/smart-induction-for-isabellehol-tool-paper" "Smart Induction for Isabelle/HOL (Tool Paper)"
    click SimpleDataset "https://yutakang.github.io/projects/simple-dataset-for-proof-method-recommendation-in-isabellehol" "Simple Dataset for Proof Method Recommendation in Isabelle/HOL"
    click LiFtEr "https://yutakang.github.io/projects/lifter-language-to-encode-induction-heuristics-for-isabellehol" "LiFtEr: Language to Encode Induction Heuristics for Isabelle/HOL"
    click TowardsEvo "https://yutakang.github.io/projects/towards-evolutionary-theorem-proving-for-isabellehol-poster-only-paper" "Towards Evolutionary Theorem Proving for Isabelle/HOL"
    click PaMpeR "https://yutakang.github.io/projects/pamper-proof-method-recommendation-system-for-isabellehol" "PaMpeR: Proof Method Recommendation System for Isabelle/HOL"
    click GoalOriented "https://yutakang.github.io/projects/goal-oriented-conjecturing-for-isabellehol" "Goal-Oriented Conjecturing for Isabelle/HOL"
    click PSL "https://yutakang.github.io/projects/a-proof-strategy-language-and-proof-script-generation-for-isabellehol" "A Proof Strategy Language and Proof Script Generation for Isabelle/HOL"
    click VerifyC "https://yutakang.github.io/projects/a-framework-for-the-automatic-formal-verification-of-refinement-from-cogent-to-c" "A framework for the automatic formal verification of refinement from Cogent to C"
    click Refinement "https://yutakang.github.io/projects/refinement-through-restraint-bringing-down-the-cost-of-verification" "Refinement through Restraint: Bringing Down the Cost of Verification"
    click VeriFile "https://yutakang.github.io/projects/cogent-verifying-high-assurance-file-system-implementations" "Cogent: Verifying High-Assurance File System Implementations"

    %% Define Edges
    VerifyC -->|is part of| Refinement
    Refinement --> |is used in| VeriFile
    TowardsEvo -->|is realised in| GeneticSyn
    TowardsEvo -.-> |should be used in| Abduction
    PSL -->|is used in| Abduction
    PSL -->|is used in| GoalOriented
    PSL -->|is used in| TemplateBased
    TemplateBased -->|is used in| Abduction
    LiFtEr -->|is used in| SmartInduct
    LiFtEr -->|evolves to| SeLFiE
    SeLFiE -->|is used in| SmarterInduct
    SmartInduct -->|evolves to| SmarterInduct
    SmarterInduct -->|is used in| TemplateBased
    SimpleDataset -->|is used in| PaMpeR
    PaMpeR -.-> |should be used in| Abduction
    GoalOriented -->|is used in| Abduction
    SmarterInduct -->|is used in| Abduction
    SeLFiE -->|is used in| Abduction
    PSL -->|integrates| SmarterInduct
</div>

### Research Fields

As mentioned above, I draw on expertise from various fields to achieve stronger proof automation. These fields include machine learning, programming languages, evolutionary computation, search, conjecturing, and abductive reasoning. The images below link to sub-pages that explain my projects, organized by research field (most of which are still under construction).

<div class="tile-container">
  <a href="/research/machine_learning" class="tile">
    <img src="/assets/images/logo_machine_learning.jpeg" alt="machine learning">
    <span class="tooltip">Link to the page for machine learning.</span>
  </a>

  <a href="/research/formal_methods" class="tile">
    <img src="/assets/images/logo_formal_methods.jpeg" alt="formal methods">
    <span class="tooltip">Link to the page for formal methods.</span>
  </a>
  
  <a href="/research/programming_language" class="tile">
    <img src="/assets/images/logo_programming_language.jpeg" alt="programming language">
    <span class="tooltip">Link to the page for programming language.</span>
  </a>

  <a href="/research/conjecturing" class="tile">
    <img src="/assets/images/logo_conjecturing.jpeg" alt="conjecturing">
    <span class="tooltip">Link to the page for conjecturing.</span>
  </a>
  
  <a href="/research/search" class="tile">
    <img src="/assets/images/logo_search.jpeg" alt="search">
    <span class="tooltip">Link to the page for search.</span>
  </a>
  
  <a href="/research/evolutionary_computation" class="tile">
    <img src="/assets/images/logo_evolution.jpeg" alt="evolutionary computation">
    <span class="tooltip">Link to the page for evolutionary computation.</span>
  </a>

  <a href="/research/induction" class="tile">
    <img src="/assets/images/logo_induction.jpeg" alt="induction">
    <span class="tooltip">Link to the page for induction.</span>
  </a>

  <a href="/research/abduction" class="tile">
    <img src="/assets/images/logo_abduction.jpeg" alt="abduction">
    <span class="tooltip">Link to the page for abduction.</span>
  </a>
  
</div>
