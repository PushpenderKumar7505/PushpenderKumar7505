<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:00d9ff,100:0d1117&height=220&section=header&text=Pushpender%20Kumar&fontSize=58&fontColor=ffffff&fontAlignY=38&desc=DevOps%20%7C%20AWS%20Cloud%20%7C%20CI%2FCD%20Automation&descAlignY=60&descSize=20&descColor=00d9ff&animation=fadeIn" width="100%" alt="Pushpender Kumar header" />

<a href="https://github.com/PushpenderKumar7505"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&duration=3200&pause=1000&color=00D9FF&center=true&vCenter=true&width=700&height=40&lines=CI%2FCD+automation+with+Jenkins+%2B+GitHub+webhooks;Infrastructure+provisioning+with+Ansible+on+AWS+EC2;Kubernetes+deployments+verified+with+kubectl;Open+to+DevOps+and+Cloud+roles+in+Delhi+NCR+and+Remote" alt="Typing animation" /></a>

<br/>

<img src="https://img.shields.io/badge/Role-DevOps%20%7C%20AWS%20Cloud%20Engineer-00d9ff?style=for-the-badge&logo=amazonaws&logoColor=white&labelColor=0d1117" alt="Role" />
<img src="https://img.shields.io/badge/Location-Gurugram%2C%20India-ff6b35?style=for-the-badge&logo=googlemaps&logoColor=white&labelColor=0d1117" alt="Location" />
<img src="https://img.shields.io/badge/Status-Open%20to%20Work-2ea44f?style=for-the-badge&logo=checkmarx&logoColor=white&labelColor=0d1117" alt="Open to work" />

<br/><br/>

<a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://cloud-devops-shine.lovable.app/"><img src="https://img.shields.io/badge/Portfolio-Visit-8A2BE2?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
<a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

---

## 👨‍💻 About Me

```yaml
name:       Pushpender Kumar
role:       DevOps Engineer | AWS Cloud Engineer (Fresher)
location:   Gurugram, Haryana, India   # originally from Mathura, UP
education:  B.Tech CSE, GLA University (2024)
training:   AWS & DevOps Infrastructure, Croma Campus (NASSCOM) | Sep 2025 - Mar 2026
looking_for:
  - Junior DevOps Engineer
  - AWS Cloud Engineer
  - Cloud Infrastructure Engineer
  - Cloud Support Engineer
  - Junior SRE
work_mode:  Delhi NCR | Gurugram | Noida | Remote
available:  Immediately
```

I am a B.Tech Computer Science graduate focused on DevOps and AWS cloud infrastructure. After my AWS and DevOps training, I built two CI/CD projects on my own AWS account: Jenkins pipelines triggered by GitHub webhooks, Ansible playbooks that create EC2 resources, and a Kubernetes pod deployed from code and verified with `kubectl`.

My earlier experience is in backend development and operations support. My DevOps experience comes from training and the lab projects below.

> 💡 **Engineering approach:** automate what is repeatable, verify every step, and document the result so someone else can reproduce it.

---

## 🧰 Tech Stack

<div align="center">

**Hands-on (used in my projects)**

<img src="https://skillicons.dev/icons?i=aws,jenkins,ansible,kubernetes,git,github,linux,ubuntu&theme=dark" alt="Hands-on skills" />

**Training and foundational**

<img src="https://skillicons.dev/icons?i=terraform,docker,bash,python,prometheus,grafana&theme=dark" alt="Foundational skills" />

**Previous backend experience**

<img src="https://skillicons.dev/icons?i=php,codeigniter,mysql&theme=dark" alt="Backend skills" />

</div>

| Area | What I have done |
|---|---|
| ☁️ **AWS** | EC2, security groups, key pairs, subnets, IAM role on the Ansible server; S3, VPC, CloudWatch at training level |
| 🔄 **CI/CD** | Jenkins Pipeline jobs, `sshagent` credentials, GitHub webhooks |
| ⚙️ **Automation** | Ansible playbooks (`amazon.aws`, `k8s`), passwordless SSH, `ansible -m ping` |
| 🐳 **Containers** | minikube on EC2, two-container pod, `kubectl` verification; Docker at lab level |
| 🐧 **Linux** | Ubuntu servers administered over SSH |

---

## 🚀 Featured Projects

