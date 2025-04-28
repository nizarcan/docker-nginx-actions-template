# Docker NGINX Actions Template

A ready-to-deploy Docker template with NGINX for static sites and pre-configured GitHub Actions workflows for automated builds and releases.

## Purpose

This repository serves primarily as a **template** for creating new Docker applications that leverage reusable GitHub Actions workflows. Instead of duplicating CI/CD configuration across multiple repositories, this template connects to centralized workflows.

## How It Works

1. This template uses the reusable workflows from your `reusable-github-actions` repository
2. When you create a new app from this template, it automatically includes the correct workflow references
3. Your apps maintain consistent build, versioning, and deployment processes
4. Updates to workflows happen in one place and apply to all derived applications

## Configuration

See the `.github/workflows/build-and-deploy.yml` file for the workflow reference configuration. This workflow calls the reusable workflow in your central actions repository.