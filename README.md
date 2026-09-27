# AWS DevOps Learning Portfolio

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](./LICENSE)
[![Status](https://img.shields.io/badge/status-actively%20building-brightgreen)]()
[![AWS](https://img.shields.io/badge/AWS-Learning%20in%20Progress-FF9900?logo=amazon-aws&logoColor=white)]()

A hands-on, transparently-tracked AWS/DevOps learning repository. Built while working through and extending the [**aws-devops-zero-to-hero**](https://github.com/iam-veeramalla/aws-devops-zero-to-hero) curriculum by [Abhishek Veeramalla](https://github.com/iam-veeramalla), then rebuilding select labs from scratch as original Terraform/IaC work.

> **Note for reviewers:** This is a learning log, not a certification or claimed production track record. Every topic is honestly labeled below — original coursework, my own rebuilds, and concept-only notes are never mixed together. Full attribution and license details: [`ATTRIBUTION.md`](./ATTRIBUTION.md).

---

## About Me

I'm a **DevOps Engineer with ~2 years of experience**, working day-to-day with:

- **Cloud:** Azure (Terraform, AKS, VNets)
- **Orchestration:** Kubernetes
- **CI/CD:** GitHub Actions, Azure DevOps Pipelines

This repository is where I'm actively building **AWS depth** — VPC, EC2, IAM, S3, serverless, and cloud automation — to complement my existing Azure/K8s/Terraform skill set.

**Other portfolio projects:**

| Project | Description |
|---|---|
| [AWS Landing Zone (Terraform)](https://github.com/aniket-devop/aws-terraform-landing-zone-project) | Production-style AWS VPC + EC2 + ALB, built from scratch |
| [Azure Landing Zone (Terraform)](https://github.com/aniket-devop/azure-landing-zone-terraform) | Azure landing zone IaC |
| [GitOps CI/CD Demo](https://github.com/aniket-devop/gitops-ci-pipeline) | App repo — paired with [GitOps config repo](https://github.com/aniket-devop/gitops-kubernetes-config) |

---

## How to Read This Repo

Every topic is tagged with what's **actually true about it right now**. Nothing is marked complete until it's genuinely built, deployed (where applicable), and documented — including what broke and how it was fixed.

| Tag | Meaning |
|---|---|
| 🟩 | **My implementation** — original code/Terraform, deployed and documented by me |
| 🟨 | **My notes on original code** — reference code kept, plus my own run-through/notes |
| 🟦 | **Original (reference only)** — unmodified source material, kept for learning, not claimed as mine |
| ⬜ | **Concept notes only** — no hands-on lab yet |
| 📌 | **Planned lab** — queued to become a 🟩 real lab next |

---

## Learning Roadmap

### Foundations
| Day | Topic | Status | Notes |
|---|---|---|---|
| 1 | Intro to AWS | ⬜ Concept notes | |
| 8 | EC2 / IAM / VPC interview prep | ⬜ Concept notes | See [`interview-questions/`](./interview-questions/) |
| 10 | AWS CLI | ⬜ Concept notes | |

### IAM & Security
| Day | Topic | Status | Notes |
|---|---|---|---|
| 2 | IAM | 📌 Planned | Users, groups, roles, least-privilege policies |
| 5 | AWS Security (SGs, NACLs, IAM policy) | ⬜ Concept notes | |

### Networking
| Day | Topic | Status | Notes |
|---|---|---|---|
| 4 | VPC | ⬜ Concept notes | |
| 6 | Route 53 | ⬜ Concept notes | |
| 7 | Secure VPC + EC2 (2-tier) | ⬜ Concept notes | Built version: [AWS Landing Zone](https://github.com/aniket-devop/aws-terraform-landing-zone-project) |
| 19 | CloudFront | ⬜ Concept notes | |
| 26 | Elastic Load Balancer | ⬜ Concept notes | Also covered in Day 24 Terraform + Landing Zone project |

### Compute
| Day | Topic | Status | Notes |
|---|---|---|---|
| 3 | EC2 | ⬜ Concept notes | |

### Storage
| Day | Topic | Status | Notes |
|---|---|---|---|
| 9 | S3 | 📌 Planned | Versioning, lifecycle policy, static site hosting |

### Infrastructure as Code
| Day | Topic | Status | Notes |
|---|---|---|---|
| 11 | CloudFormation | ⬜ Concept notes | |
| 24 | Terraform (VPC + EC2 + ALB) | 🟦 Reference | Superseded by [AWS Landing Zone](https://github.com/aniket-devop/aws-terraform-landing-zone-project) |

### CI/CD (AWS-native)
| Day | Topic | Status | Notes |
|---|---|---|---|
| 12 | CodeCommit | 📌 Planned | Part of Day 13–15 pipeline |
| 13 | CodePipeline | 📌 Planned | |
| 14 | CodeBuild | 📌 Planned | Original sample app kept as 🟦 reference |
| 15 | CodeDeploy | 📌 Planned | |

### Monitoring & Events
| Day | Topic | Status | Notes |
|---|---|---|---|
| 16 | CloudWatch | 🟦 Reference | |
| 18 | CloudWatch Events / EventBridge | 📌 Planned | Grouped with Day 17 Lambda lab |
| 25 | CloudTrail & Config | 🟦 Reference | |

### Serverless
| Day | Topic | Status | Notes |
|---|---|---|---|
| 17 | Lambda | 📌 Planned | Event-driven function triggered via EventBridge |

### Containers
| Day | Topic | Status | Notes |
|---|---|---|---|
| 20 | ECR | ⬜ Concept notes | |
| 21 | ECS | 🟦 Reference | |
| 22 | EKS + ALB Ingress | 🟦 Reference | Most substantial original lab; may rebuild given my existing AKS/K8s depth |

### Secrets & Compliance
| Day | Topic | Status | Notes |
|---|---|---|---|
| 23 | Systems/Secrets Manager | ⬜ Concept notes | |

### Career Prep
| Day | Topic | Status | Notes |
|---|---|---|---|
| 27 | AWS interview question bank | 🟦 Reference | [`interview-questions/`](./interview-questions/) |
| 28 | Cloud migration strategies | ⬜ Concept notes | |
| 29 | AWS best practices & job prep | ⬜ Concept notes | |
| 30 | RDS project | ⬜ Concept notes | |

---

## Repository Structure

```
├── day-N/                  # Per-topic folder (original numbering preserved for
│                           # traceability to the source repo/playlist — see ATTRIBUTION.md)
├── interview-questions/    # Topic-wise Q&A bank (reference)
├── ATTRIBUTION.md          # Full credit + license explanation
├── LICENSE                 # Apache 2.0
└── README.md               # This file
```

Each completed (🟩) lab follows a consistent write-up format in its `day-N/README.md`:

1. **Original reference** — what it's based on
2. **What I built** — my own implementation
3. **Architecture** — diagram / description
4. **Steps** — how it was deployed
5. **Issues hit & fixes** — real debugging notes
6. **Cleanup / cost notes**
7. **Resume-ready summary** — what I can honestly claim from this lab

---

## License

Licensed under the **Apache License 2.0** — see [`LICENSE`](./LICENSE), inherited from the original source repository. See [`ATTRIBUTION.md`](./ATTRIBUTION.md) for details on what that means for reuse of original vs. original-to-this-repo content.
