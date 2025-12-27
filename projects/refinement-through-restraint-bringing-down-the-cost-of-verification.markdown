---
layout: default
title: "Refinement through Restraint: Bringing Down the Cost of Verification"
filename: refinement-through-restraint-bringing-down-the-cost-of-verification.markdown
permalink: /projects/refinement-through-restraint-bringing-down-the-cost-of-verification/
---

# Refinement through Restraint: Bringing Down the Cost of Verification

- Venue: ACM SIGPLAN International Conference on Functional Programming (**ICFP 2016**)
- Location: Nara, Japan
- Authors: Liam O'Connor, Zilin Chen, Christine Rizkallah, Sidney Amani, Japheth Lim, Toby Murray, **Yutaka Nagashima**, Thomas Sewell, and Gerwin Klein
- Formal proceeding: [https://doi.org/10.1145/3022670.2951940](https://doi.org/10.1145/3022670.2951940)

### Abstract
We present a framework aimed at significantly reducing the cost of verifying certain classes of systems software, such as file systems. 
Our framework allows for equational reasoning about systems code written in our new language, **Cogent**. **Cogent** is a restricted, polymorphic, higher-order, and purely functional language with **linear types** and without the need for a trusted runtime or garbage collector. Linear types allow us to assign **two semantics** to the language: one imperative, suitable for efficient C code generation; and one functional, suitable for equational reasoning and verification. As Cogent is a restricted language, it is designed to easily interoperate with existing C functions and to connect to existing C verification frameworks.

Our framework is based on certifying compilation: For a well-typed **Cogent** program, our compiler produces C code, a high-level shallow embedding of its semantics in Isabelle/HOL, and a proof that the C code correctly refines this embedding. Thus one can reason about the full semantics of real-world systems code productively and equationally, while retaining the interoperability and leanness of C. The compiler certificate is a series of language-level proofs and per-program translation validation phases, combined into one coherent top-level theorem in Isabelle/HOL.

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
    class Refinement highlighted;

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

### Video (English)

<div class="video-container">
<iframe width="560" height="315" src="https://youtube.com/embed/sJwcm_worfM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

### Mindmap
[![Mindmap for Refinement at ICFP2016](/assets/images/mindmaps/2016_Refinement_ICFP.svg)](https://drive.google.com/file/d/1n2dJzS9edA2Js1Qpp_YQiTjNuscaJe4R/view?usp=sharing)