<div align="center">

<a href="https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=PushpenderKumar7505&repo=Devops-automation-jenkins-ansible&theme=tokyonight&bg_color=0d1117&title_color=00d9ff&icon_color=00d9ff&text_color=ffffff&border_color=30363d" alt="Devops-automation-jenkins-ansible" />
</a>
<a href="https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=PushpenderKumar7505&repo=Jenkins-ansible-aws-ec2-provisioning&theme=tokyonight&bg_color=0d1117&title_color=00d9ff&icon_color=00d9ff&text_color=ffffff&border_color=30363d" alt="Jenkins-ansible-aws-ec2-provisioning" />
</a>

</div>

### 🔴 1. AWS Provisioning via Jenkins, Ansible and Kubernetes CI/CD

📂 [`Devops-automation-jenkins-ansible`](https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible)

**Problem:** creating cloud resources and deploying workloads by hand is slow, error-prone and hard to repeat.
**Solution:** a three-server AWS lab. A GitHub push triggers Jenkins, Jenkins copies playbooks to an Ansible server, and Ansible either provisions an EC2 instance (`ec2.yml`) or deploys a Kubernetes pod (`pod1.yml`).

`Jenkins` `GitHub Webhooks` `Ansible` `AWS EC2` `Kubernetes (minikube)` `kubectl` `SSH/SCP` `Ubuntu`

```mermaid
flowchart LR
    DEV(["👨‍💻 git push"]) --> GH["GitHub"]
    GH -->|webhook| JEN["Jenkins<br/>3-stage pipeline"]
    JEN -->|"scp + ssh"| ANS["Ansible server"]
    ANS -->|"ec2.yml"| EC2["☁️ EC2 + Security Group"]
    ANS -->|"pod1.yml"| K8S["☸️ Kubernetes pod<br/>2 containers"]

    classDef default fill:#0f2236,stroke:#38bdf8,color:#e2e8f0
    classDef aws fill:#0f2236,stroke:#ff9900,color:#e2e8f0
    class EC2 aws
```

| Component | Implementation |
|---|---|
| **Jenkins pipeline** | 3 stages: `Github connect` → `ansible-server` (scp via `sshagent`) → `ansible deploy` |
| **EC2 provisioning** | `amazon.aws.ec2_group` and `amazon.aws.ec2_instance` create a security group and instance |
| **Security** | IAM role attached to the Ansible server, so no AWS keys are stored on it |
| **Kubernetes** | `pod1.yml` applies a two-container Pod with the `k8s` module on minikube |
| **Verification** | `ansible all -m ping` returns `pong`; `kubectl get pods` shows the pod Running |

<details>
<summary><b>🔎 Limitations and next steps</b></summary>

- SSH is open to `0.0.0.0/0` on the created security group; restrict to a trusted CIDR.
- `ec2.yml` targets `us-west-2` while servers run in `ap-south-1`; move region, AMI and key into variables.
- Commit a `Jenkinsfile` for this project, as done in project 2.
- Pod runs `sleep` placeholder containers; replace with a real app and a Deployment.

</details>

### 🟡 2. Automated AWS EC2 Provisioning via Jenkins CI/CD

📂 [`Jenkins-ansible-aws-ec2-provisioning`](https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning)

A GitHub push triggers the Jenkins job `Aws-project`. Its `Jenkinsfile`, stored in the repo, copies `ec2.yml` to an Ansible server and runs it to create a security group and an EC2 instance, with no AWS console steps.

`Jenkins` `GitHub Webhooks` `Ansible` `AWS EC2` `IAM Role` `Groovy` `YAML`

```mermaid
flowchart LR
    subgraph BEFORE["❌ Before: manual"]
        direction TB
        M1["Sign in to console"] --> M2["Create security group"] --> M3["Pick AMI, type, key"] --> M4["Launch and verify by hand"]
    end
    subgraph AFTER["✅ After: pipeline"]
        direction TB
        A1["git push"] --> A2["Webhook triggers Jenkins"] --> A3["Playbook copied to Ansible"] --> A4["ec2.yml creates infra"]
    end
    BEFORE ==> AFTER
```

