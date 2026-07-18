<h1 align="center">AWS 80 Projects Challenge</h1>

<p align="center">
  <strong>A structured cloud engineering portfolio built through 80 hands-on AWS projects.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Completed-7%20of%2080-success" alt="7 of 80 projects completed">
  <img src="https://img.shields.io/badge/Active%20Build-CloudDesk%20SaaS-blue" alt="CloudDesk SaaS active build">
  <img src="https://img.shields.io/badge/Cloud-AWS-FF9900?logo=amazonaws&logoColor=white" alt="AWS">
  <img src="https://img.shields.io/badge/IaC-Terraform-7B42BC?logo=terraform&logoColor=white" alt="Terraform">
  <img src="https://img.shields.io/badge/Containers-Docker-2496ED?logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Automation-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

---

## Overview

This repository is the central index for my **80-project AWS cloud infrastructure challenge**.

Each project is developed in its own GitHub repository and connected here as a **Git submodule**. This keeps every implementation independently documented while providing one place to review my progression across:

- AWS architecture and networking
- Infrastructure as Code
- Linux and compute administration
- containers and application delivery
- high availability and Auto Scaling
- serverless systems
- CI/CD and deployment automation
- identity, security, and secret management
- observability, reliability, and disaster recovery

The objective is not simply to deploy AWS services. Each project is designed around an operational or business requirement and documents the architecture, implementation choices, validation process, security considerations, troubleshooting, and lessons learned.

---

## Progress

**Completed:** 7 projects  
**Active:** Project 8 — CloudDesk Multi-Tenant SaaS  
**Remaining:** Projects 9–80

```text
Progress: [#######.........................................................................] 7 / 80
```

---

## Project Index

