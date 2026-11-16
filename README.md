<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/header-light.svg">
  <img alt="Elvis Konjoh Selabi — Smart Contract Verification, Formal Methods, Full-Stack and Blockchain Engineering" src="./assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://www.linkedin.com/in/elviskonjoh/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-elviskonjoh-0A66C2?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="https://linktr.ee/elviskonjoh"><img alt="Linktree" src="https://img.shields.io/badge/Links-linktr.ee%2Felviskonjoh-43E55E?style=flat-square&logo=linktree&logoColor=white"></a>
  <a href="https://hdl.handle.net/11581/502957"><img alt="PhD thesis" src="https://img.shields.io/badge/PhD%20Thesis-UNICAM%20%2F%20GSSI%202026-7C3AED?style=flat-square&logo=bookstack&logoColor=white"></a>
  <a href="https://doi.org/10.4230/LIPIcs.ECOOP.2026.15"><img alt="ECOOP 2026" src="https://img.shields.io/badge/ECOOP-2026-F59E0B?style=flat-square&logo=doi&logoColor=white"></a>
  <a href="https://doi.org/10.1007/978-3-031-62697-5_13"><img alt="Best Artefact Award COORDINATION 2024" src="https://img.shields.io/badge/Best%20Artefact%20Award-COORDINATION%202024-DC2626?style=flat-square&logo=starship&logoColor=white"></a>
</p>

## About

I build smart contracts that are **correct by construction**. My work turns formal behavioural models into verified, generated Solidity code and executable test suites, so the gap between a protocol's specification and its deployed code disappears.

