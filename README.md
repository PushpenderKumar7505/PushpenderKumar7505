<h1 align="center">Pushpender Kumar</h1>

<p align="center">
  <b>Cloud & DevOps Engineer &nbsp;|&nbsp; AWS &nbsp;|&nbsp; Kubernetes &nbsp;|&nbsp; CI/CD &nbsp;|&nbsp; IaC &nbsp;|&nbsp; Monitoring</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/pushpender-kumar-5280b7226">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:pushpender7505@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://github.com/PushpenderKumar7505">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <img src="https://komarev.com/ghpvc/?username=PushpenderKumar7505&color=0e75b6&style=for-the-badge&label=PROFILE+VIEWS"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=16&pause=900&color=0E75B6&center=true&vCenter=true&width=750&lines=Jenkins+%7C+Ansible+%7C+Kubernetes+%7C+Terraform+%7C+AWS;15+min+EC2+provisioning+%E2%86%92+under+3+min+via+Jenkins;Zero+manual+steps.+Full+pipeline.+Production-ready.;Open+to+Cloud+%7C+DevOps+%7C+SRE+%7C+Platform+Engineer+roles"/>
</p>

---

## About Me

```yaml
name      : Pushpender Kumar
location  : Mathura / Gurugram, India
education : B.Tech CSE — GLA University (2024)
training  : AWS & DevOps — Croma Campus (Sep 2025 – Mar 2026)
seeking   : Cloud Engineer | DevOps Engineer | SRE | Platform Engineer | Fresher/Intern
available : Immediately
```

- Built **end-to-end Jenkins → Ansible → Kubernetes** CI/CD pipelines on AWS from scratch
- Cut EC2 provisioning time from **15 minutes to under 3 minutes** via automated Jenkins pipelines
- Hands-on with **Terraform IaC**, **Ansible playbooks**, **Docker**, **Kubernetes**, **Prometheus + Grafana**
- Daily driver: **Linux (Ubuntu)**, Bash scripting, Git-based workflows
- Looking for roles in: `Cloud Engineering` `DevOps` `SRE` `Platform Engineering` `Infrastructure`

---

## Skill Map

```
  CI/CD & AUTOMATION          CLOUD (AWS)                CONTAINERS & ORCHESTRATION
  ──────────────────          ───────────                ──────────────────────────
  Jenkins                     EC2  S3  IAM               Docker
  GitHub Actions              VPC  CloudWatch             Kubernetes (Pods, Deployments,
  Ansible Playbooks           Security Groups             Services, ReplicaSets)
  GitHub Webhooks             ap-south-1 region           kubectl

  INFRA AS CODE               MONITORING                 OS & SCRIPTING
  ─────────────               ──────────                 ──────────────
  Terraform                   Prometheus                 Linux (Ubuntu)
  .tf modules                 Grafana                    Bash / Shell Scripting
  State Management            Metrics & Dashboards       Python
                                                         Git / GitHub / Bitbucket
```

---

## Tech Stack

<p align="center">

<img src="https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
<img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white"/>
<img src="https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white"/>
<img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white"/>
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
<img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>

</p>

---

## Projects

### Project 1 — Jenkins + Ansible + Kubernetes CI/CD Pipeline on AWS

> *One GitHub push triggers a full 3-tier pipeline — EC2 provisioning, Ansible execution, Kubernetes pod deployment. Zero manual steps.*

```
git push
   │
   ▼  (GitHub Webhook)
┌─────────────────────────────────────────────┐
│             Jenkins Pipeline                │
│  Stage 1 → Git Checkout                     │
│  Stage 2 → SCP files to Ansible Server      │
│  Stage 3 → SSH into Ansible → Run Playbook  │
└──────────────────┬──────────────────────────┘
                   │
       ┌───────────┴────────────┐
       ▼                        ▼
  ec2.yml (Ansible)         pod.yml (Ansible)
  AWS EC2 Provisioned       K8s Pod Deployed
  SG + AMI + Keypair        ubuntu:latest
  ap-south-1                Status: Running ✅
```

| What | Result |
|------|--------|
| Manual steps in full deployment | **Zero** |
| `ansible -m ping` failures | **Zero** |
| EC2 instances managed | **3** — Jenkins (t3.micro) · Ansible (t3.micro) · K8s (c7i.flex.large) |
| Deployment trigger | **Automatic** on every push |

