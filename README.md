<!-- Banner -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0f2027,50:203a43,100:2c5364&text=Pushpender%20Kumar&fontColor=ffffff&fontSize=52&fontAlignY=38&desc=DevOps%20%7C%20Cloud%20%7C%20AWS%20Infrastructure%20%26%20CI%2FCD%20Automation&descAlignY=58&descSize=18&animation=fadeIn" alt="Pushpender Kumar banner" />

<!-- Typing animation -->
<p align="center">
  <a href="https://github.com/PushpenderKumar7505">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=800&color=2DD4BF&center=true&vCenter=true&width=700&lines=I+automate+AWS+infrastructure+%E2%98%81%EF%B8%8F;One+git+push+%E2%86%92+Jenkins+%E2%86%92+Ansible+%E2%86%92+Kubernetes+%F0%9F%9A%80;Nothing+should+be+done+by+hand+twice+%E2%9A%99%EF%B8%8F;Open+to+DevOps+%26+Cloud+roles+%7C+Immediate+joiner+%F0%9F%92%BC" alt="Typing animation" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Open%20to%20Work-Immediate%20Joiner-16a34a?style=for-the-badge&logo=target&logoColor=white" alt="Open to work" />
  <img src="https://img.shields.io/badge/Location-Gurugram%2C%20India-0ea5e9?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />
  <img src="https://img.shields.io/badge/Roles-DevOps%20%7C%20Cloud%20%7C%20SRE-f59e0b?style=for-the-badge&logo=amazonaws&logoColor=white" alt="Target roles" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://cloud-devops-shine.lovable.app"><img src="https://img.shields.io/badge/Portfolio-Visit-0d1117?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://komarev.com/ghpvc/?username=PushpenderKumar7505&label=Profile%20Views&color=2c5364&style=for-the-badge" alt="Profile views" />
</p>

---

## 👋 About Me

```yaml
name: Pushpender Kumar
role: DevOps / Cloud Engineer (Fresher)
education: B.Tech CSE, GLA University (2024)
training: NASSCOM-certified AWS & DevOps Infrastructure (Croma Campus, Wipro Credential Partner)
focus: [AWS, Jenkins CI/CD, Ansible, Kubernetes, Linux]
location: Gurugram, India
availability: Immediate joiner (Delhi NCR / Noida / Pune / Remote)
```

> 💡 I build deployment pipelines where **a single `git push` provisions the infrastructure and ships the workload**, with no manual console clicks.

---

## 📈 Impact at a Glance

<div align="center">

| ⚡ EC2 Provisioning | 🖱️ Manual Console Steps | 🔗 Ansible Ping Check | ☸️ K8s Pod Deployment |
|:---:|:---:|:---:|:---:|
| **15+ min → under 3 min**<br>(≈80% faster) | **100% eliminated** | **0 failures**<br>(3-node setup) | **Running**<br>(verified via `kubectl`) |

<sub>Results are from hands-on lab and training projects, documented in the linked repositories.</sub>

</div>

---

## 🧰 Tech Stack

<div align="center">

**☁️ Cloud & CI/CD**<br>
<img src="https://skillicons.dev/icons?i=aws,jenkins,github,git&theme=dark" alt="Cloud and CI/CD" />

**⚙️ Automation, Containers & IaC**<br>
<img src="https://skillicons.dev/icons?i=ansible,docker,kubernetes,terraform&theme=dark" alt="Automation and containers" />

**🐧 OS, Scripting & Monitoring**<br>
<img src="https://skillicons.dev/icons?i=linux,ubuntu,bash,prometheus,grafana&theme=dark" alt="OS and monitoring" />

**🗄️ Prior Backend Experience**<br>
<img src="https://skillicons.dev/icons?i=php,mysql&theme=dark" alt="Backend" />

</div>

<details>
<summary><b>📋 Detailed skill breakdown</b></summary>

<br>

| Area | Tools | Level |
|---|---|---|
| **AWS** | EC2, S3, IAM, VPC, Security Groups, CloudWatch | Project-backed |
| **CI/CD** | Jenkins (3-stage pipelines), GitHub Webhooks, Bash | Project-backed |
| **Config Management** | Ansible (playbooks, SSH key auth, `amazon.aws` collection) | Project-backed |
| **Containers & Orchestration** | Docker, Kubernetes, kubectl | Project-backed |
| **OS & Scripting** | Linux (Ubuntu), Bash, YAML | Project-backed |
| **Infrastructure as Code** | Terraform | Training-level, building hands-on projects |
| **Monitoring** | Prometheus, Grafana, CloudWatch | Training-level |
| **Backend** | PHP (CodeIgniter), MySQL | Prior internship |

</details>

---

## 🚀 Featured Projects

