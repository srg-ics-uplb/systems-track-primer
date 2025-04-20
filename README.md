# 🧠 2-Month Systems Study Plan (Plan B)

**Goal**: Build strong foundational knowledge and practical skills in operating systems, architecture, networking, security, and cloud.

**Schedule**: 3x per week • 2 hours per session • 6 hours/week

---

## 📅 Week 1–2: Operating Systems

### ✅ W1-S1: Intro to Operating Systems
- OS responsibilities: abstraction, resource sharing, protection
- Kernel vs user space
- System calls: `fork()`, `exec()`, `read()`, `write()`
- Types of OS architectures: monolithic, microkernel
- **Resource**: [Harvard CS50 OS Video](https://youtu.be/26QPDBe-NB8)
- **Hands-on**: Explore basic syscalls in C; Read [Linux From Scratch](https://www.linuxfromscratch.org/)

---

### ✅ W1-S2: Processes, Threads, Context Switching
- Process lifecycle: creation → scheduling → termination
- User vs kernel threads
- Context switching mechanism
- Scheduling policies: FCFS, RR, MLFQ
- **Resource**: [MIT 6.S081 Lectures 1–2](https://pdos.csail.mit.edu/6.S081/2020/lec/)
- **Lab**: [xv6 Unix Utilities Lab](https://pdos.csail.mit.edu/6.S081/2020/labs/)

---

### ✅ W1-S3: Scheduling & Signals
- Signal handling (e.g., `kill`, `SIGINT`)
- Preemptive vs cooperative scheduling
- Simulate a user-space round-robin scheduler
- **Resource**: [OSTEP Ch. 5–7](http://pages.cs.wisc.edu/~remzi/OSTEP/)
- **Lab**: Build basic C scheduler with signal handling

---

### ✅ W2-S1: Virtual Memory & Paging
- Virtual memory abstraction
- Page tables, TLB, segmentation
- Memory protection
- **Resource**: OSTEP Ch. 13–17
- **Lab**: [MIT xv6 Memory Lab](https://pdos.csail.mit.edu/6.S081/2020/labs/memory.html)

---

### ✅ W2-S2: File Systems & I/O
- Syscalls: `open`, `read`, `write`, `stat`
- Inodes, directory structure, block layout
- Buffer cache basics
- **Resource**: OSTEP Ch. 36–42
- **Lab**: xv6 file system walk-through

---

### ✅ W2-S3: Mini-Project – Extend xv6 Shell
- Add history, I/O redirection, pipes
- Understand parsing & forking in xv6 shell
- **Codebase**: [xv6 source](https://github.com/mit-pdos/xv6-public)

---

## 📅 Week 3–4: Computer Architecture

### ✅ W3-S1: CPU, ALU, Instruction Execution
- Instruction cycle (fetch-decode-execute)
- ALU and control logic
- **Resource**: [CrashCourse Computer Architecture](https://www.youtube.com/playlist?list=PL8dPuuaLjXtOfse2ncvffeelTrqvhrz8H)
- **Lab**: Simulate CPU in [Logisim](http://www.cburch.com/logisim/)

---

### ✅ W3-S2: Pipelining & Branch Prediction
- 5-stage pipeline
- Hazards: structural, data, control
- Branch prediction: static vs dynamic
- **Resource**: [CMU 15-213](https://www.cs.cmu.edu/~213/schedule.html)
- **Lab**: Write simple pipeline simulator

---

### ✅ W3-S3: Assembly Programming (RISC-V)
- Instructions: `addi`, `lw`, `sw`, `jal`, `beq`
- Stack frames, calling convention
- **Tools**: [RISC-V Green Card](https://inst.eecs.berkeley.edu/~cs61c/fa17/img/riscvcard.pdf), [Venus Simulator](https://venus.cs61c.org/)

---

### ✅ W4-S1: Memory Hierarchy
- Registers, cache, DRAM, disk
- Locality (temporal/spatial), cache layout
- **Resource**: CS61C Lectures
- **Lab**: Simulate cache hit/miss rates

---

### ✅ W4-S2: Performance Tools & Profiling
- Use `perf`, `valgrind`, `gprof`
- Measure CPU-bound vs memory-bound workloads
- **Resource**: OSTEP + [CS:APP](http://csapp.cs.cmu.edu/)
- **Lab**: Profile and optimize a C program

---

### ✅ W4-S3: Mini Project – CPU Instruction Simulator
- Simulate register file, PC, and memory
- Build basic CPU that executes custom instructions

---

## 📅 Week 5–6: Networking + Distributed Systems

### ✅ W5-S1: Network Stack & Ethernet
- Layered model (App → Link)
- Subnetting, ARP, DHCP
- **Resource**: [Computer Networking: Top-Down](https://gaia.cs.umass.edu/kurose_ross/)
- **Lab**: Use Wireshark to capture DHCP & ARP

---

### ✅ W5-S2: TCP vs UDP
- TCP 3-way handshake
- Flow and congestion control
- **Resource**: Kurose/Ross Ch. 3–5
- **Lab**: Write TCP/UDP echo servers in Python

---

### ✅ W5-S3: Distributed Systems Basics
- CAP theorem
- Latency vs throughput
- Failure models
- **Resource**: [MIT 6.824 Lecture 1](https://pdos.csail.mit.edu/6.824/)
- **Visualization**: [Raft Demo](https://thesecretlivesofdata.com/raft/)

---

### ✅ W6-S1: Remote Procedure Call (RPC)
- Client-server structure
- Timeout & retry mechanism
- **Resource**: MIT 6.824 RPC lecture
- **Lab**: [gRPC Python Tutorial](https://grpc.io/docs/languages/python/quickstart/)

---

### ✅ W6-S2: Consensus & Time
- Logical clocks, vector clocks
- Paxos basics
- **Resource**: [Paxos Made Simple](https://lamport.azurewebsites.net/pubs/pubs.html#paxos-simple)
- **Lab**: Simulate time sync with drift in Python

---

### ✅ W6-S3: Mini-Project – Distributed KV Store
- Build a 2-node put/get key-value store
- Use sockets, threads, logs
- Add basic retry/fault handling

---

## 📅 Week 7–8: Security + Cloud

### ✅ W7-S1: Threat Models & Security Design
- CIA Triad, STRIDE
- Authentication vs Authorization
- **Resource**: [CS161 Lectures](https://cs161.org/)
- **Lab**: Threat model a messaging app

---

### ✅ W7-S2: Memory Safety Vulnerabilities
- Buffer overflow, stack smashing
- Format string bugs, canaries, ASLR
- **Resource**: [LiveOverflow CTF](https://www.youtube.com/c/LiveOverflow)
- **Lab**: Trigger overflow in C

---

### ✅ W7-S3: Web Security – XSS, SQLi, CSRF
- Input sanitization, cookies, same-origin
- CSRF tokens
- **Lab**: [PortSwigger Labs](https://portswigger.net/web-security)

---

### ✅ W8-S1: VMs vs Containers
- Hypervisors, snapshots, isolation
- Docker vs QEMU vs KVM
- **Resource**: [GCP Cloud Foundations](https://www.cloudskillsboost.google/)
- **Lab**: Spin up a VM and container (GCP or local)

---

### ✅ W8-S2: Docker + Kubernetes Basics
- Dockerfile, build, volumes
- Kubernetes: pods, services, deployments
- **Tutorial**: [Kubernetes Basics](https://kubernetes.io/docs/tutorials/kubernetes-basics/)
- **Lab**: Deploy Flask app with Docker/K8s

---

### ✅ W8-S3: Capstone – Secure Flask App Deployment
- Flask app + SQLite + HTTPS
- Dockerized, served with Nginx or Gunicorn
- TLS via Let's Encrypt (`certbot`)
- Deploy on GCP/VM/Docker Compose

---

# ✅ Optional Tools
- **Simulators**: [Logisim](http://www.cburch.com/logisim/), [Ripes](https://github.com/mortbopet/Ripes), [Godbolt](https://godbolt.org/)
- **Security Labs**: [TryHackMe](https://tryhackme.com/), [picoCTF](https://picoctf.org/)
- **Cloud Labs**: [Katacoda (O'Reilly)](https://katacoda.com/), [GCP Labs](https://www.cloudskillsboost.google/)

