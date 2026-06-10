### Compliance.tf

Terraform AWS modules with compliance controls built in.

Each module is a drop-in replacement for its [terraform-aws-modules](https://github.com/terraform-aws-modules) equivalent — same variables, same outputs. The difference: encryption, logging, access controls, and versioning are enforced by the module itself. You can't accidentally deploy non-compliant resources.

**How it works:** change your module source from `terraform-aws-modules` to [`soc2.compliance.tf`](https://soc2.compliance.tf) (or `pcidss`, `hipaa`, `nist`, `iso27001`, `gdpr`, `nis2`, `fedramp`, `cis`). Run `terraform init`. Done. Every framework host is a browsable public registry with module versions, inputs, and outputs.

Works with Terraform, OpenTofu, Terragrunt, and Terramate. No new CLI, no policy agent, no sidecar.

🔗 [compliance.tf](https://compliance.tf) · [Docs](https://compliance.tf/docs/) · [Registry](https://registry.compliance.tf) · [Blog](https://compliance.tf/blog/) · [AWS Marketplace](https://aws.amazon.com/marketplace/pp/prodview-piljg56ndgr2c)