### 1️⃣ End-to-End CI/CD: Jenkins → Ansible → Kubernetes on AWS

[![Repo](https://img.shields.io/badge/View%20Repository-Devops--automation--jenkins--ansible-181717?style=for-the-badge&logo=github)](https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible)

One GitHub push triggers the full chain, from EC2 provisioning to a running Kubernetes pod.

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

| What I built | Outcome |
|---|---|
| 3-stage Jenkins pipeline (Checkout → SCP Transfer → Remote Execute) | Fully automated, no manual steps |
| Ansible `ec2.yml` using the `amazon.aws` collection | EC2, Security Group, AMI and key pair created from code |
| Passwordless SSH between Ansible node and Kubernetes server | `ansible -m ping` returned 0 failures |
| Multi-container pod deployment triggered remotely via `pod.yml` | Pods confirmed in Running state |
| 3 EC2 instances in `ap-south-1` (Jenkins, Ansible, Kubernetes) | Managed over SSH via MobaXterm |

<details>
<summary><b>🔍 Infrastructure layout</b></summary>

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
<summary><b>🔍 Execution sequence</b></summary>

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

**Stack:** `Jenkins` `Ansible` `Kubernetes` `AWS EC2` `GitHub` `SSH/SCP` `Ubuntu`

---

### 2️⃣ Automated AWS EC2 Provisioning via Jenkins CI/CD

[![Repo](https://img.shields.io/badge/View%20Repository-Jenkins--ansible--aws--ec2--provisioning-181717?style=for-the-badge&logo=github)](https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning)

A GitHub webhook triggers a parameterized Jenkins job that provisions EC2 on AWS, replacing manual console work.

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

| What I built | Outcome |
|---|---|
| Parameterized Bash scripts run through Jenkins jobs | 100% of manual console clicks eliminated |
| GitHub Webhooks driving an event-based pipeline | Auto-trigger on every push, across 2 repositories |
| AWS IAM least-privilege policies | Scoped permissions for the automation user |
| End-to-end automated pipeline | Provisioning time: **15+ min → under 3 min** |

**Stack:** `Jenkins` `GitHub Webhooks` `AWS EC2` `AWS IAM` `Bash` `Ubuntu`

---

## 💼 Experience

```text
2026 ─┬─ Jul 2026       Associate (Incident Response), FTH ........ UnitedLex, Gurugram
2025 ─┼─ Jan – Jun 2025 Market Research Associate ................. Precise Research Solution, Gurugram
2024 ─┴─ Jul – Oct 2024 Backend Developer Intern .................. Mentobile Technology
```

<details>
<summary><b>📌 Responsibilities</b></summary>

- **UnitedLex:** Investigated data breaches and classified PII/PHI in affected datasets using Relativity and Microsoft 365.
- **Precise Research Solution:** Cleaned and analysed structured datasets and produced decision-support reports for stakeholders.
- **Mentobile Technology:** Built backend modules in CodeIgniter (MVC), designed MySQL schemas and CRUD operations, and worked through Git branching, pull requests and code reviews.

</details>

---

## 🎓 Education & Training

- 🎓 **B.Tech, Computer Science & Engineering**, GLA University, Mathura (2020 – 2024)
- 🏅 **AWS & DevOps Infrastructure Training**, Croma Campus, NASSCOM-certified, Wipro Credential Partner (Sep 2025 – Mar 2026)

<details>
<summary><b>📚 Training coverage and other courses</b></summary>

- Linux administration, Git and GitHub workflows
- Jenkins CI/CD, GitHub Webhooks, Docker, Kubernetes
- AWS: EC2, S3, IAM, VPC, CloudWatch
- Terraform, Ansible, Prometheus, Grafana
- Web Development Bootcamp (JOVAC) · Front-End Development, HTML & CSS (Great Learning) · Course on Computer Concepts, CCC (NIELIT)

</details>

---

## 🌱 Currently Learning

- 🔨 Terraform: Infrastructure as Code on AWS
- ☸️ Advanced Kubernetes
- 🐧 Linux administration fundamentals

---

## 📊 GitHub Stats

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=PushpenderKumar7505&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PushpenderKumar7505&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=PushpenderKumar7505&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</div>

---

## 🤝 Let's Connect

I'm looking for **DevOps Engineer, Cloud Engineer, Cloud Support Engineer and Cloud Infrastructure Engineer** roles (fresher / 0–1 year). If your team needs someone who automates first and documents everything, let's talk.

<p align="center">
  <a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://cloud-devops-shine.lovable.app"><img src="https://img.shields.io/badge/Portfolio-Visit-0d1117?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-pushpender7505%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=120&color=0:2c5364,50:203a43,100:0f2027&section=footer" alt="Footer" />
