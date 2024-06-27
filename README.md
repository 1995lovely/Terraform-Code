# Terraform-Code

## Overview

This repository contains Terraform configuration for creating and managing a GitHub repository using Terraform. The configuration allows for the automated creation of a new GitHub repository with predefined settings.

## Repository Details

- **Repository Name**: Terraform-Code
- **Description**: My All Terraform Codes
- **Visibility**: Public

## Terraform Configuration

Below is the Terraform code used to manage this repository:

```hcl
provider "github" {
  token = "use git personal token"
}

resource "github_repository" "git-repository" {
  name        = "Terraform-Code"
  description = "My All Terraform Codes"
  visibility  = "public"
  auto_init   = "true"
}