I hold a **Ph.D. in Computer Science** (Blockchain & Distributed Ledger Technologies) from the [Gran Sasso Science Institute](https://www.gssi.it) and the [University of Camerino](https://www.unicam.it). Before research, I spent a decade shipping production software: CRM platforms for 20,000+ users, ERP systems, mobile apps, and 15+ decentralized applications across DeFi, mobility and NFTs.

- 🔬 **Research** — formal methods, behavioural types, data-aware state machines, smart contract verification
- 🛠️ **Engineering** — full-stack web and mobile, cloud backends, DApps, AI/LLM integration
- 🌍 **Impact** — 100+ developers trained on blockchain; consulting for startups across Africa, Europe and Asia

## Currently

| Role | Organisation | Since |
| --- | --- | --- |
| Software Engineer & Researcher | **Gran Sasso Tech**, L'Aquila | Jan 2026 |
| Project Manager, [E-CoRe](https://e-core.nws.cs.unibo.it/) (MSCA network) | **Università di Bologna** | Feb 2026 |
| Decentralized Ledger Technology Specialist | Freelance · Remote | Mar 2020 |

## Research

### PhD thesis — *Analysis and Verification of Smart Contracts with Behavioural Types*
<sub>GSSI & UNICAM · defended June 2026 · supervisors: Dr. Maurizio Murgia, Prof. Emilio Tuosto · <a href="https://hdl.handle.net/11581/502957">handle 11581/502957</a></sub>

Deployed smart contracts cannot be patched, and most costly exploits come from hand-written code. The thesis introduces **EDAM** (Enhanced Data-Aware Machines), a behavioural model that extends data-aware finite state machines with dynamic role-based access control, unbounded participants, and inter-contract calls with explicit success and failure handling. From an EDAM specification, the toolchain generates **Solidity contracts** and **executable Hardhat test suites**, evaluated on ERC20, AMM and other benchmarks through coverage analysis, mutation testing and cross-validation against existing implementations.

```mermaid
flowchart LR
    A["EDAM / DAFSM<br/>specification"] --> B["TRAC<br/>well-formedness check<br/>(Z3)"]
    B --> C["EDAM Studio<br/>code generation"]
    C --> D["Solidity<br/>smart contract"]
    C --> E["Hardhat<br/>test suite"]
    D --> F["Coverage ·<br/>mutation testing"]
    E --> F
```

### Selected publications

- **Automatic Code and Test Generation of Smart Contracts from Coordination Models**<br/>
  E. Konjoh Selabi, M. Murgia, A. Ravara, E. Tuosto · *ECOOP 2026*, LIPIcs vol. 372, 15:1–15:30<br/>
  [DOI](https://doi.org/10.4230/LIPIcs.ECOOP.2026.15) · [arXiv](https://arxiv.org/abs/2604.20507) · [Artifact (DARTS)](https://doi.org/10.4230/DARTS.12.1.22) · [Zenodo](https://doi.org/10.5281/zenodo.18475933)

- **TRAC: A Tool for Data-Aware Coordination (with an Application to Smart Contracts)** 🏆 *Best Artefact Award*<br/>
  J. Afonso, E. Konjoh Selabi, M. Murgia, A. Ravara, E. Tuosto · *COORDINATION 2024*, LNCS 14676, pp. 239–257<br/>
  [DOI](https://doi.org/10.1007/978-3-031-62697-5_13) · [arXiv](https://arxiv.org/abs/2404.19523) · [Code](https://github.com/loctet/TRAC)

- **Enabling Citizen Sustainable Behaviors in Urban Mobility through Blockchain and Tokenization**<br/>
  S. Meneguzzo, E. G. Konjoh Selabi, A. Favenza, V. Gatteschi, C. Schifanella · *Blockchain Technology in the Automotive Industry*, CRC Press 2024, ch. 15<br/>
  [DOI](https://doi.org/10.1201/9781003450306-17)

## Featured projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/loctet/Edam-Studio">EDAM Studio</a></h3>
      <p>Toolchain that turns EDAM specifications into Solidity code and automated Hardhat tests. Visual graph editor, text editor, CLI and API workflows.</p>
      <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
      <img alt="Solidity" src="https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white">
      <img alt="Hardhat" src="https://img.shields.io/badge/Hardhat-FFF100?style=flat-square&logo=hardhat&logoColor=black">
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/loctet/TRAC">TRAC</a></h3>
      <p>Checks the well-formedness of data-aware finite state machines (DAFSMs) with an SMT solver, so protocol errors surface before any code exists. Best Artefact Award, COORDINATION 2024.</p>
      <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
      <img alt="Z3" src="https://img.shields.io/badge/Z3-SMT%20solver-0F172A?style=flat-square">
      <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/loctet/GraphGen">GraphGen</a></h3>
      <p>FSM visualizer that renders finite state machines from JSON descriptions. Used by TRAC to draw protocol models.</p>
      <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white">
    </td>
    <td width="50%" valign="top">
      <h3>ElectionCheck</h3>
      <p>Civic-tech mobile app for electoral transparency: secure chat, geolocated reporting, a blockchain audit trail for immutable evidence, and LLM-assisted fraud analysis.</p>
      <img alt="Flutter" src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white">
      <img alt="Blockchain" src="https://img.shields.io/badge/Blockchain-audit%20trail-121D33?style=flat-square&logo=ethereum&logoColor=white">
      <img alt="OpenAI" src="https://img.shields.io/badge/OpenAI-API-412991?style=flat-square&logo=openai&logoColor=white">
    </td>
  </tr>
</table>

## Tech stack

**Languages**<br/>
<img alt="Solidity" src="https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white"> <img alt="Move" src="https://img.shields.io/badge/Move-000000?style=flat-square"> <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"> <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"> <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"> <img alt="PHP" src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white"> <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white"> <img alt="C++" src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white"> <img alt="Haskell" src="https://img.shields.io/badge/Haskell-5D4F85?style=flat-square&logo=haskell&logoColor=white"> <img alt="OCaml" src="https://img.shields.io/badge/OCaml-EC6813?style=flat-square&logo=ocaml&logoColor=white">

**Formal methods & verification**<br/>
<img alt="Z3" src="https://img.shields.io/badge/Z3-SMT%20solver-0F172A?style=flat-square"> <img alt="Behavioural types" src="https://img.shields.io/badge/Behavioural%20types-4F46E5?style=flat-square"> <img alt="Transition systems" src="https://img.shields.io/badge/Transition%20systems-0D9488?style=flat-square"> <img alt="Mutation testing" src="https://img.shields.io/badge/Mutation%20testing-B91C1C?style=flat-square">

**Blockchain**<br/>
<img alt="Ethereum" src="https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white"> <img alt="IOTA" src="https://img.shields.io/badge/IOTA-131F37?style=flat-square&logo=iota&logoColor=white"> <img alt="Hardhat" src="https://img.shields.io/badge/Hardhat-FFF100?style=flat-square&logo=hardhat&logoColor=black"> <img alt="Truffle" src="https://img.shields.io/badge/Truffle-5E464D?style=flat-square"> <img alt="Ethers.js" src="https://img.shields.io/badge/Ethers.js-2535A0?style=flat-square"> <img alt="Web3.js" src="https://img.shields.io/badge/Web3.js-F16822?style=flat-square&logo=web3dotjs&logoColor=white">

**Web, mobile & cloud**<br/>
<img alt="React" src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"> <img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"> <img alt="Flutter" src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"> <img alt="SQL" src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white"> <img alt="NoSQL" src="https://img.shields.io/badge/NoSQL-47A248?style=flat-square&logo=mongodb&logoColor=white"> <img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white"> <img alt="DigitalOcean" src="https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white"> <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">

**AI**<br/>
<img alt="LLMs" src="https://img.shields.io/badge/LLMs-integration-111827?style=flat-square"> <img alt="RAG" src="https://img.shields.io/badge/RAG-retrieval%20augmented-6D28D9?style=flat-square"> <img alt="Prompt engineering" src="https://img.shields.io/badge/Prompt%20engineering-0369A1?style=flat-square">

## Recognition & service

- 🏆 **Best Artefact Award** + EAPLS *Available* and *Reusable* badges — COORDINATION 2024
- 🥈 **Second Prize**, IOTA Foundation Hackathon — Move smart contract DApp (2020)
- 🎤 **Invited speaker**, Ethereum Zurich 2025 · talk at **DTU** Copenhagen (2024)
- 🧑‍⚖️ **Artifact Evaluation Committee**, FM 2026 (Tokyo) · **Program Committee**, COMPSAC Mentorium 2025 (Toronto)
- 🎓 Ph.D. scholarship, GSSI (2022–2026) · Master scholarship & best student award, Zhejiang Provincial Government (2016–2017)

<details>
<summary><b>Experience & education</b></summary>

<br/>

**Experience**

| Period | Role | Where |
| --- | --- | --- |
| 2026 – now | Software Engineer & Researcher | Gran Sasso Tech, L'Aquila |
| 2026 – now | Project Manager, E-CoRe (MSCA) | Università di Bologna |
| 2025 | Visiting Researcher (4 months) | Technical University of Denmark (DTU), Copenhagen |
| 2023 | Research Collaborator | NOVA University Lisbon |
| 2020 – now | DLT Specialist & trainer | Freelance |
| 2019 – 2023 | Full-Stack Web Developer, Scrum Master & Team Lead | Marco Vasco, Shanghai |
| 2013 – 2015 | Junior Software Engineer | AfreelTech & Infrastel, Yaoundé |

**Education**

| Period | Degree | Institution |
| --- | --- | --- |
| 2022 – 2026 | Ph.D. in Computer Science (BDLT) | GSSI & University of Camerino, Italy |
| 2015 – 2017 | M.Sc. in Software Engineering | Zhejiang Normal University, China |
| 2008 – 2013 | B.Sc. in Computer Science | University of Yaoundé I, Cameroon |

**Languages:** French (native) · English (C1) · Chinese (A1)

</details>

---

<p align="center">
  <b>Open to research collaborations, postdoc positions, and blockchain / formal-methods engineering projects.</b><br/>
  <sub>Reach me on <a href="https://www.linkedin.com/in/elviskonjoh/">LinkedIn</a> or via <a href="https://linktr.ee/elviskonjoh">linktr.ee/elviskonjoh</a>.</sub>
</p>
