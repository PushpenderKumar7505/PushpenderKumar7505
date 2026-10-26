<h1 align="center">Pushpender Kumar</h1>

<p align="center">
<b>DevOps Engineer · Cloud Engineer (Fresher) · AWS Infrastructure & CI/CD Automation</b><br>
Gurugram, India · B.Tech CSE (2024) · Immediate joiner · Open to Delhi NCR and Remote roles
</p>

<p align="center">
<a href="#-impact">Impact</a> ·
<a href="#-skills">Skills</a> ·
<a href="#-projects">Projects</a> ·
<a href="#-experience">Experience</a> ·
<a href="#-education--training">Education</a> ·
<a href="#-contact">Contact</a>
</p>

I automate AWS infrastructure provisioning and deployment pipelines so that nothing is done by hand twice. My hands-on work covers **Jenkins CI/CD, Ansible, Kubernetes on AWS EC2 and Linux administration**, built and documented end to end in the projects below.

**Target roles:** DevOps Engineer · Cloud Engineer · Cloud Support Engineer · Cloud Infrastructure Engineer (fresher / 0–1 year)

---

## 📈 Impact

| Metric | Result | Where |
|---|---|---|
| EC2 provisioning time | **15+ min → under 3 min (about 80% faster)** | Both CI/CD projects |
| Manual AWS console steps | **100% eliminated** | Both CI/CD projects |
| Ansible connectivity check (`ansible -m ping`) | **0 failures** across the 3-node setup | Project 1 |
| Kubernetes pod deployment | Confirmed **Running** via `kubectl` | Project 1 |

*Results are from hands-on lab and training projects, documented in the linked repositories.*

---

## 🧰 Skills

<details open>
<summary><b>Core stack (project-backed)</b></summary>

| Area | Tools |
|---|---|
| **AWS** | EC2, S3, IAM, VPC, Security Groups, CloudWatch |
| **CI/CD** | Jenkins (3-stage pipelines), GitHub Webhooks, Bash |
| **Configuration Management** | Ansible (playbooks, SSH key authentication, `amazon.aws` collection) |
| **Containers & Orchestration** | Docker, Kubernetes, kubectl |
| **OS & Scripting** | Linux (Ubuntu), Bash, YAML |
| **Version Control** | Git, GitHub |

</details>

<details>
<summary><b>Training-level and prior experience</b></summary>

| Area | Tools |
|---|---|
| **Infrastructure as Code** | Terraform (training-level; currently building hands-on projects) |
| **Monitoring** | Prometheus, Grafana, CloudWatch |
| **Backend (prior internship)** | PHP (CodeIgniter), MySQL |

</details>

---

## 🚀 Projects

### 1. End-to-End CI/CD: Jenkins → Ansible → Kubernetes on AWS
Repository: [Devops-automation-jenkins-ansible](https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible)

One GitHub push triggers the full chain, from EC2 provisioning to a running Kubernetes pod, with no manual steps.

**Pipeline flow**

```mermaid
flowchart LR
    DEV["Developer<br/>git push"] --> GH["GitHub Repository"]
    GH -->|"Webhook"| J["Jenkins Pipeline<br/>3 stages"]
    J -->|"SCP transfer<br/>ec2.yml, pod.yml"| A["Ansible Control Node"]
    A -->|"ec2.yml<br/>amazon.aws collection"| EC2["New EC2 Instance<br/>+ Security Group + Key Pair"]
    A -->|"pod.yml over<br/>passwordless SSH"| K["Kubernetes Server"]
    K --> P["Pod Running<br/>verified with kubectl"]

    style DEV fill:#1f2937,stroke:#9ca3af,color:#fff
    style GH fill:#24292f,stroke:#9ca3af,color:#fff
    style J fill:#d24939,stroke:#fff,color:#fff
    style A fill:#ee0000,stroke:#fff,color:#fff
    style EC2 fill:#ff9900,stroke:#fff,color:#000
    style K fill:#326ce5,stroke:#fff,color:#fff
    style P fill:#16a34a,stroke:#fff,color:#fff
```

<details>
<summary><b>🔍 Click to expand: infrastructure layout</b></summary>

```mermaid
flowchart TB
    ADMIN["Admin workstation<br/>MobaXterm SSH"]

    subgraph AWS["AWS Region: ap-south-1 (Mumbai)"]
        direction LR
        JEN["Jenkins Server<br/>EC2 t3.micro"]
        ANS["Ansible Control Node<br/>EC2 t3.micro"]
        K8S["Kubernetes Server<br/>EC2 c7i.flex.large"]
    end

    ADMIN -.->|"SSH"| JEN
    ADMIN -.->|"SSH"| ANS
    ADMIN -.->|"SSH"| K8S
    JEN -->|"SCP + remote execute"| ANS
    ANS -->|"Passwordless SSH<br/>ansible -m ping: 0 failures"| K8S
    ANS -->|"amazon.aws modules"| NEW["Provisioned EC2<br/>+ Security Group + Key Pair"]
```

</details>

<details>
<summary><b>🔍 Click to expand: execution sequence</b></summary>

