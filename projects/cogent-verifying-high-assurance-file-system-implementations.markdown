---
layout: default
title: "Cogent: Verifying High-Assurance File System Implementations"
filename: cogent-verifying-high-assurance-file-system-implementations.markdown
permalink: /projects/cogent-verifying-high-assurance-file-system-implementations/
---

# Cogent: Verifying High-Assurance File System Implementations

- Venue: ACM International Conference on Architectural Support for Programming Languages and Operating Systems (**ASPLOS 2016**)
- Location: Atlanta, USA
- Authors: Sidney Amani, Alex Hixon, Zilin Chen, Christine Rizkallah, Peter Chubb, Liam O'Connor, Joel Beeren, **Yutaka Nagashima**, Japheth Lim, Thomas Sewell, Joseph Tuong, Gabriele Keller, Toby Murray, Gerwin Klein, and Gernot Heiser
- Formal proceeding: [https://doi.org/10.1145/2954679.2872404](https://doi.org/10.1145/2954679.2872404)

### Abstract

We present an approach to writing and formally verifying high-assurance file-system code in a restricted language called Cogent, supported by a certifying compiler that produces C code, high-level specification of **Cogent**, and translation correctness proofs. 
The language is strongly typed and guarantees absence of a number of common file system implementation errors. We show how verification effort is drastically reduced for proving higher-level properties of the file system implementation by reasoning about the generated formal specification rather than its low-level C code. 
We use the framework to write two Linux file systems, and compare their performance with their native C implementations.

### Project Dependency Graph

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
    class VeriFile highlighted;

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

### Mindmap
[![Mindmap for VeriFile at ASPLOS2016](/assets/images/mindmaps/2016_VeriFile_ASPLOS.svg)](https://drive.google.com/file/d/1PVLZIfMDLXJG_yAh7fYEaS_5Q6HVE0s_/view?usp=sharing)
