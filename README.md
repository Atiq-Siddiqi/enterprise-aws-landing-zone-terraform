# Enterprise AWS Landing Zone & Multi-Account Governance

A production-ready reference architecture and automation framework for deploying, securing, and governing multi-account enterprise cloud environments on AWS. This project establishes core organizational guardrails, automates isolated account provisioning via **Terraform**, and enforces continuous compliance baselines using **Ansible**.

---

## 🚀 Project Overview
Architected and deployed a secure, multi-account AWS environment utilizing AWS Control Tower, Terraform, and Ansible to automate baseline configuration and IAM guardrails. This project simulates an enterprise-grade landing zone designed to eliminate manual provisioning delays and ensure strict multi-account security compliance during large-scale corporate migrations.

---

## 🛠️ Tech Stack
* **Cloud Platform:** AWS (Control Tower, AWS Organizations, IAM, Systems Manager, S3)
* **Infrastructure as Code (IaC):** Terraform (modular structure supporting multi-account environments)
* **Configuration Management & Automation:** Ansible (automated server baselining and patch management)
* **Governance & Security:** Service Control Policies (SCPs), regional restrictions, and encryption enforcement

---

## 📐 Repository Architecture & Structure

```text
enterprise-aws-landing-zone-terraform/
├── ansible/
│   ├── inventories/
│   │   └── inventory.ini
│   └── playbooks/
│       └── baseline_config.yml
├── terraform/
│   ├── environments/
│   │   └── prod/
│   │       ├── iam_guardrails.tf
│   │       ├── main.tf
│   │       ├── outputs.tf
│   │       └── variables.tf
│   └── modules/
│       ├── control_tower_ous/
│       │   ├── main.tf
│       │   └── outputs.tf
│       └── sandbox_account/
│           ├── main.tf
│           └── outputs.tf
└── README.md
