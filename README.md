<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1a2e,100:16213e&height=180&section=header&text=Akshay%20Raj&fontSize=56&fontColor=58a6ff&fontAlignY=38&desc=Systems%20%7C%20Security%20%7C%20ML&descAlignY=58&descSize=18&descColor=8b949e)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/akshay-raj-0aa751217)
[![GitHub](https://img.shields.io/badge/GitHub-Akshay--X--Raj-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Akshay-X-Raj)
[![Email](https://img.shields.io/badge/Email-akshayraj2502%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:akshayraj2502@gmail.com)

</div>

---

3rd-year CS student who builds systems from first principles — futex primitives, RDTSC hardware profiling, DB-enforced state machines. I care about *why* a design decision was made, not just that it works.

Currently open to internships in **systems programming**, **backend infrastructure**, or **security**.

---

### Projects

---

#### ⚡ [ZeroRPC](https://github.com/Akshay-X-Raj/ZeroRPC) &nbsp;·&nbsp; `C++` `Linux` `Systems`

Unified RPC interface over 4 transports — Unix sockets, TCP, pipes, and POSIX shared memory — letting callers switch transports without changing application code.

- Profiled all transports with **RDTSC hardware counters**: shared memory dominated at every latency percentile, demonstrating that eliminating kernel-mediated copies is the critical factor in IPC performance
- Used **futex primitives** to minimise kernel round-trips on the shared memory path
- Shipped a **Dear ImGui + SDL2 + OpenGL** dashboard that sends live RPC calls and renders per-request latency histograms in real time; exports full run logs to CSV

`futex` `POSIX shared memory` `RDTSC profiling` `Dear ImGui` `TCP / Unix sockets`

---

#### 🗂️ [Issue Tracker](https://github.com/Akshay-X-Raj/Issue-Tracker) &nbsp;·&nbsp; `Node.js` `PostgreSQL` `Docker`

Production-deployed issue tracker with a strict 5-state lifecycle enforced at the **database layer** via a workflow transitions table — illegal state jumps are impossible regardless of application logic.

- Instrumented every write path with **audit-logging middleware**: actor, timestamp, and delta recorded for each entity change, exposed through a paginated API endpoint
- Secured with **JWT authentication + role-based access control**; containerised with Docker Compose and deployed on free-tier infrastructure (Cloudflare Pages · Render · Neon)

`DB-enforced state machine` `audit logging` `JWT + RBAC` `Docker Compose` `REST API`

---

#### 🛡️ [Ransomware Detection](https://github.com/Akshay-X-Raj/Ransomeware_tool) &nbsp;·&nbsp; `Python` `scikit-learn` `Linux`

End-to-end autonomous containment pipeline: on consecutive high-confidence detections, the system isolates the host from the network, terminates the offending process, and backs up critical files — no human intervention required.

- Random Forest classifier trained on the **Zenodo 2024 ransomware dataset** spanning multiple malware families; achieved **zero false negatives** on held-out malicious samples
- Live behavioural monitor via **psutil** polls process activity, file I/O, network connections, and shared library usage; Windows-trained model bridged to Linux by mapping equivalent OS telemetry signals

`Random Forest` `autonomous containment` `cross-platform ML` `psutil` `behavioural analysis`

---

#### 🔑 [VM Encryption Framework](https://github.com/ARYAN-KUMAR-22/Cyber) &nbsp;·&nbsp; `Java` `AES-128` `CloudSim`

Implemented all ten AES-128 cipher rounds (SubBytes, ShiftRows, MixColumns, AddRoundKey) from scratch in Java alongside PKCS#7 padding and cryptographically secure key generation, wired into a CloudSim VM-communication pipeline.

`AES-128` `cryptography` `CloudSim` `SecureRandom`

---

### Tech Stack

**Languages** &nbsp;
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Systems & Security** &nbsp;
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)

**Backend & Infra** &nbsp;
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)

**Tools** &nbsp;
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![NeoVim](https://img.shields.io/badge/NeoVim-57A143?style=flat-square&logo=neovim&logoColor=white)

---

### Currently

- Exploring **adversarial ML** techniques for malware evasion & detection
- Deepening expertise in **Linux kernel internals** and kernel security
- Open to collaborating on security tools, CTF challenges, and open-source systems projects

---

<div align="center">

![footer](https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0d1117&height=100&section=footer)

</div>
