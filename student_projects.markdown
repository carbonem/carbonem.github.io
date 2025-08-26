---
layout: default
title: Student Projects
---

I am interested in supervising student projects that explore the correctness of **concurrent and distributed systems**, often through the development of tools for **visualisation tools**, **simulation** and other **applications**.  Students will benefit most from working in **groups of two or three**, where they can collaborate and share expertise. I am happy to supervise projects from all study programmes, both at the BSc and MSc level, including MSc theses.



**Projects:**

- **Distributed Protocol Visualisation**
  + Develop a tool that reads a specification of a communication protocol (in a choreographic language or some other simple DSL) and produces an interactive visualisation that represents the protocol. By interacting with it, one can explore the different possible runs of the protocol, including branching choices, concurrent steps, and parallel interactions. The project will require designing a small protocol language or format, implementing the visualisation tool, and exploring case studies. The project deliverables include a working prototype with at least two protocols fully represented and a report on how concurrency and protocol correctness are modelled. As an optional extension, the tool may simulate probabilistic message delivery.
  + **Keywords:** visualisation, distributed protocols, concurrency, tooling
  + **Level:** BSc/MSc

<br>

- **Extracting and Verifying Communication Protocols from Distributed Rust Code**
  + Develop a tool that analyses distributed Rust programs and automatically extracts all communication operations, abstracting them into a protocol representation or state machine. The tool should then translate this representation into the input language of a model checker such as SPIN (Promela) or TLA+ (TLC), enabling verification of properties like functional correctness, deadlock freedom, or other protocol-level guarantees. Students will experiment with real Rust implementations and demonstrate the approach on a few concrete examples. As an optional extension, the tool may handle dropped or out-of-order messages to explore robustness under realistic distributed conditions.
  + **Keywords:** messaging, protocols, distributed systems, model checking
  + **Level:** BSc/MSc





- [Interactive DSL for Structured Content in Jupyter (with Dan W. Hansen)](http://itu.dk/people/maca/student_projects/Jupiter_Notebooks_Python_DSL.pdf)