**Stack:** Jenkins · Ansible · Kubernetes · AWS EC2 · GitHub · SSH/SCP · Linux Ubuntu

---

### Project 2 — Automated AWS EC2 Provisioning via Jenkins

> *Parameterised Bash scripts + GitHub Webhooks + IAM policies = infrastructure on demand.*

```
git push → Webhook → Jenkins Job → Bash Script → EC2 live in < 3 min
                          │
                   Parameterized:
                   instance type / region / AMI
                   Version-controlled. Auditable. Repeatable.
```

| Metric | Before | After |
|--------|--------|-------|
| Provisioning time | 15 min | **< 3 min** |
| Manual console steps | Many | **Zero** |
| Trigger | Manual | **Event-driven (Webhook)** |
| Access control | Ad-hoc | **IAM least-privilege** |

**Stack:** Jenkins · GitHub Webhooks · AWS EC2 · AWS IAM · Bash Scripting · Linux Ubuntu

---

## GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=PushpenderKumar7505&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true"/>
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PushpenderKumar7505&layout=compact&theme=tokyonight&hide_border=true"/>
</p>

<p align="center">
  <img width="65%" src="https://streak-stats.demolab.com/?user=PushpenderKumar7505&theme=tokyonight&hide_border=true"/>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=PushpenderKumar7505&theme=tokyonight&no-frame=true&column=7&margin-w=4"/>
</p>

---

## Recruiter Reference

> *Whatever Cloud/DevOps role you're hiring for — here's what I bring:*

| Role | My Relevant Skills |
|------|--------------------|
| **DevOps Engineer** | Jenkins pipelines · Ansible automation · Git workflows · Linux admin |
| **Cloud Engineer (AWS)** | EC2 · S3 · IAM · VPC · CloudWatch · Terraform IaC |
| **Platform / Infra Engineer** | Kubernetes · container orchestration · IaC · multi-node AWS setup |
| **SRE / Monitoring** | Prometheus + Grafana stack · metrics · observability |
| **CI/CD Engineer** | End-to-end pipeline design · GitHub Webhooks · zero manual deployments |
| **Cloud Security (Entry Level)** | IAM least-privilege · SSH key auth · VPC security groups |

---

## Work Experience

**Backend Developer Intern — Mentobile Technology** &nbsp;`Jul 2024 – Oct 2024`
- Backend modules in CodeIgniter PHP MVC · MySQL schema design · CRUD operations
- Git branching, PRs, code reviews in a live production team

**Market Research Associate — Precise Research Solution, Gurugram** &nbsp;`Jan 2025 – Jun 2025`
- Cleaned and analysed structured datasets · stakeholder decision-support reports

---

## Education & Certifications

| | |
|---|---|
| **B.Tech — Computer Science & Engineering** | GLA University · 2020–2024 · CGPA: 6.83/10 |
| **AWS & DevOps Infrastructure Training** | Croma Campus · Sep 2025 – Mar 2026 |
| Web Development Bootcamp | JOVAC |
| Front End Development (HTML & CSS) | Great Learning |
| Course on Computer Concepts (CCC) | NIELIT |

**Croma Campus covered:** Linux · Git · Jenkins · Docker · AWS (EC2 · S3 · IAM · VPC · CloudWatch) · Kubernetes · Terraform · Ansible · Prometheus · Grafana

---

## Connect

<p align="center">
  <a href="https://linkedin.com/in/pushpender-kumar-5280b7226">
    <img src="https://img.shields.io/badge/LinkedIn-Pushpender_Kumar-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;
  <a href="mailto:pushpender7505@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-pushpender7505@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  &nbsp;
  <a href="https://github.com/PushpenderKumar7505">
    <img src="https://img.shields.io/badge/GitHub-PushpenderKumar7505-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</p>

<p align="center">
  <i>Open to Cloud · DevOps · SRE · Platform Engineering roles — fresher/intern level. Let's talk.</i>
</p>

---

<p align="center">
  <img src="https://github-contributor-stats.vercel.app/api?username=PushpenderKumar7505&limit=5&theme=tokyonight&combine_all_yearly_contributions=true&hide_border=true"/>
</p>

<p align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight"/>
</p>

<p align="center"><i>"Build. Automate. Monitor. Repeat."</i></p>
