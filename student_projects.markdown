---
layout: default
title: Student Projects
---

I am interested in projects that explore the correctness of **concurrent and distributed systems**. This includes developing tools for **visualisation**, **simulation**, **verification** and other **applications**.  Students will benefit most from working in **groups of two or three**. I am happy to supervise projects from all study programmes, both at the BSc and MSc level, including MSc theses.



**Projects**

- *Proving Theorems with AI: An Experiment in Vibe-Proving*
  + Proof assistants such as [Rocq](https://rocq-prover.org) (formerly Coq) allow proving mathematical theorems and program properties with machine-checked certainty — but proof engineering is labour-intensive. Can modern AI assistants (Claude, Copilot, etc.) do the heavy lifting? This project is an *experiment and evaluation*: pick a target formalisation — e.g. a small process calculus or choreographic language, a type system, or a data structure library — and develop it in Rocq with AI assistance, systematically recording where AI-generated proofs succeed, fail, or mislead, and measuring the effort saved compared to manual proving. The deliverables are a mechanised formalisation and an evidence-based report on AI-assisted proof engineering: methodology, metrics, and lessons learned. No prior Rocq experience is required, but functional programming (F#/Haskell/OCaml) and comfort with logic are expected.
  + **Keywords:** proof assistants, Rocq, AI-assisted proving, formal verification, empirical evaluation
  + **Level:** MSc / ambitious BSc

<br>

- *Neural Network-Based Protocol Mining*
  + Develop a tool that trains a neural network to infer communication protocols from network traces. The network is trained on observed traces paired with known protocol specifications and, once trained, can predict unknown or partially observed protocol behaviors. The protocol language may include probabilistic elements, capturing message choices, delays, or failures. The project will require designing the neural network, generating synthetic training data (e.g., via an automatic protocol generator), and validating predictions through simulations. The deliverables include a working prototype capable of learning from traces and producing estimated protocol representations.
  + **Keywords:** neural networks, protocol mining, distributed systems, tool, simulation
  + **Level:** BSc/MSc

<br>

- *Extracting and Verifying Communication Protocols from Distributed (Rust) Code*
  + Develop a tool that analyses distributed programs (preferably in Rust but other programming languages are possible) and automatically extracts all communication operations, abstracting them into a protocol representation or state machine. The tool should then translate this representation into the input language of a model checker such as SPIN (Promela) or TLA+ (TLC), enabling verification of properties like functional correctness, deadlock freedom, or other protocol-level guarantees. Students will experiment with real Rust implementations and demonstrate the approach on a few concrete examples. As an optional extension, the tool may handle dropped or out-of-order messages to explore robustness under realistic distributed conditions.
  + **Keywords:** messaging, protocols, distributed systems, model checking
  + **Level:** BSc/MSc

<br>

- *Probabilistic Choreographies and PRISM*
  + Real-world protocols are often probabilistic: messages get dropped or delayed, and protocols themselves make randomised choices. In recent work ([COORDINATION 2024](https://doi.org/10.1007/978-3-031-62697-5_2), with an [extended version](https://arxiv.org/abs/2503.08530) to appear in LMCS), we developed a choreographic language for describing probabilistic protocols from a global viewpoint, together with a compiler translating it into the input language of the [PRISM](https://www.prismmodelchecker.org) probabilistic model checker. This project extends this framework in one or more directions: (1) *property specification at the choreographic level* — express quantitative properties ("probability of termination within n steps") directly on the choreography and compile them to PRISM's property language; (2) *result interpretation* — map PRISM's analysis results and counterexamples back to the choreography, e.g. by visualising problematic runs; (3) *language extensions* — e.g. asynchronous communication or parameterised participants, with the corresponding translation; or (4) *case studies* — model and verify substantial randomised protocols (gossip, randomised consensus, blockchain-style protocols) in the language. Scope is adjusted to group size and level.
  + **Keywords:** probabilistic model checking, PRISM, choreographies, distributed protocols
  + **Level:** BSc/MSc

<br>

- *From Global Protocols to Local Code: Endpoint Projection for Choreographies*
  + Choreographic languages describe communication protocols from a global viewpoint ("Alice sends to Bob"). Not every choreography makes sense: when a choreography branches, participants behaving differently in each branch must be informed of the choice (*knowledge of choice*). This project develops a *choreography compiler*: (1) a well-formedness checker enforcing conditions such as knowledge of choice, and (2) *endpoint projection* — automatic generation of per-participant code (local state machines or executable stubs in e.g. Rust, Erlang, or Akka) from the global description. The generated code is correct by construction: it cannot deadlock or mismatch messages. The project involves defining the projection function, implementing it, and demonstrating it on concrete protocols. As an optional extension, the tool may include an interactive visualisation of the projected local behaviours.
  + **Keywords:** choreographies, endpoint projection, session types, compilers, concurrency
  + **Level:** BSc/MSc
