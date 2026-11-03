<div align="center">

<img src="assets/header.svg" alt="Pushpender Kumar: DevOps and Cloud Engineer. Animated pipeline from GitHub to Jenkins, Ansible, AWS EC2 and Kubernetes" width="100%" />

<a href="https://github.com/PushpenderKumar7505">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=900&color=2DD4BF&center=true&vCenter=true&width=720&height=40&lines=DevOps+%26+Cloud+Engineer+%28Fresher%29;Jenkins+%C2%B7+Ansible+%C2%B7+Kubernetes+%C2%B7+AWS+EC2;git+push+%E2%86%92+Jenkins+%E2%86%92+Ansible+%E2%86%92+AWS+%2F+Kubernetes;Immediate+joiner+%C2%B7+Gurugram%2C+India" alt="Typing animation" />
</a>

<p>
  <img src="https://img.shields.io/badge/Status-Open%20to%20work-16a34a?style=flat-square" alt="Open to work" />
  <img src="https://img.shields.io/badge/Availability-Immediate%20joiner-0ea5e9?style=flat-square" alt="Immediate joiner" />
  <img src="https://img.shields.io/badge/Location-Gurugram%2C%20India-64748b?style=flat-square" alt="Gurugram, India" />
</p>

<p>
  <a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://cloud-devops-shine.lovable.app/"><img src="https://img.shields.io/badge/Portfolio-Visit-0d1117?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-pushpender7505%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

<sub>
<a href="#about">About</a> ·
<a href="#skills">Skills</a> ·
<a href="#featured-projects">Projects</a> ·
<a href="#experience">Experience</a> ·
<a href="#education">Education</a> ·
<a href="#analytics">Analytics</a> ·
<a href="#contact">Contact</a>
</sub>

</div>

<div align="center">
  <img src="assets/snapshot.svg" alt="Snapshot: 2 CI/CD projects, 3 EC2 nodes, 3 pipeline stages, 5 of 6 green builds" width="100%" />
</div>

<a id="about"></a>
<img src="assets/sec-about.svg" alt="About" width="100%" />

I am a fresher DevOps and Cloud engineer (B.Tech CSE, 2024) who learns by building and documenting. My hands-on work is **CI/CD automation on AWS**: Jenkins pipelines that are triggered by GitHub webhooks, Ansible playbooks that create AWS EC2 infrastructure, and a Kubernetes (minikube) pod deployed from code.