| # | Status | Project | Engineering outcome | Core technologies |
|---:|:---:|---|---|---|
| 1 | ✅ | [Static Website with CloudFront](https://github.com/simeonprimordial/aws-static-website-cloudfront) | Hosted static content in Amazon S3 and delivered it through CloudFront for improved availability and global distribution. | S3, CloudFront, IAM |
| 2 | ✅ | [WordPress on Amazon Lightsail](https://github.com/simeonprimordial/aws-wordpress-lightsail) | Deployed and administered a WordPress workload using a simplified AWS virtual server platform. | Lightsail, WordPress, Linux, DNS |
| 3 | ✅ | [EC2 Apache Web Server](https://github.com/simeonprimordial/aws-ec2-apache-webserver) | Provisioned an EC2 instance, configured network access, and automated Apache installation and website delivery. | EC2, Security Groups, Linux, Apache |
| 4 | ✅ | [Highly Available Web Application with Terraform](https://github.com/simeonprimordial/highly-available-web-app-terraform) | Replaced single-instance architecture with repeatable infrastructure using an ALB, Launch Template, and Auto Scaling Group. | Terraform, EC2, ALB, Auto Scaling |
| 5 | ✅ | [FinTrust NLB Docker Service](https://github.com/simeonprimordial/fintrust-nlb-docker) | Deployed a containerized Flask service behind a Network Load Balancer with automated instance replacement and scaling. | Docker, Terraform, NLB, Auto Scaling, Flask |
| 6 | ✅ | [FinTrust Customer Portal](https://github.com/simeonprimordial/fintrust-customer-portal) | Built a production-oriented three-tier application with private compute and database layers, container delivery, load balancing, and managed secrets. | Terraform, Docker, ECR, ALB, Auto Scaling, RDS, Secrets Manager |
| 7 | ✅ | [NovaTech Serverless Website](https://github.com/simeonprimordial/novatech-serverless-website) | Automated secure static-site delivery using a private S3 origin, CloudFront OAC, GitHub Actions, and passwordless AWS authentication through OIDC. | S3, CloudFront, OAC, IAM, GitHub Actions, OIDC |
| 8 | 🚧 | [CloudDesk Multi-Tenant SaaS](https://github.com/simeonprimordial/clouddesk-multi-tenant-saas) | Active build exploring tenant-aware application architecture, authentication, authorization, and secure SaaS infrastructure patterns. | AWS, Go, Amazon Cognito, OIDC, SaaS architecture |

> **Status legend:** ✅ Completed · 🚧 In progress · ⬜ Planned

---

## What the Projects Demonstrate

### Architecture

- selecting services based on workload and business requirements
- designing for availability, scalability, and failure recovery
- separating public, application, and database responsibilities
- documenting data flow and deployment workflows with diagrams

### Infrastructure as Code

- reusable Terraform configuration
- variables, outputs, data sources, and resource dependencies
- repeatable infrastructure deployment and teardown
- validation through `terraform fmt`, `terraform init`, and `terraform validate`

### Security

- least-privilege IAM roles and policies
- private S3 origins through CloudFront Origin Access Control
- private application and database networking
- GitHub OIDC instead of long-lived AWS access keys
- AWS Secrets Manager for application and database credentials

### Delivery and Operations

- Docker image build and deployment
- Amazon ECR integration
- GitHub Actions CI/CD
- load-balancer health checks
- Auto Scaling and unhealthy-instance replacement
- troubleshooting documentation and architecture decision records

---

## Repository Model

This is a **portfolio index repository**. The project directories are Git submodules rather than copied source-code folders.

```text
AWS80ProjectsChallenge/
├── aws-static-website-cloudfront/
├── aws-wordpress-lightsail/
├── aws-ec2-apache-webserver/
├── highly-available-web-app-terraform/
├── fintrust-nlb-docker/
├── fintrust-customer-portal/
├── novatech-serverless-website/
├── clouddesk-multi-tenant-saas/
├── .gitmodules
├── LICENSE
└── README.md
```

Each submodule points to the corresponding standalone project repository, where the complete source code, diagrams, screenshots, decisions, and troubleshooting notes are maintained.

---

## Clone the Complete Portfolio

Clone the index and initialize every project submodule:

```bash
git clone --recurse-submodules https://github.com/simeonprimordial/AWS80ProjectsChallenge.git
cd AWS80ProjectsChallenge
```

When the repository was cloned without `--recurse-submodules`, initialize the projects afterward:

```bash
git submodule update --init --recursive
```

Pull the latest commits recorded by the portfolio repository:

```bash
git pull
git submodule update --init --recursive
```

To fetch newer commits from each submodule's tracked remote branch for review:

```bash
git submodule update --remote --recursive
```

> Updating a submodule locally does not automatically update this index. The new submodule commit must also be committed in the parent repository.

---

## Project Documentation Standard

As the challenge progresses, each substantial project aims to include:

- a clear business problem and solution overview
- architecture and deployment diagrams
- repository structure and deployment instructions
- security and cost considerations
- validation evidence
- architecture decision records
- troubleshooting notes
- lessons learned and future improvements

Projects may differ in depth depending on their scope, but the standard becomes more rigorous as the portfolio advances.

---

## Current Focus

Project 8, **CloudDesk**, is the next stage of the roadmap. It moves beyond individual infrastructure components into a multi-tenant SaaS system where identity, tenant isolation, authorization, application design, and cloud infrastructure must work together.

Upcoming portfolio areas include:

- observability with CloudWatch, Prometheus, and Grafana
- configuration management and automation
- ECS and Kubernetes workloads
- secure multi-environment CI/CD
- event-driven and data-processing systems
- backup, disaster recovery, and cross-region architectures
- cloud security and compliance controls

---

## Portfolio Links

- [GitHub Profile](https://github.com/simeonprimordial)
- [Cloud Portfolio Website](https://simeonprimordial.github.io/SimeonOnTheCloudSpace/)
- [LinkedIn](https://www.linkedin.com/in/simeon-siaka-8a8367312/)

---

## License

This index repository is licensed under the [MIT License](LICENSE). Individual project repositories may include their own license and usage conditions.
