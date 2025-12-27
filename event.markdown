---
layout: default
title: Event
filename: event.markdown
permalink: /event/
---

# List of Notable Events

## AI & Reasoning Winter 2025 in Prague, Czechia

### Title: Verilog verification and semantics for interactive theorem proving and beyond

### Abstract: 

I will talk about my now long-running work on the verification of Verilog hardware designs and the semantics of Verilog. My verification work is based on interactive theorem proving (ITP), whereas my semantics work is broader and targets usages outside ITPs as well.

A while back I developed Verilog development tools for the ITP HOL4, providing users a trustworthy development flow that allows for connecting up high-level specifications to low-level technology-mapped netlists. The development flow is inspired by the CakeML development flow: it starts off with Verilog circuits modelled as functional programs, these are then translated to deeply embedded Verilog circuits using a proof-producing translator, which are in turn synthesised to technology-mapped netlists using a verified synthesis tool.

The above work made me interested in the semantics of Verilog, which the work made obvious is in need of rescue. I have set out to carry out such needed rescue operation. In particular, the fact that Verilog comes with three different semantics—its simulation semantics, its synthesis semantics, and its cycle semantics—opens up a range of problems. The formal meaning of each semantics needs to be pinned down fully and the connections between these semantics must be made clear. For example, as I have shown in a recent paper published at OOPSLA'25, the Verilog standard's description of Verilog's simulation semantics has internal inconsistencies and the described semantics is different from the simulation semantics used in everyday Verilog practice. 

Some relevant papers: This extended abstract from PLARCH'23 gives a short but good overview of the verification work I did during my PhD: [https://www.cs.rhul.ac.uk/home/upac096/papers/plarch23.pdf](https://www.cs.rhul.ac.uk/home/upac096/papers/plarch23.pdf). For my semantics work, I have this recent paper at OOPSLA'25: [https://doi.org/10.1145/3720484](https://doi.org/10.1145/3720484). The paper comes with a tool that visualises the simulation semantics of Verilog: [https://andreasloow.github.io/vv](https://andreasloow.github.io/vv).

<a href="/assets/images/andreas_loow_seminar_a4_poster.jpg">
  <img src="/assets/images/andreas_loow_seminar_a4_poster.jpg" alt="AI Reasoning Winter Seminar Poster" style="max-width: 100%; height: auto;">
</a>

## Proof Summit 2025 in Tokyo, Japan

<div class="tile-container">
<a href="https://proof-summit.connpass.com/event/352671/" class="tile">
  <img src="/assets/images/proof_summit.png" width="300" alt="WAIT 2025" >
</a>
</div>


## Workshop on Automated (Co)inductive Theorem Proving 2024 in Nancy, France
<div class="tile-container">
<a href="https://wait2024.github.io" class="tile">
  <img src="/assets/images/wait2024.png" width="300" alt="WAIT 2025" >
</a>
</div>