```mermaid
sequenceDiagram
    autonumber
    actor Dev as Developer
    participant GH as GitHub
    participant J as Jenkins
    participant A as Ansible Node
    participant AWS as AWS EC2 API
    participant K as Kubernetes Server

    Dev->>GH: git push
    GH->>J: Webhook triggers pipeline
    J->>J: Stage 1: Checkout
    J->>A: Stage 2: SCP transfer of playbooks
    J->>A: Stage 3: Remote execute over SSH
    A->>AWS: ec2.yml creates EC2, Security Group, Key Pair
    A->>K: pod.yml over passwordless SSH
    K-->>A: Pod status: Running
    A-->>J: Playbook run complete
```

</details>

| What I built | Outcome |
|---|---|
| 3-stage Jenkins pipeline (Checkout → SCP Transfer → Remote Execute) | Fully automated, no manual steps |
| Ansible `ec2.yml` using the `amazon.aws` collection | EC2, Security Group, AMI and key pair created from code |
| Passwordless SSH between Ansible control node and Kubernetes server | `ansible -m ping` returned 0 failures |
| Multi-container pod deployment triggered remotely via `pod.yml` | Pods confirmed in Running state |
| 3 EC2 instances in `ap-south-1` (Jenkins, Ansible, Kubernetes) | Managed over SSH via MobaXterm |

**Stack:** `Jenkins` `Ansible` `Kubernetes` `AWS EC2` `GitHub` `SSH/SCP` `Ubuntu`

---

### 2. Automated AWS EC2 Provisioning via Jenkins CI/CD
Repository: [Jenkins-ansible-aws-ec2-provisioning](https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning)

A GitHub webhook triggers a parameterized Jenkins job that provisions EC2 on AWS, replacing manual console work.

**Pipeline flow**

```mermaid
flowchart LR
    C["Code push<br/>to GitHub"] -->|"Webhook fires"| J["Jenkins<br/>parameterized job"]
    J --> S["Bash script<br/>version-controlled"]
    S -->|"AWS API calls<br/>IAM least-privilege"| E["EC2 instance<br/>provisioned"]
    E --> R["Auditable,<br/>repeatable deployment"]

    style C fill:#24292f,stroke:#9ca3af,color:#fff
    style J fill:#d24939,stroke:#fff,color:#fff
    style S fill:#4eaa25,stroke:#fff,color:#fff
    style E fill:#ff9900,stroke:#fff,color:#000
    style R fill:#16a34a,stroke:#fff,color:#fff
```

<details>
<summary><b>🔍 Click to expand: manual vs automated</b></summary>

```mermaid
flowchart LR
    subgraph BEFORE["Before: manual, 15+ minutes"]
        direction LR
        M1["Open AWS console"] --> M2["Configure instance"] --> M3["Set security group and key"] --> M4["Launch and verify"]
    end
    subgraph AFTER["After: automated, under 3 minutes"]
        direction LR
        A1["git push"] --> A2["Jenkins job runs"] --> A3["EC2 ready"]
    end
    BEFORE ==>|"CI/CD automation"| AFTER
```

</details>

| What I built | Outcome |
|---|---|
| Parameterized Bash scripts run through Jenkins jobs | 100% of manual console clicks eliminated |
| GitHub Webhooks driving an event-based pipeline | Auto-trigger on every push, across 2 repositories |
| AWS IAM least-privilege policies | Scoped permissions for the automation user |
| End-to-end automated pipeline | Provisioning time: **15+ min → under 3 min** |

**Stack:** `Jenkins` `GitHub Webhooks` `AWS EC2` `AWS IAM` `Bash` `Ubuntu`

---

## 💼 Experience

| Role | Organization | Period |
|---|---|---|
| Associate (Incident Response), FTH | UnitedLex, Gurugram | Jul 2026 |
| Market Research Associate | Precise Research Solution, Gurugram | Jan 2025 – Jun 2025 |
| Backend Developer Intern | Mentobile Technology | Jul 2024 – Oct 2024 |

<details>
<summary><b>Click to expand: responsibilities</b></summary>

- **UnitedLex:** Investigated data breaches and classified PII/PHI in affected datasets using Relativity and Microsoft 365.
- **Precise Research Solution:** Cleaned and analysed structured datasets and produced decision-support reports for stakeholders.
- **Mentobile Technology:** Built backend modules in CodeIgniter (MVC), designed MySQL schemas and CRUD operations, and worked through Git branching, pull requests and code reviews.

</details>

---

## 🎓 Education & Training

- **B.Tech, Computer Science & Engineering**, GLA University, Mathura (2020 – 2024)
- **AWS & DevOps Infrastructure Training**, Croma Campus, NASSCOM-certified, Wipro Credential Partner (Sep 2025 – Mar 2026)

<details>
<summary><b>Click to expand: training coverage and other courses</b></summary>

- Linux administration, Git and GitHub workflows
- Jenkins CI/CD, GitHub Webhooks, Docker, Kubernetes
- AWS: EC2, S3, IAM, VPC, CloudWatch
- Terraform, Ansible, Prometheus, Grafana
- Web Development Bootcamp (JOVAC) · Front-End Development, HTML & CSS (Great Learning) · Course on Computer Concepts, CCC (NIELIT)

</details>

---

## 🌱 Currently Working On

- Terraform infrastructure as code on AWS
- Advanced Kubernetes
- Linux administration fundamentals

---

## 📬 Contact

<p align="center">
<a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://cloud-devops-shine.lovable.app"><img src="https://img.shields.io/badge/Portfolio-Visit-0d1117?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
<a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-pushpender7505@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
</p>
