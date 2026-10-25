### Compliance.tf

The Terraform control layer for AWS. Compliance.tf makes a Terraform estate provable: the controls are built into the modules, held before apply, and mapped to the clauses your auditor asks about.

**Our modules:** the 51 maintained [terraform-aws-modules](https://github.com/terraform-aws-modules), served with controls through a framework endpoint or your org endpoint. One source line, same inputs and outputs, no state migration.

**Your modules:** any public registry module for AWS through the compliance.tf endpoint, and your own modules from a private source, returned with controls applied. **ctfkit by compliance.tf** scans and reports on modules without patching them.

**How it works:** change the module source from the public registry to `soc2.compliance.tf` (or `pcidssv40.compliance.tf`, `hipaa.compliance.tf`, or your org endpoint) and run `terraform init`. The controls are in the module before apply, and each one maps to the SOC 2, PCI DSS, HIPAA, NIST 800-53 and CIS clauses it serves. Org rules, promotion gates and an audit trail come with your org endpoint.

Works with Terraform 1.0 or later and OpenTofu 1.6 or later. Modules for AWS; control and framework references for AWS, Azure and Google Cloud; Azure and Google Cloud modules planned for Q1 2027.

[compliance.tf](https://compliance.tf) | [Docs](https://compliance.tf/docs/) | [Blog](https://compliance.tf/docs/blog/) | [AWS Marketplace](https://aws.amazon.com/marketplace/seller-profile?id=seller-k6xaeawuwu2mu)
