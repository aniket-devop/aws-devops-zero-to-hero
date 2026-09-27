# AWS DevOps Learning Portfolio

Personal, hands-on AWS/DevOps learning repository — built by me while working through and
extending the [aws-devops-zero-to-hero](https://github.com/iam-veeramalla/aws-devops-zero-to-hero)
curriculum by [Abhishek Veeramalla](https://github.com/iam-veeramalla). Full credit and license
details are in [`ATTRIBUTION.md`](./ATTRIBUTION.md) — please read that before assuming any
content here is original coursework design.

**This is not a certification, a production track record, or claimed work experience.** It's
a transparent record of what I've actually built, run, broken, and fixed while learning AWS —
alongside my existing DevOps work in Azure/Kubernetes/Terraform (see my other repos below).

## Who I am

DevOps Engineer, ~2 years experience, working day-to-day with Azure (Terraform, AKS, VNets),
Kubernetes, and CI/CD (GitHub Actions, Azure DevOps Pipelines). This repo is where I'm
building AWS depth on VPC, EC2, IAM, S3, and broader cloud/DevOps automation.

## How to read the status table

Every topic below is tagged with what's *actually true about it right now* — no topic is
marked done until it's genuinely built, deployed (where applicable), and documented with
what went wrong along the way.

| Tag | Meaning |
|---|---|
| 🟩 My implementation | My own code/Terraform, deployed and documented by me |
| 🟨 My notes on original code | Original author's code kept as reference + my own run-through/notes |
| 🟦 Original (reference only) | Unmodified original material, kept for learning — not claimed as mine |
| ⬜ Concept notes only | No hands-on lab yet — notes describe the concept only |
| 📌 Planned lab | Queued to become a 🟩 real lab next |

## Topic map

### Foundations
| Day | Topic | Status | Notes |
|---|---|---|---|
| 1 | Intro to AWS | ⬜ Concept notes only | |
| 8 | EC2/IAM/VPC interview prep | ⬜ Concept notes only | See `interview-questions/` |
| 10 | AWS CLI | ⬜ Concept notes only | |

### IAM & Security
| Day | Topic | Status | Notes |
|---|---|---|---|
| 2 | IAM | 📌 Planned lab | Users/groups/roles/least-privilege policies |
| 5 | AWS Security (SGs, NACLs, IAM policy) | ⬜ Concept notes only | |

### Networking
| Day | Topic | Status | Notes |
|---|---|---|---|
| 4 | VPC | ⬜ Concept notes only | |
| 6 | Route 53 | ⬜ Concept notes only | |
| 7 | Secure VPC + EC2 (2-tier) | ⬜ Concept notes only | Overlaps my [AWS Landing Zone](https://github.com/aniket-devop/aws-terraform-landing-zone-project) project — see that repo for the built version |
| 19 | CloudFront | ⬜ Concept notes only | |
| 26 | Elastic Load Balancer | ⬜ Concept notes only | Also covered in Day 24 Terraform + Landing Zone project |

### Compute
| Day | Topic | Status | Notes |
|---|---|---|---|
| 3 | EC2 | ⬜ Concept notes only | |

### Storage
| Day | Topic | Status | Notes |
|---|---|---|---|
| 9 | S3 | 📌 Planned lab | Versioning, lifecycle policy, static site hosting |

### Infrastructure as Code
| Day | Topic | Status | Notes |
|---|---|---|---|
| 11 | CloudFormation | ⬜ Concept notes only | |
| 24 | Terraform (VPC + EC2 + ALB) | 🟦 Original (reference only) | Superseded by my [AWS Landing Zone](https://github.com/aniket-devop/aws-terraform-landing-zone-project) Terraform project |

### CI/CD (AWS-native)
| Day | Topic | Status | Notes |
|---|---|---|---|
| 12 | CodeCommit | 📌 Planned lab | Part of Day 13–15 pipeline |
| 13 | CodePipeline | 📌 Planned lab | |
| 14 | CodeBuild | 📌 Planned lab | Original sample app kept as 🟦 reference |
| 15 | CodeDeploy | 📌 Planned lab | |

### Monitoring & Events
| Day | Topic | Status | Notes |
|---|---|---|---|
| 16 | CloudWatch | 🟦 Original (reference only) | |
| 18 | CloudWatch Events / EventBridge | 📌 Planned lab | Grouped with Day 17 Lambda lab |
| 25 | CloudTrail & Config | 🟦 Original (reference only) | |

### Serverless
| Day | Topic | Status | Notes |
|---|---|---|---|
| 17 | Lambda | 📌 Planned lab | Event-driven function triggered via EventBridge |

### Containers
| Day | Topic | Status | Notes |
|---|---|---|---|
| 20 | ECR | ⬜ Concept notes only | |
| 21 | ECS | 🟦 Original (reference only) | |
| 22 | EKS + ALB Ingress | 🟦 Original (reference only) | Most substantial original lab — kept for reference; may rebuild later given my existing AKS/K8s depth |

### Secrets & Compliance
| Day | Topic | Status | Notes |
|---|---|---|---|
| 23 | Systems/Secrets Manager | ⬜ Concept notes only | |

### Career prep
| Day | Topic | Status | Notes |
|---|---|---|---|
| 27 | AWS interview question bank | 🟦 Original (reference only) | `interview-questions/` |
| 28 | Cloud migration strategies | ⬜ Concept notes only | |
| 29 | AWS best practices & job prep | ⬜ Concept notes only | |
| 30 | RDS project | ⬜ Concept notes only | |

## Repo layout

```
day-N/            # Per-topic folder (original numbering kept for traceability to the
                   # source repo and its video playlist — see ATTRIBUTION.md)
interview-questions/  # Original author's topic-wise Q&A bank (kept as reference)
ATTRIBUTION.md    # Full credit + license explanation
README.md         # This file
```

As each 📌 planned lab is built, its `day-N/README.md` will follow the same format:
**original reference → what I built → architecture → steps → issues hit & how I fixed
them → cleanup/cost notes → what I can honestly say about this on my resume.**

## My other DevOps portfolio projects

- [AWS Landing Zone (Terraform)](https://github.com/aniket-devop/aws-terraform-landing-zone-project)
- [Azure Landing Zone (Terraform)](https://github.com/aniket-devop/azure-landing-zone-terraform)
- GitOps CI/CD demo: [app](https://github.com/aniket-devop/gitops-ci-pipeline) / [GitOps config](https://github.com/aniket-devop/gitops-kubernetes-config)

## License

Apache License 2.0 — see [`LICENSE`](./LICENSE), inherited from the original repository. See
[`ATTRIBUTION.md`](./ATTRIBUTION.md) for what that means for reuse of this repo's content.
