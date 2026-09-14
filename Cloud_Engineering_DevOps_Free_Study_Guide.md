# The Complete Free Study Guide: Cloud Engineering & DevOps

> Based on the **bKash Cloud Engineering / DevOps Engineering Support Service** Job Description  
> Everything listed here is **100% free**. No paid courses. No subscriptions.

---

## How to Use This Guide

Follow the modules in order, complete every hands-on lab, and build the portfolio projects at the end. This guide maps directly to every responsibility and qualification in the JD.

**Prerequisites:**
- An AWS Free Tier account (set MFA + $1 budget alert immediately)
- A GitHub account
- A Linux environment (WSL2, VM, or cloud shell)

---

## Module 1: Cloud Infrastructure — AWS (Primary) & GCP

### What the JD Requires
- **AWS**: EC2, VPC, IAM, S3, RDS, EKS, ALB/NLB, Route 53, CloudWatch
- **GCP**: Working knowledge of GKE and core services

### Free AWS Training Path

| Topic | Free Resource | What to Do |
|-------|--------------|------------|
| **AWS Fundamentals** | [AWS Skill Builder — Free Tier](https://skillbuilder.aws) | Start with "AWS Cloud Practitioner Essentials" (free digital training) |
| **EC2, VPC, IAM, S3, RDS** | [AWS Tutorial for Beginners 2026 (YouTube)](https://www.youtube.com/watch?v=uvK4c3FOW5w) | 36-minute crash course with live demos using Free Tier |
| **IAM Deep Dive** | [AWS IAM Documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html) | Master users, groups, roles, policies, least privilege |
| **VPC & Networking** | [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) | Learn subnets, route tables, NAT Gateway, peering, security groups vs NACLs |
| **EKS (Kubernetes)** | [Amazon EKS Documentation](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) | Understand managed control plane, node groups, Fargate profiles |
| **ALB/NLB** | [AWS Elastic Load Balancing](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/what-is-load-balancing.html) | ALB (Layer 7, HTTP/HTTPS) vs NLB (Layer 4, TCP/UDP) |
| **Route 53** | [AWS Route 53 Tutorial — DevOpsSchool](https://www.devopsschool.com/tutorials/aws-amazon-route-53-tutorial-architecture-pricing-use-cases-and-hands-on-guide-for-networking-and-content-delivery/) | Hosted zones, alias records, health checks, routing policies |
| **CloudWatch** | [AWS CloudWatch Documentation](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) | Metrics, logs, alarms, dashboards, Container Insights for EKS |

**Critical Free Tier Setup:** Create an AWS Free Tier account. Set MFA, budget alerts ($1), and IAM users immediately. Never use the root account for daily tasks.

### Free GCP Training Path

| Topic | Free Resource |
|-------|--------------|
| **GCP Fundamentals** | [Google Cloud Skills Boost — Free Tier](https://www.cloudskillsboost.google) |
| **GCP Core Services** | [Google Cloud Full Course 2025 (YouTube)](https://www.youtube.com/watch?v=lvZk_sc8u5I) |
| **GKE** | [Google Kubernetes Engine Docs](https://cloud.google.com/kubernetes-engine/docs) |
| **GCP Free Tier** | [$300 free credits + always-free tier](https://cloud.google.com/free) |

---

## Module 2: Containers & Orchestration (Docker, Kubernetes, Helm)

### What the JD Requires
- Manage Kubernetes platforms (EKS/GKE)
- Containerized applications using Docker
- Helm for package management

### Free Learning Path

| Topic | Free Resource | Hands-On |
|-------|--------------|----------|
| **Docker** | [Docker Official Docs — Get Started](https://docs.docker.com/get-started/) | Build, run, and push images to Docker Hub |
| **Kubernetes Basics** | [Official Kubernetes Tutorials (Katacoda)](https://kubernetes.io/docs/tutorials/kubernetes-basics/) | Browser-based interactive labs — no setup needed |
| **KillerCoda K8s Labs** | [KillerCoda Interactive Kubernetes](https://killercoda.com/kubernetes) | Free sandbox environments |
| **KodeKloud Free Labs** | [KodeKloud Free Kubernetes Labs](https://kodekloud.com/blog/kubernetes-tutorial-for-beginners-2025/) | Browser-based, no installation |
| **Helm** | [Helm Official Docs](https://helm.sh/docs/) + [Helm Chart Tutorial 2026](https://tech-insider.org/ie/helm-chart-tutorial-2026/) | Learn charts, values, templating, releases, rollbacks |
| **IBM CloudLabs** | [IBM Free Interactive Kubernetes Tutorials](https://www.ibm.com/products/tutorials/ibm-cloudlabs-free-interactive-kubernetes-tutorials) | 3 free labs with certification badge |

### Key Concepts to Master
- **Pods, Deployments, Services, Ingress, ConfigMaps, Secrets, Namespaces**
- **EKS vs GKE**: Managed control plane, node groups, cluster autoscaling
- **Helm 3 vs Helm 4**: Helm 3 is in maintenance; Helm 4 adds Server-Side Apply and Wasm plugins
- **Docker best practices**: Multi-stage builds, non-root users, image scanning, layer caching

---

## Module 3: Infrastructure as Code (Terraform & Packer)

### What the JD Requires
- Develop and maintain Infrastructure as Code (Terraform)
- Experience with Packer

### Free Terraform Training

| Resource | Link | Notes |
|----------|------|-------|
| **Official HashiCorp Tutorials** | [Terraform Tutorials — AWS](https://developer.hashicorp.com/terraform/tutorials/aws-get-started) | The canonical free source — step-by-step, command-line |
| **Terraform GCP Tutorials** | [Terraform Tutorials — GCP](https://developer.hashicorp.com/terraform/tutorials/gcp-get-started) | Same official quality for Google Cloud |
| **freeCodeCamp 7-Hour Course** | [YouTube — Terraform Complete Course](https://www.youtube.com/results?search_query=freecodecamp+terraform+2026) | Best free video for certification prep |
| **Terraform Style Guide** | [HashiCorp Style Guide](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/terraform-style-guide) | Best practices for formatting and structure |

### Free Packer Training

| Resource | Link | Notes |
|----------|------|-------|
| **Official Packer Tutorials** | [Packer Getting Started](https://developer.hashicorp.com/packer/tutorials) | Build Docker images locally (free, no cloud needed) or AWS AMIs |
| **Microsoft DevOps Lab** | [Automating Azure Image Pipelines with HCP Packer](https://learn.microsoft.com/en-us/shows/devops-lab/automating-azure-image-pipelines-with-hcp-packer) | Video tutorial on golden image pipelines |
| **Packer GitHub** | [hashicorp/packer](https://github.com/hashicorp/packer) | Source code and quick start |

### Key Concepts
- **Terraform**: HCL syntax, state files, backends, modules, workspaces, `plan`/`apply`/`destroy`, remote state locking
- **Packer**: Builders, provisioners (shell, Ansible), post-processors, golden image pipeline
- **Best Practice**: Store state remotely (S3 + DynamoDB), use modules for reusability, never commit secrets

---

## Module 4: CI/CD Pipelines (GitHub Actions & Jenkins)

### What the JD Requires
- Build and support CI/CD pipelines using GitHub Actions and/or Jenkins

### Free GitHub Actions Training

| Resource | Link | What You Learn |
|----------|------|----------------|
| **GitHub Docs** | [GitHub Actions Quickstart](https://docs.github.com/en/actions/quickstart) | Official, always up-to-date |
| **GitHub Actions Free Tier** | Unlimited minutes for public repos; 2,000 min/month for private repos | Generous free tier for learning |
| **GitHub Skills** | [GitHub Skills — Actions](https://skills.github.com/) | Interactive, in-repo learning |
| **freeCodeCamp CI/CD Course** | [YouTube — CI/CD with GitHub Actions](https://www.youtube.com/results?search_query=freecodecamp+github+actions+2026) | Full project-based tutorial |

### Free Jenkins Training

| Resource | Link | What You Learn |
|----------|------|----------------|
| **Jenkins Official Docs** | [Jenkins.io Tutorials](https://www.jenkins.io/doc/tutorials/) | Pipeline-as-code, Jenkinsfile, Groovy DSL |
| **Jenkins Complete Guide 2026** | [Stackademic Jenkins Tutorial 2026](https://blog.stackademic.com/part-1-jenkins-tutorial-2026-the-complete-guide-to-ci-cd-pipelines-plugins-devops-3218daa4cb1d) | Installation, plugins, nodes, security, integrations |
| **Jenkins is Free** | Self-hosted = MIT license free | Note: TCO includes maintenance time |

### Key CI/CD Concepts
- **Pipeline stages**: Build → Test → Security Scan → Deploy
- **GitHub Actions**: YAML syntax, reusable workflows, self-hosted runners, OIDC for AWS auth, secrets management
- **Jenkins**: Declarative vs Scripted pipelines, agents, master/agent architecture, Blue Ocean
- **Deployment strategies**: Blue/Green, Canary, Rolling updates
- **Security in CI/CD**: Dependency scanning, SAST/DAST, signed artifacts, least privilege on runners

---

## Module 5: Linux Administration, Shell Scripting & Ansible

### What the JD Requires
- Strong Linux administration and Shell scripting skills
- Experience with Ansible

### Free Linux & Shell Scripting Training

| Resource | Link | Notes |
|----------|------|-------|
| **Linux Foundation Free Courses** | [Linux Foundation Training](https://www.linuxfoundation.org/resources) | System administration basics |
| **freeCodeCamp Shell Scripting** | [YouTube — Shell Scripting Full Course 2026](https://www.youtube.com/watch?v=ro0Wees2ghA) | 2026 updated free course |
| **FreeAcademy Bash** | [Free Bash Scripting Course + Certificate](https://freeacademy.ai/blog/best-free-bash-scripting-course) | Free certificate upon completion |

### Free Ansible Training

| Resource | Link | Notes |
|----------|------|-------|
| **Red Hat Ansible Basics** | [Red Hat Learning Ansible Tutorial](https://www.redhat.com/en/topics/automation/learning-ansible-tutorial) | Official, interactive lab included |
| **Red Hat Free Course DO007** | [Ansible Basics: Automation Technical Overview](https://www.redhat.com/en/technologies/management/ansible/training-and-certification) | Free before advanced courses |
| **Ansible Official Docs** | [Ansible Documentation](https://docs.ansible.com/ansible/latest/index.html) | Playbooks, inventory, modules, roles, collections |

### Key Concepts
- **Linux**: File permissions, systemd, cron, networking tools (`netstat`, `ss`, `tcpdump`), log management (`journalctl`, `rsyslog`), package managers (`apt`, `yum`, `dnf`)
- **Shell Scripting**: Variables, loops, conditionals, functions, error handling, `set -euo pipefail`, logging
- **Ansible**: Playbooks, inventory (static/dynamic), roles, handlers, idempotency, vault for secrets, ad-hoc commands

---

## Module 6: Networking, Cloud Security, Monitoring & Logging

### What the JD Requires
- Good understanding of networking, cloud security, monitoring, and logging

### Free Training Resources

| Topic | Free Resource | Key Concepts |
|-------|--------------|------------|
| **Cloud Networking** | [AWS VPC Networking](https://docs.aws.amazon.com/vpc/latest/userguide/how-it-works.html) | Subnets, CIDR, NAT, peering, transit gateway, private link |
| **Cloud Security** | [AWS Security Documentation](https://docs.aws.amazon.com/security/) | IAM policies, security groups, NACLs, KMS, Secrets Manager, WAF, Shield |
| **Monitoring** | [AWS CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) + [Prometheus/Grafana Docs](https://prometheus.io/docs/introduction/overview/) | Metrics, alarms, dashboards, log insights |
| **Logging** | [AWS CloudWatch Logs](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html) + [ELK Stack](https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-elastic-stack.html) | Log groups, log streams, retention, centralized logging |
| **DevOps Monitoring 2026** | [Refonte Learning — DevOps Monitoring Tools](https://www.refontelearning.com/blog/monitoring-tools-in-devops-engineering-in-2026-essential-tools-trends-and-best-practices) | Prometheus/Grafana + cloud-native tools together |

### Best Practices
- **Defense in depth**: MFA, least privilege, encryption at rest/transit, private subnets for databases
- **Observability**: Metrics (what), logs (why), traces (where) — the three pillars
- **Alerting**: Alert on symptoms (latency, error rate), not causes (CPU). Use runbooks for every alert.

---

## Module 7: Version Control & Git Workflow

### What the JD Requires
- Experience with Git
- Follow operational procedures, Git workflow

### Free Git Training

| Resource | Link | Best For |
|----------|------|----------|
| **Pro Git Book** | [git-scm.com/book](https://git-scm.com/book) | The definitive free deep dive — branching, rebasing, internals |
| **Atlassian Git Tutorials** | [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials) | Branching strategies, team workflows, merge vs rebase |
| **freeCodeCamp Git Crash Course** | [YouTube — Git & GitHub](https://www.youtube.com/results?search_query=freecodecamp+git+github+crash+course) | One-session foundation for visual learners |
| **GitHub Skills** | [skills.github.com](https://skills.github.com/) | Interactive, in-repo learning for GitHub-specific workflows |

### Git Workflows to Master
- **Feature Branch Workflow**: Create branch → Commit → PR → Review → Merge
- **GitHub Flow**: Simplified version — branch, PR, deploy, merge
- **GitFlow**: `main`, `develop`, `feature/*`, `release/*`, `hotfix/*` — good for scheduled releases
- **Trunk-Based Development**: Short-lived branches, frequent merges to main — preferred for CI/CD

---

## Module 8: Deployment Environments & Operations

### What the JD Requires
- Support deployments across Dev, SIT, UAT, and Production environments
- Administer core cloud services, networking, storage, security, and IAM

### Environment Strategy

| Environment | Purpose | Key Practices |
|-------------|---------|---------------|
| **Dev** | Developer experimentation | Frequent resets, lowest cost instances, feature flags |
| **SIT (System Integration Testing)** | Integrate components | Mirror production topology at smaller scale, automated deployments |
| **UAT (User Acceptance Testing)** | Stakeholder validation | Production-like data (anonymized), stable releases |
| **Production** | Live customer traffic | Immutable infrastructure, blue/green or canary, strict change management |

### Change Management Best Practices
- **Infrastructure as Code**: Same Terraform module for all environments, different `tfvars`
- **GitOps**: Git as single source of truth for infrastructure and app configs
- **Approval Gates**: Manual approval for UAT → Prod; automated for Dev → SIT
- **Rollback Plan**: Every deployment must have a tested rollback procedure

---

## Module 9: Agile, SDLC & DevOps Best Practices

### What the JD Requires
- Knowledge of Agile, SDLC, and DevOps best practices
- Participate in sprint planning, knowledge sharing, and continuous service improvement

### Free Training & Reading

| Resource | Link | What You Learn |
|----------|------|----------------|
| **Agile SDLC Overview** | [SixSigma.us — Agile SDLC](https://www.6sigma.us/six-sigma-in-focus/agile-sdlc-software-development-life-cycle/) | Kanban, Scrum, XP, best practices |
| **SDLC Best Practices 2026** | [Axify — SDLC Best Practices](https://axify.io/blog/sdlc-best-practices) | 12 modern practices including shift-left security, DORA metrics, CI/CD |
| **DevOps Best Practices 2026** | [TierPoint — 11 DevOps Strategies](https://www.tierpoint.com/blog/cloud/devops-best-practices-to-give-you-the-competitive-advantage/) | CI/CD, Agile project management, automation, observability |

### Key Frameworks & Metrics
- **Agile**: Scrum (sprints, ceremonies, story points), Kanban (WIP limits, continuous flow)
- **SDLC Phases**: Planning → Design → Development → Testing → Deployment → Maintenance
- **DORA Metrics**: Deployment Frequency, Lead Time for Changes, Change Failure Rate, Mean Time to Restore (MTTR)
- **Shift-Left Security**: Security checks in CI/CD, dependency scanning, SAST — not just at the end

---

## Module 10: Incident Management, RCA, SLA & Documentation

### What the JD Requires
- Ensure platform availability within agreed SLA
- Monitor, troubleshoot, investigate alerts, perform incident recovery, RCA
- Prepare technical documentation, SOPs, and operational runbooks

### Free Training & Templates

| Resource | Link | What You Learn |
|----------|------|----------------|
| **SRE Incident Management** | [Skillsoft — SRE Deep Dives & Postmortems](https://www.skillsoft.com/course/sre-incident-management-deep-dives-postmortems-continuous-improvement-4cdbe942-147f-4a10-8f4c-b47a242c8c5e) | Blameless postmortems, 5 Whys, continuous improvement |
| **Postmortem Template** | [Xurrent — How to Write Incident Postmortems](https://www.xurrent.com/blog/how-to-write-incident-postmortem) | Free template + 5 Whys technique |

### Key Concepts
- **SLA (Service Level Agreement)**: Uptime target (e.g., 99.9% = 43.8 min downtime/month). Measure with CloudWatch Synthetics.
- **SLI (Service Level Indicator)**: Measurable metric (latency, error rate, throughput)
- **SLO (Service Level Objective)**: Target value for SLI (e.g., p99 latency < 200ms)
- **Incident Response**: Detect → Triage → Mitigate → Resolve → Postmortem
- **RCA (Root Cause Analysis)**: 5 Whys technique. Focus on systemic issues, never blame individuals.
- **Runbooks**: Step-by-step procedures for common alerts (e.g., "Disk Full on EKS Node"). Store in wiki/Git repo.
- **SOPs (Standard Operating Procedures)**: Change management process, deployment checklist, access request workflow

---

## Module 11: Java Application Deployment (Advantage)

### What the JD Requires
- Exposure to Java application deployment (Maven/Gradle) is an advantage

### Free Training

| Resource | Link | What You Learn |
|----------|------|----------------|
| **Maven Official** | [Maven Getting Started](https://maven.apache.org/guides/getting-started/index.html) | `pom.xml`, lifecycle, plugins, packaging JARs/WARs |
| **Gradle Official** | [Gradle Docs](https://docs.gradle.org/current/userguide/userguide.html) | `build.gradle`, tasks, wrapper, dependency management |
| **Spring Boot Deployment** | [Spring Boot Deployment Guide](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#deployment) | Executable JARs, externalized config, profile-specific properties |
| **Java CI/CD Example** | [Deploying Java Gradle Application](https://dev.to/574n13y/deploying-a-java-gradle-application-on-digitalocean-64a) | Build → Test → Deploy pipeline example |

### Key Concepts
- **Maven**: `mvn clean package`, `pom.xml`, dependencies, `spring-boot-maven-plugin`
- **Gradle**: `./gradlew build`, `build.gradle`, tasks, `bootJar`
- **Deployment**: Executable JAR with embedded Tomcat, Docker multi-stage build for Java apps, JVM tuning (`-Xmx`, `-Xms`)

---

## Free Certification Roadmap

| Certification | Free Prep | Cost of Exam | Value for This JD |
|---------------|-----------|--------------|-------------------|
| **AWS Cloud Practitioner** | [AWS Skill Builder Free](https://skillbuilder.aws) | ~$100 | Foundation — good to have |
| **AWS Solutions Architect Associate** | [FreeCodeCamp + AWS Docs](https://www.youtube.com/results?search_query=freecodecamp+aws+solutions+architect+2026) | ~$150 | **Highly relevant** — covers EC2, VPC, IAM, S3, RDS, EKS |
| **Terraform Associate (004)** | [HashiCorp Free Study Guide](https://developer.hashicorp.com/terraform/tutorials/certification) | ~$70 | **Required skill** — free official prep |
| **CKA (Certified Kubernetes Administrator)** | [KodeKloud Free + KillerCoda](https://kodekloud.com/blog/kubernetes-tutorial-for-beginners-2025/) | ~$395 | **Highly relevant** — EKS/GKE management |
| **Google Cloud Digital Leader** | [Google Cloud Skills Boost](https://www.cloudskillsboost.google) | ~$99 | GCP working knowledge |

---

## Portfolio Projects (Build These for Free)

Build these using **AWS Free Tier** + **GitHub Actions** (free for public repos). Document everything in GitHub READMEs.

### Project 1: Multi-Tier Web App on AWS
- **VPC** with public/private subnets, NAT Gateway
- **EC2** (Bastion host in public, app in private) or **ECS/EKS**
- **RDS** MySQL/PostgreSQL in private subnet
- **ALB** in public subnets
- **Route 53** alias record to ALB
- **Terraform** for all infrastructure
- **GitHub Actions** pipeline: Terraform plan on PR, apply on merge
- **CloudWatch** dashboard for monitoring

### Project 2: Kubernetes Microservices Deployment
- Local **minikube** or **kind** (free, no cloud cost)
- **Docker** multi-stage builds for 2-3 microservices
- **Helm** chart to deploy all services
- **Ingress** controller (NGINX)
- **Prometheus + Grafana** for monitoring (Helm charts available)
- **GitHub Actions**: Build → Push to Docker Hub → Helm upgrade

### Project 3: Golden Image Pipeline
- **Packer** template to build hardened Ubuntu AMI
- **Ansible** provisioner to install CloudWatch agent, security patches
- **Terraform** to launch EC2 from the golden image
- **S3** + **DynamoDB** for Terraform remote state
- Versioned AMIs with lifecycle management

### Project 4: Java App CI/CD
- Fork a simple **Spring Boot** app from GitHub
- **Maven/Gradle** build in GitHub Actions
- **Docker** build and push
- Deploy to **AWS ECS** or **EKS** via GitHub Actions
- Include **SonarQube** community edition (free) for code quality

---

## 12-Week Study Schedule

| Week | Focus | Daily Commitment |
|------|-------|------------------|
| **1-2** | AWS Core (EC2, VPC, IAM, S3) + Linux basics | 2 hours |
| **3-4** | Docker + Kubernetes basics (minikube + Katacoda labs) | 2 hours |
| **5-6** | Terraform (AWS) + Packer | 2 hours |
| **7-8** | CI/CD — GitHub Actions deep dive + Jenkins setup | 2 hours |
| **9** | Ansible + Shell scripting | 2 hours |
| **10** | GCP basics + Route 53 + CloudWatch + ALB/NLB | 2 hours |
| **11** | Helm + EKS/GKE + Monitoring/Logging stack | 2 hours |
| **12** | Portfolio projects + documentation + review | 3-4 hours |

---

## Quick Reference: Every JD Term Explained

| Term | Meaning |
|------|---------|
| **EKS** | Amazon Elastic Kubernetes Service — managed K8s control plane |
| **GKE** | Google Kubernetes Engine — managed K8s on GCP |
| **ALB/NLB** | Application Load Balancer (L7) / Network Load Balancer (L4) |
| **IaC** | Infrastructure as Code — Terraform, CloudFormation |
| **Helm** | Kubernetes package manager — charts, releases, values |
| **SIT** | System Integration Testing environment |
| **UAT** | User Acceptance Testing environment |
| **RCA** | Root Cause Analysis — finding the true source of an incident |
| **SLA** | Service Level Agreement — uptime/performance contract |
| **SOP** | Standard Operating Procedure — documented repeatable process |
| **Runbook** | Step-by-step guide for responding to specific alerts |
| **DORA** | DevOps Research and Assessment metrics |
| **Shift-Left** | Moving testing/security earlier in the SDLC |
| **GitOps** | Using Git as the source of truth for infrastructure |

---

> **Final Tip:** The JD requires **documentation skills**. As you learn, write your own SOPs and runbooks in a GitHub repository. This proves you can do the job before you even start. Good luck!
