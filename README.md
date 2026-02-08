# Terraform GitHub Actions CI

![Terraform CI](https://github.com/yassinahmed323/terraform-github-actions-ci/actions/workflows/terraform-ci.yml/badge.svg)

A production-ready **Terraform CI pipeline** using **GitHub Actions** that automatically enforces Infrastructure-as-Code (IaC) best practices on every push and pull request.

---

## 🚀 What This Project Demonstrates

This repository showcases real-world **DevOps & Terraform CI practices**, including:

- ✅ Automated **Terraform formatting (`fmt`)**
- ✅ Configuration **validation (`validate`)**
- ✅ Infrastructure planning **without applying changes (`plan`)**
- ✅ CI enforcement on **every push to `main`**
- ✅ Clean repository structure with ignored Terraform artifacts

---

## 🧱 Tech Stack

- Terraform
- GitHub Actions
- AzureRM Provider
- Infrastructure as Code (IaC)

---

## 📂 Repository Structure

## ⚙️ CI Workflow Overview

The GitHub Actions workflow runs automatically on every push to `main` and performs the following steps:

1. **Terraform Format Check (`terraform fmt -check`)**
   - Ensures consistent formatting across all Terraform files

2. **Terraform Initialization (`terraform init`)**
   - Downloads required providers in an isolated CI environment

3. **Terraform Validation (`terraform validate`)**
   - Verifies the Terraform configuration is syntactically and logically correct

4. **Terraform Plan (`terraform plan`)**
   - Generates an execution plan without applying any infrastructure changes

❗ No cloud resources are created or modified — this pipeline is **CI-only**.
