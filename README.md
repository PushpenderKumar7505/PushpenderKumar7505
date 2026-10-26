<div align="center">
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:00d9ff,100:0d1117&height=200&section=header&text=Pushpender%20Kumar&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=DevOps%20Engineer%20%7C%20Cloud%20Infrastructure%20%7C%20CI%2FCD%20Automator&descAlignY=60&descSize=18&descColor=00d9ff&animation=fadeIn"/>
</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1000&color=00D9FF&center=true&vCenter=true&width=700&lines=🚀+Automating+AWS+EC2+in+under+3+minutes...;⚙️+Jenkins+%7C+Ansible+%7C+Kubernetes+%7C+Terraform;🐳+Containers+%26+Pods+%7C+Zero+Manual+Steps;☁️+Cloud+Infrastructure+%7C+IaC+%7C+CI%2FCD+Pipelines;🔥+Turning+15-min+tasks+into+3-min+pipelines)](https://git.io/typing-svg)

</div>

---

<img align="right" alt="Coding GIF" width="340" src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif"/>

## `$ whoami`

```bash
Name     : Pushpender Kumar
Role     : DevOps Engineer (Fresher / Intern)
Location : Mathura → Gurugram, India 🇮🇳
Degree   : B.Tech CSE — GLA University (2024)
Status   : Actively Seeking Opportunities ✅
Belief   : "If I do it twice, I'll automate it."
```

<br>

- 🔥 &nbsp;Building **Jenkins + Ansible + K8s** CI/CD pipelines on **AWS**
- ⚡ &nbsp;Cut EC2 provisioning time: **15 min → under 3 min**
- 🌱 &nbsp;Levelling up in **Terraform IaC** & advanced **Kubernetes**
- 🤝 &nbsp;Open to collaborate on **DevOps & Cloud** projects
- 💬 &nbsp;Ask me about: `Jenkins` `AWS EC2` `Docker` `Kubernetes` `Ansible` `Linux`

<br clear="right"/>

---

## 🧰 Arsenal

<div align="center">

**⚙️ CI/CD & Automation**

![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)

**☁️ AWS Cloud**

![AWS EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![AWS S3](https://img.shields.io/badge/AWS_S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)
![AWS IAM](https://img.shields.io/badge/AWS_IAM-DD344C?style=for-the-badge&logo=amazon-aws&logoColor=white)
![AWS VPC](https://img.shields.io/badge/AWS_VPC-8C4FFF?style=for-the-badge&logo=amazon-aws&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazon-cloudwatch&logoColor=white)

**🐳 Containers & Orchestration**

![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=Kubernetes&logoColor=white)

**📦 IaC & Monitoring**

![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

**🖥️ Scripting & OS**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

**🔀 Version Control**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Bitbucket](https://img.shields.io/badge/Bitbucket-0052CC?style=for-the-badge&logo=bitbucket&logoColor=white)

**🧩 Backend & Database**

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![CodeIgniter](https://img.shields.io/badge/CodeIgniter-EF4223?style=for-the-badge&logo=codeIgniter&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

</div>

---

## 🚀 Projects That Actually Ship

<details open>
<summary><b>🔴 Project 1 — Full Stack CI/CD: Jenkins → Ansible → Kubernetes on AWS</b></summary>
<br>

> *"One GitHub push. Zero manual steps. Kubernetes pod up and running."*

```
GitHub Push ──► Jenkins Pipeline ──► SCP Transfer ──► Ansible SSH ──► K8s Pod ✅
     │               │                    │                 │               │
  Webhook        3 Stages            ec2.yml runs      pod.yml runs    ubuntu:latest
  Trigger    Auto checkout +      EC2 + SG + AMI     Multi-container   Status: Running
             file transfer         + Keypair          deployment       Confirmed kubectl
```

| What I Built | Impact |
|---|---|
| 3-stage Jenkins pipeline (Checkout → SCP Transfer → Remote Execute) | **100% automated** end-to-end |
| Ansible `ec2.yml` using `amazon.aws` collection | EC2 + Security Group + AMI + Keypair via code |
| Passwordless SSH between Ansible control node & K8s server | `ansible -m ping` → **0 failures** |
| K8s multi-container pod deployment via remote `pod.yml` trigger | Pods confirmed **Running** state |
| 3 EC2 instances managed in `ap-south-1` via MobaXterm | Jenkins (t3.micro) · Ansible (t3.micro) · K8s (c7i.flex.large) |

**Stack:** `Jenkins` `Ansible` `Kubernetes` `AWS EC2` `GitHub` `SSH` `SCP` `Linux Ubuntu`

</details>

---

<details open>
<summary><b>🟡 Project 2 — Automated AWS EC2 Provisioning via Jenkins CI/CD</b></summary>
<br>

> *"Manual clicking eliminated. 15 minutes became 3 minutes."*

```
Code Push ──► Webhook Fires ──► Jenkins Triggers ──► Bash Script Runs ──► EC2 Alive 🟢
    │               │                 │                     │                   │
  GitHub      Instant trigger    Parameterized job      AWS API calls      Auditable
  commit      on every push      version-controlled    IAM least-priv     deployment
```

| What I Built | Impact |
|---|---|
| Parameterized Bash scripts via Jenkins jobs | **Eliminated 100%** of manual console clicks |
| GitHub Webhooks → event-driven pipeline | Auto-triggers on every push across 2 repos |
| AWS IAM least-privilege policies on Ubuntu | Cloud security best practices enforced |
| End-to-end automated pipeline | **15 min → under 3 min** ⚡ provisioning time |

**Stack:** `Jenkins` `GitHub Webhooks` `AWS EC2` `AWS IAM` `Bash Scripting` `Linux Ubuntu`

</details>

---

## 📊 GitHub Stats

<div align="center">
  <img height="180em" src="https://github-readme-stats.shion.dev/api?username=PushpenderKumar7505&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=00d9ff&icon_color=00d9ff&text_color=ffffff"/>
  <img height="180em" src="https://github-readme-stats.shion.dev/api/top-langs/?username=PushpenderKumar7505&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d9ff&text_color=ffffff"/>
</div>

<div align="center">
  <img width="70%" src="https://streak-stats.demolab.com/?user=PushpenderKumar7505&theme=tokyonight&hide_border=true&background=0d1117&ring=00d9ff&fire=ff6b35&currStreakLabel=00d9ff"/>
</div>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=PushpenderKumar7505&theme=tokyonight&no-frame=true&column=7&margin-w=4"/>
</div>

---

## 💼 Work Experience

<table width="100%">
<tr>
<td width="50%" valign="top">

### 🏢 Mentobile Technology
**Backend Developer Intern**
`Jul 2024 – Oct 2024`

```
Stack: CodeIgniter PHP · MySQL · Git
```
- Built & maintained backend modules with **MVC** framework
- Designed MySQL schemas + full **CRUD** operations
- Git branching, PRs & code reviews in team workflow

</td>
<td width="50%" valign="top">

### 🏢 Precise Research Solution
**Market Research Associate · Gurugram**
`Jan 2025 – Jun 2025`

```
Stack: Data Analysis · Excel · Research
```
- Cleaned & analysed structured datasets
- Produced **decision-support reports** for stakeholders
- Synthesised multi-source findings for presentations

</td>
</tr>
</table>

---

## 🎓 Education & Certifications

```
🎓  B.Tech in Computer Science & Engineering
    GLA University, Mathura  ·  Jul 2020 – May 2024  ·  CGPA: 6.83 / 10.0

📜  AWS & DevOps Infrastructure Training — Croma Campus  (Sep 2025 – Mar 2026)
    ├── Linux Administration · Git & GitHub Workflows
    ├── Jenkins CI/CD · GitHub Webhooks · Docker · Kubernetes
    ├── AWS (EC2 · S3 · IAM · VPC · CloudWatch)
    ├── Terraform (IaC) · Ansible (Config Mgmt)
    └── Prometheus · Grafana (Monitoring & Observability)

📋  Other Certifications
    ├── Web Development Bootcamp — JOVAC
    ├── Front End Development (HTML & CSS) — Great Learning
    └── Course on Computer Concepts (CCC) — NIELIT
```

---

## 🌐 Find Me Here

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Pushpender_Kumar-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pushpender-kumar-5280b7226)
[![Gmail](https://img.shields.io/badge/Gmail-pushpender7505@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:pushpender7505@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-PushpenderKumar7505-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PushpenderKumar7505)

</div>

---

<div align="center">

### 🔝 Top Contributed Repos
![](https://github-contributor-stats.vercel.app/api?username=PushpenderKumar7505&limit=5&theme=tokyonight&combine_all_yearly_contributions=true&hide_border=true)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:00d9ff,100:0d1117&height=120&section=footer&animation=fadeIn"/>

> *"Automate everything. Deploy with confidence. Sleep at night."*
> — **Pushpender Kumar**

[![Profile Views](https://komarev.com/ghpvc/?username=PushpenderKumar7505&color=00d9ff&style=for-the-badge&label=PROFILE+VIEWS)](https://github.com/PushpenderKumar7505)

</div>
