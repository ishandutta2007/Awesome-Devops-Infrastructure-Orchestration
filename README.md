# Awesome-Devops-Infrastructure-Orchestration

markdown

## Top DevOps & Infrastructure Orchestration Ecosystem



**Curated List of SaaS/Hosted Platforms & Open-Source GitHub Projects**  

*Focused on Infrastructure-as-Code (IaC), Declarative Cloud Provisioning, TACOS (Terraform Automation & Collaboration Software), Configuration Management & GitOps Orchestration*  

**Last updated: November 2026**



This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **DevOps & Infrastructure Orchestration**. These tools define, plan, provision, drift-detect, govern, and orchestrate cloud and on-premise infrastructure across AWS, Azure, GCP, Kubernetes, and bare-metal datacenters using declarative Infrastructure-as-Code (IaC), policy-as-code, and automated CI/CD pipelines.



**Examples** include Terraform Cloud (HCP Terraform), Pulumi Cloud, Spacelift, env0, Scalr, AWS CloudFormation, Azure Resource Manager (Bicep), Google Cloud Deployment Manager / Infrastructure Manager, Octopus Deploy, HashiCorp Cloud Platform (HCP), and ogulcancelik/herdr (the category leaders and popular runtimes). 



**Open-source emphasis**: This section is heavily expanded with every major active project for open-source Infrastructure-as-Code engines (`OpenTofu`, `Pulumi`, `Crossplane`, `Terragrunt`, `CDKTF`), self-hosted Terraform/OpenTofu automation & GitOps runners (`Atlantis`, `Digger`, `Terramate`, `ogulcancelik/herdr`), and configuration management & policy-as-code suites (`Ansible`, `Nix / NixOS`, `Open Policy Agent`) — ideal for DevOps engineers, SREs, cloud architects, and platform teams.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Support & Share](#support--share)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform | Company Valuation / Revenue | Starting Tier Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Azure Resource Manager & Azure Deployment Environments](https://microsoft.com)** | **Valuation: ~$3.1T** (Market Cap) / Revenue: ~$245B | **$0.00 / mo** (Free platform management; underlying Azure infrastructure resources billed as used) | **Free forever**: ADE service is free (subject to operational defaults of 200 deployment runtime mins/mo per region and 1 GB storage per environment) | Native Microsoft Azure deployment and governance layer orchestrating cloud resources via ARM JSON templates, Bicep, and role-based subscription blueprints. |
| **[AWS CloudFormation & AWS CDK](https://amazon.com)** | **Valuation: ~$2.1T** (Market Cap) / Revenue: ~$575B | **$0.00 / mo** (No charge for standard `AWS::*` resources; pay only for provisioned infrastructure. Custom extensions at $0.0009/handler op beyond free tier) | **Free forever**: Unlimited standard `AWS::*` resource management; 1,000 handler operations per month per account free for registry/custom extensions & hooks | Native AWS declarative infrastructure orchestration service modeling and provisioning AWS resources via YAML/JSON templates, StackSets, and programmatic CDK constructs. |
| **[Google Cloud Infrastructure Manager](https://google.com)** | **Valuation: ~$2.0T** (Market Cap) / Revenue: ~$307B | **$0.00 / mo** (Free for Terraform <=v1.5.7; for Terraform >=v1.16.5, $0.000000032/resource-second / ~$1.00/resource-year beyond 500 free resources) | **Free forever**: Unlimited resources on Terraform <=v1.5.7; first 500 concurrent managed resources per month (1.314B resource-seconds) free at $0.00 for Terraform >=v1.16.5 | Managed Google Cloud service automating deployment, state management, and drift tracking of GCP resources using Terraform/OpenTofu blueprints. |
| **[HCP Terraform & HashiCorp Cloud Platform (HCP)](https://hashicorp.com)** | **Valuation: $6.4B** (Acquired by IBM) / Revenue: ~$600M | **$0.10 / mo per managed resource** (Essentials plan, billed hourly at ~$0.00013/RUM) | **Free forever**: Up to 500 managed resources (RUM), unlimited users, 1 concurrent run, remote execution, and private module registry | Managed cloud Infrastructure-as-Code platform providing remote state locking, private module registries, drift detection, Sentinel/OPA policy checks, and HCP Vault/Consul integration. |
| **[Octopus Deploy](https://octopus.com)** | **Valuation: ~$625M** / Revenue: ~$83.4M ARR | **$360.83 / mo** ($4,330 / yr billed annually for Professional tier) | **Free forever**: Up to 10 targets/machines, 10 projects, 10 tenants, 10 users, and 1 space. Also provides a 30-day Enterprise free trial | Enterprise continuous delivery and runbook orchestration platform coordinating complex multi-environment deployments across Kubernetes, VMs, cloud PaaS, and hybrid infrastructure. |
| **[Pulumi Cloud](https://pulumi.com)** | **Valuation: ~$390M** / Revenue: ~$20M ARR ($99M funding) | **$40.00 / mo** (Team Essentials plan, includes up to 500 managed resources) | **Free forever**: Individual edition includes 1 user, unlimited managed resources, unlimited projects/stacks, and 500 deployment/workflow minutes/mo (1 concurrency) | Managed backend for Pulumi IaC offering encrypted state management, audit logs, Pulumi ESC (Environments, Secrets, and Configuration), and AI-assisted infrastructure authoring. |
| **[Spacelift](https://spacelift.io)** | **Valuation: ~$250M - $500M** / Revenue: ~$15M ARR ($73.6M funding) | **$399.00 / mo** (Starter tier for up to 10 users and 2 public workers) | **Free forever**: Up to 2 users, 1 API key, core IaC workflows (Terraform, OpenTofu, Pulumi, CloudFormation, Ansible), and VCS integration. Also offers a 14-day free trial of paid tiers | Sophisticated CI/CD and infrastructure orchestration platform supporting OpenTofu, Terraform, Pulumi, CloudFormation, Ansible, and Kubernetes with Rego policy-as-code and stack dependencies. |
| **[env0](https://env0.com)** | **Valuation: ~$72M** / Revenue: ~$5.5M ARR ($42M funding) | **$0.00 / mo** (Free tier; paid Cloud Navigator / Cloud Pilot enterprise tiers start at custom quote based on active environments) | **Free forever**: Up to 30 active environments, 250 runs/mo, 1 concurrent deployment, unlimited users, and 1 self-hosted agent | Enterprise self-service cloud infrastructure automation platform featuring dynamic cost estimation, RBAC governance, drift detection, and multi-framework IaC workflows. |
| **[ControlMonkey](https://controlmonkey.io)** | **Valuation: ~$25M - $50M** ($7M Seed funding) | **$800.00 / mo** (Essentials tier for automated drift detection and IaC management) | **Free tier / trial**: Permanent Free Resilience Assessment (read-only cloud & SaaS posture evaluation); custom POC / demo free trial upon booking sales evaluation | Cloud governance and Terraform/OpenTofu automation platform featuring one-click legacy cloud-to-IaC code generation, continuous drift alerts, and disaster-recovery snapshots. |
| **[Scalr](https://scalr.com)** | **Valuation: Bootstrapped / VC** / Revenue: ~$5.3M ARR ($7.35M Series A) | **$0.99 / run** (Pay-as-you-go per apply/dry run beyond the monthly free allowance) | **Free forever**: Up to 50 runs per month with drift detection and Open Policy Agent (OPA) integration included | Hierarchical Terraform and OpenTofu remote operations backend designed for decentralized enterprise teams with OPA policy enforcement and federated module registries. |





## Open-Source GitHub Projects



- **[ogulcancelik/herdr](https://github.com)**  

  Open-source DevOps and infrastructure orchestration utility engineered for streamlined environment coordination, automated deployment workflows, and modular infrastructure operations.



- **[OpenTofu (`opentofu/opentofu`)](https://github.com)**  

  Flagship Linux Foundation open-source (MPL-2.0) fork of Terraform providing full HCL compatibility, client-side state encryption, early variable evaluation, and community-driven providers.



- **[Pulumi (`pulumi/pulumi`)](https://github.com)**  

  Modern open-source Infrastructure-as-Code SDK enabling developers to define, test, and orchestrate cloud infrastructure using TypeScript, Python, Go, C#, Java, and YAML.



- **[Crossplane (`crossplane/crossplane`)](https://github.com)**  

  CNCF open-source control-plane framework extending Kubernetes into a universal cloud orchestrator so platform teams can compose self-service infrastructure APIs.



- **[Atlantis (`runatlantis/atlantis`)](https://github.com)**  

  Battle-tested open-source self-hosted application for automating OpenTofu and Terraform pull-request workflows—running `plan` and `apply` directly from GitHub, GitLab, or Bitbucket comments.



- **[Digger (`diggerhq/digger`)](https://github.com)**  

  Open-source IaC orchestration tool that runs OpenTofu/Terraform plans and applies natively inside your existing CI compute (GitHub Actions, GitLab CI) without duplicating cloud secrets.



- **[Terragrunt (`gruntwork-io/terragrunt`)](https://github.com)**  

  Essential open-source thin wrapper for OpenTofu and Terraform that keeps configurations DRY across multi-account, multi-region environments and orchestrates module dependency graphs.



- **[Terramate (`terramate-io/terramate`)](https://github.com)**  

  High-performance open-source IaC orchestrator and code generator featuring change detection, DAG stack execution, drift checks, and multi-IaC support.



- **[Ansible (`ansible/ansible`)](https://github.com)**  

  Industry-standard open-source agentless IT automation and configuration management engine orchestrating server provisioning, OS hardening, and multi-tier application rollouts over SSH/WinRM.



- **[Azure Bicep (`Azure/bicep`) & AWS CDK (`aws/aws-cdk`)](https://github.com)**  

  Official open-source domain-specific language (`Bicep`) and multi-language framework (`AWS CDK`) compiling high-level abstractions into native cloud templates.



- **[Open Policy Agent — OPA (`open-policy-agent/opa`) & Checkov (`bridgecrewio/checkov`)](https://github.com)**  

  Leading open-source policy-as-code (`Rego`) and static IaC security/compliance scanners preventing misconfigurations in Terraform, OpenTofu, CloudFormation, and Kubernetes manifests before apply.



### Additional Strong Open-Source Options



- **[Nix & NixOS / Colmena (`zhaofengli/colmena`)](https://github.com)** for purely functional, bit-for-bit reproducible declarative server builds and multi-host fleet orchestration over SSH.

- **[Packer (`hashicorp/packer`)](https://github.com)** for open-source automated creation of identical golden machine images (AMIs, Azure VHDs, GCP images, QEMU/Proxmox templates) from a single JSON/HCL config.

- **[CDK for Terraform — CDKTF (`hashicorp/cdk-terraform`)](https://github.com)** for writing Terraform and OpenTofu infrastructure definitions in TypeScript, Python, Java, C#, or Go.

- **[TofuController / Flux TF-Controller (`flux-iac/tofu-controller`)](https://github.com)** for a Kubernetes GitOps operator enabling continuous reconciliation and self-healing drift correction of OpenTofu/Terraform resources.

- **[Infracost (`infracost/infracost`)](https://github.com)** for an open-source FinOps CLI showing real-time cloud cost diffs directly inside pull requests before infrastructure changes are applied.



**Frameworks for building custom systems**: Combine **OpenTofu + Terragrunt** (or **Pulumi**) for multi-environment declarative provisioning, **Atlantis** or **Digger** for pull-request GitOps orchestration, **Checkov + OPA + Infracost** for automated security/cost guardrails, and **Ansible** for post-provisioning OS configuration.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Support & Share



If you find this curated list helpful, consider supporting the project:



- ⭐ **Star this repository** to help others discover it.

- 🍴 **Fork & Share** it with your team, friends, or community on X/Twitter, LinkedIn, and Reddit.

- ☕ **Buy me a coffee / Sponsor** my open-source work on [GitHub Sponsors](https://github.com) — featuring tiers for profile badges, README shoutouts, logo placements, and prioritized bug fixes/features!



[![Sponsor @ishandutta2007](https://shields.io)](https://github.com)



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

Use code with caution.

• Note that Terraform (1.6+) and Packer use the Business Source License (BSL 1.1), whereas OpenTofu (MPL-2.0), Pulumi (Apache 2.0), Crossplane (Apache 2.0), Atlantis (Apache 2.0), and Ansible (GPL-3.0) are OSI-approved open-source projects.

• Infrastructure state files (.tfstate) frequently contain sensitive database passwords, TLS private keys, and cloud tokens; always store state in encrypted remote backends with strict IAM access controls and client-side state encryption enabled.

Made for DevOps engineers, SREs, cloud architects, platform teams, and open-source contributors.

Let's make infrastructure orchestration and Infrastructure-as-Code more open, auditable, and reproducible.