| | |
|---|---|
| **What I have built** | Two Jenkins CI/CD projects on AWS EC2 (see [Featured Projects](#featured-projects)) |
| **How my automation works** | `git push` → GitHub webhook → Jenkins 3-stage pipeline → `scp` + `ssh` to an Ansible server → playbook creates EC2 resources or deploys a Kubernetes pod |
| **Core tools** | Jenkins, Ansible, AWS EC2, Kubernetes + kubectl, Git/GitHub, Linux (Ubuntu) |
| **Training in progress** | Terraform, advanced Kubernetes, Linux administration, monitoring with Prometheus and Grafana |
| **Seeking** | Entry-level DevOps / Cloud roles in Delhi NCR, Noida, Pune or remote |

> Every project below is a **lab / training project** built on my own AWS account. The details shown come from the repositories and their screenshots.

<a id="roles"></a>
<img src="assets/sec-roles.svg" alt="Open to Roles" width="100%" />

`DevOps Engineer (Fresher)` · `AWS Cloud Engineer` · `Junior Cloud Engineer` · `Cloud Infrastructure Engineer` · `DevOps Trainee` · `Cloud Support Associate` · `Junior Site Reliability Engineer`

<a id="skills"></a>
<img src="assets/sec-skills.svg" alt="Skills" width="100%" />

Grouped by how I have actually used each tool, so you can judge depth quickly.

### ✅ Hands-on (used in my projects)

<div align="center">
  <img src="https://skillicons.dev/icons?i=aws,jenkins,ansible,kubernetes,git,github,linux,ubuntu&theme=dark" alt="Hands-on skills: AWS, Jenkins, Ansible, Kubernetes, Git, GitHub, Linux, Ubuntu" />
</div>

| Area | What I have done with it |
|---|---|
| **AWS** | Launched and managed EC2 instances, security groups, key pairs and subnets; attached an IAM role so the Ansible server needs no stored access keys |
| **Jenkins** | Installed on EC2; built 3-stage Pipeline jobs; `sshagent` credentials; GitHub webhook trigger |
| **Ansible** | Playbooks using the `amazon.aws` collection and the `k8s` module; passwordless SSH to managed nodes; `ansible -m ping` checks |
| **Kubernetes** | Single-node minikube on EC2; deployed a two-container pod and verified it with `kubectl` |
| **Git / GitHub** | Clone, commit, push, webhooks |
| **Linux (Ubuntu)** | Server setup and SSH-based administration |

### 📘 Training-level (course and labs, not yet in a deployed project)

<div align="center">
  <img src="https://skillicons.dev/icons?i=docker,terraform,bash,prometheus,grafana&theme=dark" alt="Training-level skills: Docker, Terraform, Bash, Prometheus, Grafana" />
</div>

Docker · Terraform · Bash scripting · Prometheus · Grafana · AWS S3, VPC and CloudWatch

### 🌱 Currently learning

Terraform on AWS (building hands-on projects) · Advanced Kubernetes · Linux administration fundamentals

### 🗂️ Prior backend experience (internship)

<div align="center">
  <img src="https://skillicons.dev/icons?i=php,codeigniter,mysql&theme=dark" alt="Backend: PHP, CodeIgniter, MySQL" />
</div>

<a id="featured-projects"></a>
<img src="assets/sec-projects.svg" alt="Featured Projects" width="100%" />

### 1️⃣ AWS Resource Provisioning via Jenkins, Ansible and Kubernetes CI/CD

[![Repository](https://img.shields.io/badge/Repository-Devops--automation--jenkins--ansible-181717?style=flat-square&logo=github)](https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible)

**Overview.** A three-server CI/CD lab on AWS. A GitHub push triggers Jenkins, Jenkins hands the playbooks to an Ansible server, and Ansible either provisions an EC2 instance (`ec2.yml`) or deploys a Kubernetes pod (`pod1.yml`). Two Jenkins pipeline jobs follow the same 3-stage pattern.

**Technical problem it addresses.** Creating cloud resources and deploying workloads by hand in the console or terminal is slow, easy to get wrong and hard to repeat. Here the steps live in version-controlled playbooks and run the same way every time.

**Stack:** `Jenkins` `GitHub Webhooks` `Ansible` `amazon.aws` `AWS EC2` `Kubernetes (minikube)` `kubectl` `SSH/SCP` `Ubuntu`

#### End-to-end architecture

```mermaid
flowchart LR
    DEV(["Developer<br/>git push"]) --> GH["GitHub repository<br/>ec2.yml, pod1.yml"]
    GH -->|"webhook on push"| JEN["Jenkins<br/>3-stage pipeline"]
    JEN -->|"scp playbooks<br/>ssh via sshagent"| ANS["Ansible server"]
    ANS -->|"ec2.yml"| EC2["New EC2 instance<br/>+ security group"]
    ANS -->|"pod1.yml over SSH"| K8S["Kubernetes node<br/>minikube"]
    K8S --> POD["Pod with 2 containers<br/>Running"]

    classDef src fill:#24292f,stroke:#9ca3af,color:#fff
    classDef ci fill:#d24939,stroke:#fff,color:#fff
    classDef cm fill:#ee0000,stroke:#fff,color:#fff
    classDef aws fill:#ff9900,stroke:#fff,color:#000
    classDef k8s fill:#326ce5,stroke:#fff,color:#fff
    class DEV,GH src
    class JEN ci
    class ANS cm
    class EC2 aws
    class K8S,POD k8s
```

#### AWS infrastructure

```mermaid
flowchart TB
    ADMIN["Admin workstation<br/>MobaXterm SSH"]
    GH["GitHub<br/>webhook"]

    subgraph AWS["AWS Cloud"]
        direction TB
        subgraph MUM["ap-south-1 (Mumbai): CI/CD lab"]
            direction LR
            JEN["Jenkins server<br/>EC2 t3.micro<br/>port 8080"]
            ANS["Ansible server<br/>EC2 t3.micro<br/>IAM role attached"]
            K8S["Kubernetes server<br/>EC2 c7i.flex.large<br/>minikube"]
        end
        subgraph ORE["us-west-2: region set in ec2.yml"]
            direction LR
            SG["Security group<br/>SSH port 22"]
            NEW["Provisioned EC2<br/>t3.micro"]
            SG --- NEW
        end
    end

    GH -->|"HTTP webhook"| JEN
    ADMIN -.->|"SSH"| JEN
    ADMIN -.->|"SSH"| ANS
    ADMIN -.->|"SSH"| K8S
    JEN -->|"scp + ssh"| ANS
    ANS -->|"passwordless SSH"| K8S
    ANS -->|"EC2 API via amazon.aws"| SG
```

<details>
<summary><b>🔍 More architecture diagrams: Jenkins pipeline, Ansible, Kubernetes, sequence, components</b></summary>

#### Jenkins pipeline execution

```mermaid
flowchart TD
    T(["Trigger<br/>GitHub webhook on push"]) --> S1

    subgraph PIPE["Pipeline script (node block)"]
        direction TB
        S1["Stage 1: Github connect<br/>check out the repository"] --> S2
        S2["Stage 2: ansible-server<br/>sshagent + scp playbooks to Ansible server"] --> S3
        S3["Stage 3: ansible deploy<br/>ssh to Ansible server, run ansible-playbook"]
    end

    S3 --> OK{"Exit code 0?"}
    OK -->|"yes"| GREEN(["Build SUCCESS"])
    OK -->|"no"| RED(["Build FAILURE<br/>read console output and fix"])
```

#### Ansible automation workflow

```mermaid
flowchart LR
    subgraph ANS["Ansible server"]
        direction TB
        EC2YML["ec2.yml<br/>hosts: localhost"]
        PODYML["pod1.yml<br/>hosts: all"]
    end

    EC2YML --> T1["ec2_group<br/>create security group"] --> T2["ec2_instance<br/>launch and wait"]
    T2 -.->|"amazon.aws + boto3<br/>IAM role credentials"| API[("AWS EC2 API")]
    PODYML -->|"SSH key auth"| T4["k8s module<br/>apply Pod definition"] --> T5["Pod created on the node"]
```

#### Kubernetes deployment workflow

```mermaid
flowchart TB
    A["Ansible server<br/>ansible-playbook pod1.yml"] -->|"SSH"| B["Kubernetes node (minikube)"]
    B --> C["k8s module applies the Pod<br/>name: croma-pod, namespace: default"]
    C --> D["Scheduler assigns the pod to the node"]
    D --> E["kubelet pulls ubuntu:latest"]
    E --> F["Container 1 started"]
    E --> G["Container 2 started"]
    F --> H{{"Verify with kubectl get pods and describe"}}
    G --> H
    H --> I(["Pod Ready, both containers Running"])
```

#### Provisioning sequence

```mermaid
sequenceDiagram
    autonumber
    actor Dev as Developer
    participant GH as GitHub
    participant J as Jenkins
    participant A as Ansible server
    participant AWS as AWS EC2 API
    participant K as Kubernetes node

    Dev->>GH: git push to main
    GH->>J: Webhook (push event)
    J->>GH: Stage 1: check out repository
    J->>A: Stage 2: scp playbooks (sshagent)
    J->>A: Stage 3: ssh, run ansible-playbook
    alt Job Aws-project runs ec2.yml
        A->>AWS: Create security group
        A->>AWS: Launch EC2 instance and wait
        AWS-->>A: Instance running
    else Job Kubernetes-project runs pod1.yml
        A->>K: SSH, apply Pod definition
        K-->>A: Pod created
    end
    A-->>J: PLAY RECAP and exit code
    Note over J: Build marked SUCCESS or FAILURE
```

#### Component interaction

```mermaid
flowchart LR
    subgraph SRC["Source control"]
        REPO["GitHub repository<br/>playbooks and docs"]
        HOOK["Webhook<br/>/github-webhook/"]
    end
    subgraph CI["Jenkins server"]
        JOB["Pipeline jobs<br/>Aws-project<br/>Kubernetes-project"]
        CRED["SSH credential<br/>ID: ansible"]
        PLG["Plugins<br/>Git, Pipeline, GitHub, SSH Agent"]
    end
    subgraph CM["Ansible server"]
        PB["Playbooks<br/>ec2.yml, pod1.yml"]
        COL["amazon.aws collection<br/>boto3 / botocore"]
        ROLE["IAM role<br/>EC2 permissions"]
    end
    subgraph TGT["Targets"]
        EC2API["AWS EC2 API"]
        KN["Kubernetes node<br/>minikube + kubectl"]
    end

    REPO --- HOOK
    HOOK -->|"push event"| JOB
    PLG -.-> JOB
    CRED -.->|"sshagent"| JOB
    JOB -->|"scp + ssh"| PB
    PB --> COL
    ROLE -.->|"credentials"| COL
    COL -->|"API calls"| EC2API
    PB -->|"SSH key auth"| KN
```

</details>

#### What was verified

| Check | Evidence |
|---|---|
| 3 EC2 instances running (Jenkins, Ansible, Kubernetes) | AWS console screenshot in the repository |
| Passwordless SSH from Ansible server to the managed node | `ansible all -m ping` returned `"ping": "pong"` |
| Pod deployed on minikube and healthy | `kubectl describe pod` shows the pod scheduled to `minikube`, both containers `Running`, conditions `Ready: True` |
| Pipeline pattern | Jenkins job configuration screenshots (3 stages: checkout, scp, `ansible-playbook`) |

<details>
<summary><b>Setup prerequisites</b></summary>

<br>

- **3 Ubuntu EC2 instances:** Jenkins, Ansible control node, Kubernetes node (minikube + `kubectl`)
- **Jenkins:** plugins Git, Pipeline, GitHub, SSH Agent; credential of type *SSH Username with private key* (ID `ansible`, user `ubuntu`)
- **Ansible server:** Ansible, `amazon.aws` collection, `python3-boto3` and `python3-botocore`, plus an IAM role with EC2 permissions attached to the instance (no access keys stored on disk)
- **Kubernetes node:** reachable from the Ansible server over SSH with key-based login (public key in `authorized_keys`)
- **Network:** Jenkins port `8080` open for the GitHub webhook; SSH `22` between the servers
- **Inventory note:** `pod1.yml` uses `hosts: all`, so the Ansible inventory must contain only the Kubernetes node (or run with `--limit`)

</details>

<details>
<summary><b>Installation and execution</b></summary>

<br>

1. Create the three EC2 instances and install Jenkins, Ansible and minikube.
2. Generate an SSH key pair, add the public key to the managed node's `authorized_keys`, and add the private key to Jenkins as credential `ansible`.
3. Verify connectivity from the Ansible server:
   ```bash
   ansible all -m ping
   ```
4. Create a Jenkins Pipeline job with the 3 stages below and enable the *GitHub hook trigger for GITScm polling*.
5. In the GitHub repository add the webhook `http://<jenkins-public-ip>:8080/github-webhook/` (`application/json`, push event).
6. Push a commit to `main` and watch the build in Jenkins.

```groovy
node {
    stage('Github connect') {
        git branch: 'main', url: 'https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible.git'
    }
    stage('ansible-server') {
        sshagent(['ansible']) {
            sh 'scp <workspace-path>/* ubuntu@<ansible-private-ip>:/home/ubuntu'
        }
    }
    stage('ansible deploy') {
        sshagent(['ansible']) {
            sh 'ssh ubuntu@<ansible-private-ip> ansible-playbook <playbook>.yml'
        }
    }
}
```

**Validation commands**

```bash
ansible all -m ping          # connectivity: expect "ping": "pong"
kubectl get pods             # on the Kubernetes node: pod listed as Running
kubectl describe pod <name>  # both containers Running, Ready: True
```

</details>

<details>
<summary><b>Project structure</b></summary>

```text
Devops-automation-jenkins-ansible/
├── README.md              # project documentation
├── ec2.yml                # Ansible: security group + EC2 instance (amazon.aws)
├── pod1.yml               # Ansible: two-container Kubernetes pod (k8s module)
└── *.png                  # 12 screenshots (Jenkins, Ansible, kubectl, AWS console)
```

</details>

<details>
<summary><b>Limitations and future improvements</b></summary>

<br>

- Security group in `ec2.yml` allows SSH from `0.0.0.0/0`. Next step: restrict it to a trusted CIDR.
- `ec2.yml` targets `us-west-2` while the CI/CD servers run in `ap-south-1`. Next step: make region, AMI, key and subnet variables.
- Pipeline scripts for this project are configured inside Jenkins. Next step: commit a `Jenkinsfile` (as done in project 2) so the pipeline itself is version-controlled.
- The pod runs `sleep` placeholder containers. Next step: deploy a real application image with a Deployment and Service.
- Next steps on my roadmap: Terraform for the AWS layer, Ansible roles and Vault, Prometheus and Grafana monitoring, HTTPS for Jenkins.

</details>

<img src="assets/divider.svg" alt="" width="100%" />

### 2️⃣ Automated AWS EC2 Provisioning via Jenkins CI/CD

[![Repository](https://img.shields.io/badge/Repository-Jenkins--ansible--aws--ec2--provisioning-181717?style=flat-square&logo=github)](https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning)

**Overview.** A GitHub push triggers the Jenkins job `Aws-project`. Its `Jenkinsfile` (stored in the repository) copies `ec2.yml` to an Ansible server and runs it, which creates a security group and an EC2 instance. No AWS console clicks are needed for provisioning.

**Stack:** `Jenkins` `GitHub Webhooks` `Ansible` `amazon.aws` `AWS EC2` `AWS IAM role` `Groovy` `YAML` `Ubuntu`

```mermaid
flowchart LR
    GH["GitHub repository<br/>Jenkinsfile + ec2.yml"] -->|"webhook on push"| J["Jenkins<br/>job Aws-project"]
    J -->|"scp ec2.yml<br/>ssh via sshagent"| A["Ansible server<br/>ap-south-1"]
    A -->|"ansible-playbook ec2.yml"| API["AWS EC2 API"]
    API --> SG["Security group<br/>SSH port 22"]
    API --> EC2["EC2 instance<br/>t3.micro"]
```

#### Before vs after

```mermaid
flowchart LR
    subgraph BEFORE["Before: manual"]
        direction TB
        M1["Sign in to AWS console"] --> M2["Create security group"] --> M3["Choose AMI, type, key pair, subnet"] --> M4["Launch and verify by hand"]
    end
    subgraph AFTER["After: pipeline"]
        direction TB
        A1["git push"] --> A2["Webhook triggers Jenkins"] --> A3["Playbook copied to Ansible server"] --> A4["ec2.yml creates security group and instance"]
    end
    BEFORE ==> AFTER
```

| Topic | Detail |
|---|---|
| **Jenkins job** | `Aws-project`, Pipeline script from SCM (`Jenkinsfile`), 3 stages: `Github connect`, `ansible-server`, `ansible deploy` |
| **Build history** | 6 builds: #1 failed, #2 to #6 successful (last build about 18 seconds) |
| **GitHub webhook** | `/github-webhook/`, `application/json`, push event; GitHub shows "Last delivery was successful" |
| **AWS IAM** | IAM role with EC2 permissions attached to the Ansible server, so no access keys are stored on it |
| **EC2 provisioning** | `amazon.aws.ec2_group` then `amazon.aws.ec2_instance` (`wait: yes`), then a `debug` task prints the new instance ID and state |
| **Validation** | `ansible -m ping` returns `pong`; Jenkins dashboard shows the job green; webhook delivery succeeded |

<details>
<summary><b>Limitations of this lab setup</b></summary>

<br>

SSH open to `0.0.0.0/0` on the created security group · `StrictHostKeyChecking=no` in the pipeline · Jenkins on plain HTTP · playbook region (`us-west-2`) differs from the CI/CD servers (`ap-south-1`). Documented in the repository with the planned hardening steps.

</details>

<a id="experience"></a>
<img src="assets/sec-experience.svg" alt="Experience" width="100%" />

| Role | Organisation | Period |
|---|---|---|
| **Associate, FTH** (Incident Response) | UnitedLex India, Gurugram | Jul 2026 |
| **Market Research Associate Intern** | Precise Research Solutions, Gurugram | Jan 2025 – Jun 2025 |
| **Backend Developer Intern** | Mentobile Technologies | Jul 2024 – Oct 2024 |

- **UnitedLex:** Investigated data breaches and classified PII/PHI in affected datasets using Relativity and Microsoft 365.
- **Precise Research Solutions:** Cleaned and analysed structured datasets and produced decision-support reports for stakeholders.
- **Mentobile Technologies:** Built backend modules in CodeIgniter (MVC), designed MySQL schemas and CRUD operations, and worked with Git branching, pull requests and code reviews.

<a id="education"></a>
<img src="assets/sec-education.svg" alt="Education and Training" width="100%" />

- 🎓 **B.Tech, Computer Science & Engineering**, GLA University, Mathura (2020 – 2024)
- 🏅 **AWS & DevOps Infrastructure Training**, Croma Campus (NASSCOM-certified, Wipro Credential Partner), Sep 2025 – Mar 2026
- 📚 Also completed: Web Development Bootcamp (JOVAC) · Front-End Development, HTML & CSS (Great Learning) · Course on Computer Concepts, CCC (NIELIT)

<a id="analytics"></a>
<img src="assets/sec-analytics.svg" alt="GitHub Analytics" width="100%" />

These cards are generated live from my public GitHub activity.

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=PushpenderKumar7505&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PushpenderKumar7505&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=PushpenderKumar7505&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=PushpenderKumar7505&theme=tokyo-night&hide_border=true" alt="Contribution activity graph" width="100%" />
</div>

#### Repository highlights

<div align="center">
  <a href="https://github.com/PushpenderKumar7505/Devops-automation-jenkins-ansible"><img src="https://github-readme-stats.vercel.app/api/pin/?username=PushpenderKumar7505&repo=Devops-automation-jenkins-ansible&theme=tokyonight&hide_border=true" alt="Devops-automation-jenkins-ansible" /></a>
  <a href="https://github.com/PushpenderKumar7505/Jenkins-ansible-aws-ec2-provisioning"><img src="https://github-readme-stats.vercel.app/api/pin/?username=PushpenderKumar7505&repo=Jenkins-ansible-aws-ec2-provisioning&theme=tokyonight&hide_border=true" alt="Jenkins-ansible-aws-ec2-provisioning" /></a>
</div>

<a id="contact"></a>
<img src="assets/sec-contact.svg" alt="Contact" width="100%" />

I am looking for an entry-level **DevOps / AWS Cloud / Cloud Infrastructure** role where I can keep automating and documenting. Available to join immediately.

<div align="center">
  <a href="https://www.linkedin.com/in/pushpender-kumar-5280b7226/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://cloud-devops-shine.lovable.app/"><img src="https://img.shields.io/badge/Portfolio-Visit-0d1117?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="mailto:pushpender7505@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20hello-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=100&color=0:134e5e,50:0f2a3a,100:0b1220&section=footer" alt="" />
