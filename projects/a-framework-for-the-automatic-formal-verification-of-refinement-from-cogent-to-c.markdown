---
layout: default
title: "A framework for the automatic formal verification of refinement from Cogent to C"
filename: a-framework-for-the-automatic-formal-verification-of-refinement-from-cogent-to-c.markdown
permalink: /projects/a-framework-for-the-automatic-formal-verification-of-refinement-from-cogent-to-c/
---

# A Framework for the Automatic Formal Verification of Refinement from COGENT to C

- Venue: The seventh conference on Interactive Theorem Proving (**ITP 2016**)
- Location: Nancy, France
- Authors: Christine Rizkallah, Japheth Lim, **Yutaka Nagashima**, Thomas Sewell, Zilin Chen, Liam O'Connor, Toby Murray, Gabriele Keller, and Gerwin Klein
- Formal proceeding: [https://doi.org/10.1007/978-3-319-43144-4_20](https://doi.org/10.1007/978-3-319-43144-4_20)

### Abstract

Our language **COGENT** simplifies verification of systems software using a certifying compiler, which produces a proof that the generated C code is a refinement of the original **COGENT** program. 
Despite the fact that **COGENT** itself contains a number of refinement layers, the semantic gap between even the lowest level of **COGENT** semantics and the generated C code remains large.

In this paper we close this gap with an automated refinement framework which validates the compiler’s code generation phase. 
This framework makes use of existing C verification tools and introduces a new technique to relate the type systems of **COGENT** and C.

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
    class VerifyC highlighted;

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
[![Mindmap for VerifyC at ITP2016](/assets/images/mindmaps/2016_VerifyC_ITP.svg)](https://drive.google.com/file/d/1hUmFJst6fWvg5iJE1YIKzU5thZe23CoE/view?usp=sharing)
