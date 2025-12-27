---
layout: default
title: Publication
filename: publication.markdown
permalink: /publication/
---

# Publication

This page lists the publications I have (co-)authored. 
**I provide more details of these publications on [the research pages](https://yutakang.github.io/research/)**.

## Table of Contents
1. [Dependency Graph](#dependency-graph)
2. [Main Publications](#main-publications)
3. [Other Publications and Posters](#other-publications-and-posters)

## Dependency Graph
This graph summarises the dependencies of my publications.
You can view the details of each paper by clicking on its corresponding node.

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

## Main Publications

### [Template-Based Conjecturing for Automated Induction in Isabelle/HOL](https://yutakang.github.io/projects/template-based-conjecturing-for-automated-induction-in-isabellehol)
- Venue: The 10th IPM International Conference on Fundamentals of Software Engineering (**FSEN 2023**)
- Location: Tehran, Iran
- Authors: **Yutaka Nagashima**, Zijin Xu, Ningli Wang, Daniel Sebastian Goc, and James Bang
- [https://doi.org/10.1007/978-3-031-42441-0_9](https://doi.org/10.1007/978-3-031-42441-0_9)

---

### [Genetic Algorithm for Program Synthesis](https://yutakang.github.io/projects/genetic-algorithm-for-program-synthesis)
- Venue: The 10th IPM International Conference on Fundamentals of Software Engineering (**FSEN 2023**)
- Location: Tehran, Iran
- Author: **Yutaka Nagashima**
- [https://doi.org/10.1007/978-3-031-42441-0_8](https://doi.org/10.1007/978-3-031-42441-0_8)

---

### [Definitional Quantifiers Realise Semantic Reasoning for Proof by Induction](https://yutakang.github.io/projects/definitional-quantifiers-realise-semantic-reasoning-for-proof-by-induction)
- Venue: The 16th International Conference on Tests and Proofs (**TAP 2022**)
- Location: Nantes, France
- Author: **Yutaka Nagashima**
- [https://doi.org/10.1007/978-3-031-09827-7_4](https://doi.org/10.1007/978-3-031-09827-7_4)

---

### [Faster Smarter Induction for Isabelle/HOL](https://yutakang.github.io/projects/faster-smarter-induction-for-isabellehol)
- Venue: The 30th International Joint Conference on Artificial Intelligence (**IJCAI 2021**)
- Location: Montreal-Themed Virtual Reality
- Author: **Yutaka Nagashima**
- Paper: [https://www.ijcai.org/proceedings/2021/273](https://www.ijcai.org/proceedings/2021/273)
- Video: [https://youtu.be/4umf8Zhjy7c](https://youtu.be/4umf8Zhjy7c)

<div class="video-container">

<iframe width="560" height="315" src="https://www.youtube.com/embed/4umf8Zhjy7c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</div>

---

### [Smart Induction for Isabelle/HOL (Tool Paper)](https://yutakang.github.io/projects/smart-induction-for-isabellehol-tool-paper)
- Venue: The 20th International Conference on Formal Methods in Computer-Aided Design (**FMCAD 2020**)
- Location: Online
- Author: **Yutaka Nagashima**
- Paper: [https://doi.org/10.34727/2020/isbn.978-3-85448-042-6_32](https://doi.org/10.34727/2020/isbn.978-3-85448-042-6_32)
- Video: [https://youtu.be/iaH0Mx926CU](https://youtu.be/iaH0Mx926CU)

<div class="video-container">

<iframe width="560" height="315" src="https://www.youtube.com/embed/iaH0Mx926CU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</div>

---

### [Simple Dataset for Proof Method Recommendation in Isabelle/HOL (Dataset Description)](https://yutakang.github.io/projects/simple-dataset-for-proof-method-recommendation-in-isabellehol)
- Venue: The 13th Conference on Intelligent Computer Mathematics (**CICM 2020**)
- Location: Bertinoro, Italy (online)
- Author: **Yutaka Nagashima**
- Formal proceeding: [https://doi.org/10.1007/978-3-030-53518-6_21](https://doi.org/10.1007/978-3-030-53518-6_21)
- Appendix at Zenodo: [http://doi.org/10.5281/zenodo.3839417](http://doi.org/10.5281/zenodo.3839417)
- Dataset at Zenodo: [https://doi.org/10.5281/zenodo.3819026](https://doi.org/10.5281/zenodo.3819026)

---

### [LiFtEr: Language to Encode Induction Heuristics for Isabelle/HOL](https://yutakang.github.io/projects/lifter-language-to-encode-induction-heuristics-for-isabellehol)
- Venue: The 17th Asian Symposium on Programming Languages and Systems (**APLAS 2019**)
- Location: Bali, Indonesia
- Author: **Yutaka Nagashima**
- Formal proceeding: [https://doi.org/10.1007/978-3-030-34175-6_14](https://doi.org/10.1007/978-3-030-34175-6_14)

---

### [Towards Evolutionary Theorem Proving for Isabelle/HOL (poster-only paper)](https://yutakang.github.io/projects/towards-evolutionary-theorem-proving-for-isabellehol-poster-only-paper)
- Venue: The Genetic and Evolutionary Computation Conference (**GECCO 2019**)
- Location: Prague, Czech Republic
- Author: **Yutaka Nagashima**
- Formal proceeding: [https://doi.org/10.1145/3319619.3321921](https://doi.org/10.1145/3319619.3321921)

---

### [PaMpeR: Proof Method Recommendation System for Isabelle/HOL](https://yutakang.github.io/projects/pamper-proof-method-recommendation-system-for-isabellehol)
- Venue: The 33rd IEEE/ACM International Conference on Automated Software Engineering (**ASE 2018**)
- Location: Montpellier, France
- Authors: **Yutaka Nagashima** and Yilun He
- Formal proceeding without appendices: [https://doi.org/10.1145/3238147.3238210](https://doi.org/10.1145/3238147.3238210)

<div class="video-container">
<iframe width="560" height="315" src="https://youtube.com/embed/BEtf8zzAlsU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<div class="video-container">
<iframe width="560" height="315" src="https://youtube.com/embed/GBsOwaRmQ5g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
---

### [Goal-Oriented Conjecturing for Isabelle/HOL](https://yutakang.github.io/projects/goal-oriented-conjecturing-for-isabellehol)
- Venue: The 11th Conference on Intelligent Computer Mathematics (**CICM 2018**)
- Location: Hagenberg, Austria
- Authors: **Yutaka Nagashima** and Julian Parsert
- This paper won the **best system award**
- Formal proceeding: [https://doi.org/10.1007/978-3-319-96812-4_19](https://doi.org/10.1007/978-3-319-96812-4_19)

<div class="video-container">
<iframe width="560" height="315" src="https://youtube.com/embed/kUjuolPT1J0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

---

### [A Proof Strategy Language and Proof Script Generation for Isabelle/HOL](https://yutakang.github.io/projects/a-proof-strategy-language-and-proof-script-generation-for-isabellehol)
- Venue: The 26th Conference on Automated Deduction (**CADE-26 (2017)**)
- Location: Gothenburg, Sweden
- Authors: **Yutaka Nagashima** and Ramana Kumar
- Formal Proceeding: [https://doi.org/10.1007/978-3-319-63046-5_32](https://doi.org/10.1007/978-3-319-63046-5_32

<div class="video-container">
<iframe width="560" height="315" src="https://youtube.com/embed/xGQQJKTtgsE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

---

### [Refinement through Restraint: Bringing Down the Cost of Verification](https://yutakang.github.io/projects/refinement-through-restraint-bringing-down-the-cost-of-verification)
- Venue: ACM SIGPLAN International Conference on Functional Programming (**ICFP 2016**)
- Location: Nara, Japan
- Authors: Liam O'Connor, Zilin Chen, Christine Rizkallah, Sidney Amani, Japheth Lim, Toby Murray, **Yutaka Nagashima**, Thomas Sewell, and Gerwin Klein
- Formal proceeding: [https://doi.org/10.1145/3022670.2951940](https://doi.org/10.1145/3022670.2951940)

<div class="video-container">
<iframe width="560" height="315" src="https://youtube.com/embed/sJwcm_worfM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

---

### [A framework for the automatic formal verification of refinement from Cogent to C](https://yutakang.github.io/projects/a-framework-for-the-automatic-formal-verification-of-refinement-from-cogent-to-c)
- Venue: The seventh conference on Interactive Theorem Proving (**ITP 2016**)
- Location: Nancy, France
- Authors: Christine Rizkallah, Japheth Lim, **Yutaka Nagashima**, Thomas Sewell, Zilin Chen, Liam O'Connor, Toby Murray, Gabriele Keller, and Gerwin Klein
- Formal proceeding: [https://doi.org/10.1007/978-3-319-43144-4_20](https://doi.org/10.1007/978-3-319-43144-4_20)

---

### [Cogent: Verifying High-Assurance File System Implementations](https://yutakang.github.io/projects/cogent-verifying-high-assurance-file-system-implementations)
- Venue: ACM International Conference on Architectural Support for Programming Languages and Operating Systems (**ASPLOS 2016**)
- Location: Atlanta, USA
- Authors: Sidney Amani, Alex Hixon, Zilin Chen, Christine Rizkallah, Peter Chubb, Liam O'Connor, Joel Beeren, **Yutaka Nagashima**, Japheth Lim, Thomas Sewell, Joseph Tuong, Gabriele Keller, Toby Murray, Gerwin Klein, and Gernot Heiser
- Formal proceeding: [https://doi.org/10.1145/2954679.2872404](https://doi.org/10.1145/2954679.2872404)

## Other Publications and Posters

### Proof By Abduction in Isabelle/HOL
- Venue: Seventh Conference on Artificial Intelligence and Theorem Proving (**AITP2024**)
- Location: Aussois, France
- Authors: **Yutaka Nagashima**, Daniel Sebastian Goc
- Abstract: [https://aitp-conference.org/2024/abstract/AITP_2024_paper_35.pdf](https://aitp-conference.org/2024/abstract/AITP_2024_paper_35.pdf)
- Slides: [https://aitp-conference.org/2024/slides/YN.pdf](https://aitp-conference.org/2024/slides/YN.pdf)
<div class="video-container">

<iframe width="560" height="315" src="https://www.youtube.com/embed/rXU-lJxP_GI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</div>

---

### Evolutionary Computation for Program Synthesis in SuSLik
- Venue: Seventh Conference on Artificial Intelligence and Theorem Proving (**AITP2022**)
- Location: Aussois, France (hybrid)
- Author: **Yutaka Nagashima**

---

### Faster Smarter Proof by Induction in Isabelle/HOL with Definitional Quantifiers
- Venue: Sixth Conference on Artificial Intelligence and Theorem Proving (**AITP2021**)
- Location: Aussois, France (hybrid)
- Author: **Yutaka Nagashima**

---

### Towards United Reasoning for Automatic Induction in Isabelle/HOL
- Venue: The 34th Annual Conference of the Japanese Society for Artificial Intelligence (**JSAI 2020**)
- Location: Kumamoto, Japan (online)
- Author: **Yutaka Nagashima**
- [https://doi.org/10.11517/pjsai.JSAI2020.0_3G1ES103](https://doi.org/10.11517/pjsai.JSAI2020.0_3G1ES103)

---

### Smart Induction for Isabelle/HOL (Tool Paper)
- Venue: Isabelle Workshop 2020 (**Isabelle2020**)
- Location: Online
- Author: **Yutaka Nagashima**

---

### LiFtEr: Language to Encode Induction Heuristics
- Venue: Fifth Conference on Artificial Intelligence and Theorem Proving (**AITP2020**)
- Location: Aussois, France (hybrid)
- Author: **Yutaka Nagashima**

---

### Towards United Reasoning for Automatic Induction in Isabelle/HOL
- Venue: The 17th Asian Symposium on Programming Languages and Systems Poster Track (**APLAS 2019 poster**)
- Location: Bali, Indonesia
- Author: **Yutaka Nagashima**

---

### Domain-Specific Language to Encode Induction Heuristics
- Venue: The ACM Student Research Competition co-located at the 24th International Conference on Functional Programming (**ICFP-SRC 2019**)
- Location: Berlin, Germany
- Author: **Yutaka Nagashima**
- [https://arxiv.org/abs/1907.02594](https://arxiv.org/abs/1907.02594)

---

### Towards Machine Learning Induction
- Venue: The ML family workshop co-located at the 24th International Conference on Functional Programming (**ML 2019**)
- Location: Berlin, Germany
- Author: **Yutaka Nagashima**
- [https://arxiv.org/abs/1812.04088v2](https://arxiv.org/abs/1812.04088v2)

---

### Towards Machine Learning Induction
- Venue: Fourth Conference on Artificial Intelligence and Theorem Proving (**AITP 2019**)
- Location: Obergurgl, Austria
- Author: **Yutaka Nagashima**
- [https://arxiv.org/abs/1812.04088v2](https://arxiv.org/abs/1812.04088v2)

---

### Towards Machine Learning Induction
- Venue: Third Workshop on Learning in Verification (**LiVe 2019**)
- Location: Prague, The Czech Republic
- Author: **Yutaka Nagashima**
- [https://arxiv.org/abs/1812.04088v2](https://arxiv.org/abs/1812.04088v2)

---

### PaMpeR: A Proof Method Recommendation System for Isabelle/HOL
- Venue: Isabelle Workshop 2018 (**Isabelle 2018**)
- Location: Oxford, UK
- Authors: **Yutaka Nagashima** and Yilun He
- [https://files.sketis.net/Isabelle_Workshop_2018/Isabelle_2018_paper_8.pdf](https://files.sketis.net/Isabelle_Workshop_2018/Isabelle_2018_paper_8.pdf)

---

### Designing Games of Theorem Proving
- Venue: Third Conference on Artificial Intelligence and Theorem Proving (**AITP 2018**)
- Location: Aussois, France
- Author: **Yutaka Nagashima**
- [http://aitp-conference.org/2018/aitp18-proceedings.pdf](http://aitp-conference.org/2018/aitp18-proceedings.pdf)

---

### Towards Smart Proof Search for Isabelle
- Venue: Second Conference on Artificial Intelligence and Theorem Proving (**AITP 2017**)
- Location: Obergurgl, Austria
- Author: **Yutaka Nagashima**
- [https://arxiv.org/abs/1701.03037](https://arxiv.org/abs/1701.03037)

---

### Proof Strategy Language
- Venue: Archive of Formal Proofs (**AFP 2016**)
- Author: **Yutaka Nagashima**
- [https://www.isa-afp.org/entries/Proof_Strategy_Language.html](https://www.isa-afp.org/entries/Proof_Strategy_Language.html)

---

### Close Encounters of the Higher Kind - Emulating Constructor Classes in Standard ML (extended abstract)
- Venue: ACM SIGPLAN Workshop on ML (**ML 2016**)
- Location: Nara, Japan
- Authors: **Yutaka Nagashima** and Liam O'Connor
- The abstract is available at arXiv: [https://arxiv.org/abs/1608.03350](https://arxiv.org/abs/1608.03350)
- The presentation is available at YouTube: [https://www.youtube.com/watch?v=A2BJ6HRPRyg](https://www.youtube.com/watch?v=A2BJ6HRPRyg)

---

### Keep Failed Proof Attempts in Memory
- Venue: Isabelle Workshop 2016 (**Isabelle 2016**)
- Location: Nancy, France
- Author: **Yutaka Nagashima**