**Result:** 6 builds (#1 failed, #2 to #6 successful, last build about 18 seconds). Hardening steps are documented in the repository.

---

## 📚 All Repositories

| | Repository | Description | Stack |
|:-:|---|---|---|
| ☁️ | [Devops-automation-jenkins-ansible](https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible) | CI/CD pipeline that provisions EC2 and deploys a Kubernetes pod via webhooks | Jenkins · Ansible · K8s · AWS |
| ☁️ | [Jenkins-ansible-aws-ec2-provisioning](https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning) | Webhook-triggered Jenkinsfile pipeline creating EC2 with Ansible | Jenkins · Ansible · AWS |
| 🧩 | [CodeIgnitier-3-](https://github.com/PushpenderKumar7505/CodeIgnitier-3-) | PHP MVC internship project with CRUD and MySQL | PHP · CodeIgniter 3 · MySQL |
| 🧩 | [Basic_project_CI-3](https://github.com/PushpenderKumar7505/Basic_project_CI-3) | Basic starter project with CodeIgniter 3 | PHP · CodeIgniter 3 |
| 🗳️ | [E-Voting-Machine](https://github.com/PushpenderKumar7505/E-Voting-Machine) | E-voting application using blockchain | PHP |
| 🐍 | [pyhton-programming](https://github.com/PushpenderKumar7505/pyhton-programming) | Python practice programs | Python |
| 📝 | [question1](https://github.com/PushpenderKumar7505/question1) | Practice exercise | - |

🔗 Full list: [github.com/PushpenderKumar7505?tab=repositories](https://github.com/PushpenderKumar7505?tab=repositories)

---

## 💼 Experience

| Role | Organisation | Location | Period |
|---|---|---|---|
| **Associate, FTH (Incident Response)** · Contract | UnitedLex India | Gurugram | Jul 2026 |
| **Market Research Associate Intern** | Precise Research Solutions | Gurugram | Jan 2025 – Jun 2025 |
| **Backend Developer Intern** | Mentobile Technologies | India | Jul 2024 – Oct 2024 |

- **UnitedLex:** investigated data breaches and classified PII/PHI in affected datasets using Relativity and Microsoft 365.
- **Precise Research Solutions:** cleaned and analysed structured datasets; produced decision-support reports.
- **Mentobile Technologies:** built CodeIgniter (MVC) modules, designed MySQL schemas and CRUD operations; worked with Git branching, pull requests and code reviews.

---

## 🎓 Education and Training

- 🎓 **B.Tech, Computer Science and Engineering**: GLA University, Mathura (2020 – 2024)
- 📜 **AWS and DevOps Infrastructure Training**: Croma Campus, NASSCOM-certified, Wipro Credential Partner (Sep 2025 – Mar 2026)
- 📋 **Other:** Web Development Bootcamp (JOVAC) · Front End Development (Great Learning) · CCC (NIELIT)

---

## 🗺️ Learning Roadmap

```mermaid
flowchart LR
    A["✅ Jenkins + Ansible + EC2"] --> B["🔄 Terraform / IaC"] --> C["☸️ Kubernetes Deployments"] --> D["☁️ AWS VPC, IAM, S3"] --> E["📊 Prometheus + Grafana"]
```

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=PushpenderKumar7505&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d9ff&icon_color=00d9ff" width="49%" alt="GitHub stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=PushpenderKumar7505&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d9ff" width="49%" alt="Top languages" />

<img src="https://streak-stats.demolab.com?user=PushpenderKumar7505&theme=tokyonight&hide_border=true&background=0d1117&ring=00d9ff&fire=ff6b35&currStreakLabel=00d9ff" width="100%" alt="Contribution streak" />

</div>

---

## 📫 Let's Connect

<div align="center">

I am open to **Junior DevOps**, **AWS Cloud**, **Cloud Infrastructure**, **Cloud Support** and **Junior SRE** roles.
📍 **Gurugram, Haryana, India** · Delhi NCR · Noida · Remote · Can join immediately

<a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://github.com/PushpenderKumar7505"><img src="https://img.shields.io/badge/GitHub-PushpenderKumar7505-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://cloud-devops-shine.lovable.app/"><img src="https://img.shields.io/badge/Portfolio-Visit-8A2BE2?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
<a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

<br/><br/>

*"Automate everything. Verify every step. Document the result."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:00d9ff,100:0d1117&height=120&section=footer" width="100%" alt="footer" />

</div>
