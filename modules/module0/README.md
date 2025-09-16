# Module 0 — Environment & Tooling (Day 0–1)

## What we installed
- Ubuntu VM + updates
- Docker CE (with containerd) ✅
- AWS CLI v2 ✅
- Terraform CLI ✅
- kubectl ✅
- Kind local K8s cluster ✅
- Git + SSH to GitHub ✅

## Verification (expected good outputs)
- `docker run hello-world` → “Hello from Docker!”
- `aws --version` → aws-cli/2.x
- `terraform -version` → Terraform v1.x
- `kubectl version --client` → Client Version v1.xx
- `kind create cluster --name lab` → cluster created, node **Ready**
- `ssh -T git@github.com` → “Hi Olagoldstx! …”

## Why this matters (Deep Reasoning)
This is the **workbench + tools**. If the tools are sharp, every module after this is smooth.
