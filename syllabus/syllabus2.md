# **Engineering Research in Computer Systems (13-Week Syllabus)**

**Level:** MS / early PhD
**Focus:** Operating Systems, Networks, Computer Architecture, Security
**Outcome:** A conference-ready systems paper + reproducible artifact

---

## **Week 1 — What “Research” Means in Systems**

**Topics:**

* Systems research vs. engineering
* Three pillars: performance, correctness, scalability
* Types of contributions: mechanism, insight, evaluation
* Storytelling in systems: problem → mechanism → design → evaluation

**Readings:**

* Saltzer & Kaashoek, *Principles of Computer System Design*, Ch. 1
* Hennessy & Patterson, “A New Golden Age for Computer Architecture” (CACM)
* David C. Clark et al., “Design Philosophy of the DARPA Internet Protocols”

**Deliverable:**

* Pick 3 SOSP/OSDI/NSDI papers
* Identify for each: problem, mechanism, system built, evaluation metric, why accepted/rejected

---

## **Week 2 — How to Read and Analyze Systems Papers**

**Topics:**

* Paper anatomy: problem → insight → system → evaluation
* Spotting novelty vs incremental work

**Readings:**

* Keshav, *How to Read a Paper*
* Arpaci-Dusseau & Arpaci-Dusseau, *Operating Systems: Three Easy Pieces*, Ch. 1
* Any recent OSDI/NSDI best paper

**Deliverable:**

* Dissect 1 paper: assumptions, system model, bottleneck, what could break

---

## **Week 3 — Finding Research Problems**

**Topics:**

* Sources of problems: hardware, workloads, failures, security attacks
* Recognizing publishable gaps

**Readings:**

* HotOS proceedings (last 2 editions)
* Hennessy & Patterson, *Computer Architecture: A Quantitative Approach*, Ch. 1
* Barroso et al., *The Datacenter as a Computer*, Ch. 1

**Deliverable:**

* Write 5 problem statements using:

> “Current systems fail when ___ because ___.”

---

## **Week 4 — Turning Problems into Research Questions**

**Topics:**

* Converting problems into measurable, falsifiable hypotheses
* Research question → hypothesis → metrics

**Readings:**

* Jim Gray, “Why Do Computers Stop and What Can Be Done About It?”
* Dean & Barroso, “The Tail at Scale” (CACM)
* One NSDI paper with strong evaluation

**Deliverable:**

* For 2 problems:

  * Research question
  * Hypothesis
  * Metric

---

## **Week 5 — Experimental Methodology**

**Topics:**

* Microbenchmarks vs macrobenchmarks
* Controlled experiments
* Threats to validity in systems experiments

**Readings:**

* Mytkowicz et al., “Producing Wrong Data Without Doing Anything Obviously Wrong”
* ACM SIGMETRICS evaluation guidelines
* Paxson, “Strategies for Sound Internet Measurement”

**Deliverable:**

* Design a full experiment: variables, controls, metrics, expected outcomes

---

## **Week 6 — Systems Prototyping**

**Topics:**

* Prototyping levels: kernel/user-space, emulator, trace-driven simulation
* Build only what touches the bottleneck
* Minimal prototypes vs full systems

**Readings:**

* Feamster et al., “The Case for Reproducible Networking Research”
* Arpaci-Dusseau, “The Development of the Cedar File System”
* EuroSys papers with new systems

**Deliverable:**

* Decide: real system, emulator, or trace-based model
* Justify choice

---

## **Week 7 — Measurement Infrastructure**

**Topics:**

* Observing system behavior correctly
* Low-level vs high-level metrics
* Perf, eBPF, tracing, profiling

**Readings:**

* Brendan Gregg, *Systems Performance*, Ch. 1–3
* Linux perf documentation
* Gregg, “The USE Method”

**Deliverable:**

* Build measurement scripts producing latency distribution, CPU breakdown, queueing behavior

---

## **Week 8 — Data Analysis for Systems**

**Topics:**

* Tail latency, throughput, resource efficiency
* Repeatability, variance, confidence intervals
* Avoid cherry-picking

**Readings:**

* Dean & Barroso, “The Tail at Scale”
* Jain, *The Art of Computer Systems Performance Analysis*, Ch. 11
* SIGMETRICS papers

**Deliverable:**

* Graphs showing mechanism + performance: mean, P95, P99
* Explain why improvements occur

---

## **Week 9 — Positioning Against Prior Work**

**Topics:**

* Literature mapping: table of prior systems
* Identifying gaps
* Related Work storytelling
* Anticipating reviewer critiques

**Readings:**

* Armstrong et al., “Towards a Common Benchmark for DB Systems”
* Feamster & Rexford, “Why (and How) Networks Should Run Themselves”
* Related Work sections from OSDI/SOSP papers

**Deliverable:**

* Literature map table
* Head-to-head comparison plan
* Draft Related Work section
* Gap statement

---

## **Week 10 — Writing the Paper**

**Topics:**

* Paper structure: title, abstract, intro, evaluation, conclusion
* Storytelling through metrics
* Emphasize mechanism and impact

**Readings:**

* Simon Peyton Jones, “How to Write a Great Research Paper”
* OSDI paper template (USENIX)
* Top systems papers (OSDI/SOSP/NSDI)

**Deliverable:**

* Draft title, abstract, and introduction

---

## **Week 11 — Evaluation That Survives Reviewers**

**Topics:**

* Ablation, sensitivity, stress tests
* Show mechanism behind performance improvements
* Edge cases (P50, P95, P99)
* Repeatability and statistical rigor

**Readings:**

* Pat Helland, “Life Beyond Distributed Transactions”
* Harchol-Balter, *Performance Modeling and Design of Computer Systems*, Ch. 2
* 2 NSDI papers with deep evaluation

**Deliverable:**

* Complete evaluation plan with:

  * Ablation and sensitivity studies
  * Head-to-head comparisons
  * Mechanism graphs
  * Repeatable scripts

---

## **Week 12 — Reproducibility and Artifacts**

**Topics:**

* Docker, scripts, VMs for reproducible experiments
* Artifact evaluation committees
* Open science and sharing

**Readings:**

* NSDI Artifact Evaluation Guidelines
* “Repeatability in Computer Systems Research” (EuroSys)
* Docker / containerization documentation

**Deliverable:**

* Package system and experiments so another student can run them successfully

---

## **Week 13 — Submission and Review**

**Topics:**

* How top-tier systems conference review works
* Rebuttal strategies
* Surviving rejection and revision

**Readings:**

* “How to Get a Paper Accepted at OSDI” (Stoica)
* SIGCOMM / SOSP review guidelines
* Sample HotCRP reviews

**Deliverable:**

* Mock program committee: review classmates’ papers
* Prepare rebuttal for your own draft

---

# **Final Outcome**

By the end of Week 13, you will have:

* A **working systems prototype**
* A **real evaluation with graphs, stats, and comparisons**
* A **conference-ready paper** for OSDI/SOSP/NSDI/EuroSys

This syllabus follows the same pipeline used in **MIT PDOS, Berkeley RISELab, CMU Systems, ETH Systems, and Microsoft Research**.


