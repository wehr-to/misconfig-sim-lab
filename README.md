# 🛠️ misconfig-sim-lab

This repository contains simulations of **common cloud and infrastructure misconfigurations** — and the tools, scripts, and detection logic used to uncover and prevent them.

It’s designed to strengthen your skills in **posture management**, **cloud security**, and **configuration hygiene** across multiple environments.

## 🎯 Why This Repo Exists

Most breaches begin with something misconfigured:

- An open S3 bucket
- A wide-open security group
- An admin role with no MFA
- DNS records leaking private IPs

This repo intentionally recreates these weaknesses, then walks through how to detect, prevent, and automate their remediation — turning lessons into defensive strategy.

## 🔍 What's Covered

| Area                     | Description |
|--------------------------|-------------|
| `cloud-misconfigs/`       | AWS/Azure/GCP-specific misconfiguration simulations |
| `network-posture/`        | Open ports, exposed services, misused firewalls |
| `iam-errors/`             | Weak roles, missing MFA, and excessive permissions |
| `data-exposure/`          | Public S3 buckets, DNS leaks, metadata exposure |
| `detection-and-response/` | CLI and SIEM-based detection techniques |
| `prevention-automation/`  | Terraform and script-based guardrails |
| `docs/`                   | Playbooks, remediation guides, and reference material |

## 🧪 Misconfig Scenarios Simulated

| Scenario                             | Learnings |
|--------------------------------------|-----------|
| `s3-public-read/`                    | Detecting and remediating publicly exposed S3 buckets |
| `sg-open-to-world/`                 | Alerting on 0.0.0.0/0 ingress on SSH, RDP, or DB ports |
| `iam-overprivileged-role/`          | Mapping excessive IAM permissions and missing MFA |
| `dns-record-leakage/`               | Discovering internal IPs via DNS zone misconfig |
| `ec2-imdsv1-enabled/`               | Identifying metadata service v1 exposure |
| `storage-no-encryption/`            | Flagging cloud disks and buckets missing encryption-at-rest |
| `cloudtrail-not-enabled/`           | Simulating gaps in visibility and audit logs |

## 🧠 Tools Used

- AWS CLI, Azure CLI, GCP CLI
- ScoutSuite, Prowler, Cloudsplaining
- OSQuery, Sysmon, CloudWatch Logs
- Terraform for provisioning + prevention
- Bash + Python for simulation scripting

## 👥 Who Should Use This

- Cloud security and blue team professionals
- SOC analysts studying cloud misconfig detection
- DevOps engineers embedding guardrails in CI/CD
- Students or career pivoters learning real-world cloud posture management

## 🛡️ Bonus: Hardening Playbooks

Each simulation includes:

- `detect.md` – How to identify the misconfig
- `prevent.md` – How to block it in IaC or policy
- `remediate.sh` – Fix script if applicable
- `references.md` – Real breaches that used this vector


