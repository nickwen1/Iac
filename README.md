# Iac

# Azure IaC GRC Scan

## 1. Scan details
- Scan ID:
- Assessment date:
- Assessor / reviewer:
- Repository / commit:
- Deployment environment / subscription:
- Frameworks: ☐ Azure Security Benchmark ☐ NIST CSF ☐ ISO 27001 ☐ SOC 2 ☐ Other:
- Overall status: ☐ Pass ☐ Pass with findings ☐ Fail ☐ Not assessed

## 2. Scope
- In-scope IaC: Azure Policy JSON, Bicep, Terraform, deployment pipelines
- In-scope services: Azure OpenAI, networking/private DNS, Defender for Cloud, Key Vault, logging/monitoring
- Out-of-scope:
- Scan methods/tools:
- Exceptions approved:

## 3. Control and evidence matrix

| ID | Control / check | Expected result | Status | Evidence / file and line | Finding ID | Owner |
|---|---|---|---|---|---|---|
| AOAI-01 | Azure OpenAI public network access | Disabled where private connectivity is required | ☐ Pass ☐ Fail ☐ N/A | | | |
| AOAI-02 | Azure OpenAI private endpoint | Configured and connected to the intended VNet | ☐ Pass ☐ Fail ☐ N/A | | | |
| AOAI-03 | Private DNS | Private endpoint name resolution is configured and validated | ☐ Pass ☐ Fail ☐ N/A | | | |
| AOAI-04 | Authentication and authorization | Approved identity-based access; no embedded credentials | ☐ Pass ☐ Fail ☐ N/A | | | |
| AZP-01 | Azure Policy definitions | Definitions are valid, scoped correctly, and use appropriate effects | ☐ Pass ☐ Fail ☐ N/A | | | |
| AZP-02 | Policy assignment and enforcement | Required policies are assigned; exemptions are documented and approved | ☐ Pass ☐ Fail ☐ N/A | | | |
| DEF-01 | Defender for Cloud plans | Required plans are enabled at the intended scope | ☐ Pass ☐ Fail ☐ N/A | | | |
| DEF-02 | Security recommendations | Relevant recommendations are reviewed, assigned, and tracked | ☐ Pass ☐ Fail ☐ N/A | | | |
| KV-01 | Key Vault authorization | RBAC is used as intended; access is least-privilege | ☐ Pass ☐ Fail ☐ N/A | | | |
| KV-02 | Key Vault network access | Public access is disabled or restricted to the approved design | ☐ Pass ☐ Fail ☐ N/A | | | |
| KV-03 | Key Vault recovery protections | Soft delete and purge protection meet the baseline | ☐ Pass ☐ Fail ☐ N/A | | | |
| LOG-01 | Diagnostic settings | Required platform and security logs are sent to the approved destination | ☐ Pass ☐ Fail ☐ N/A | | | |
| IaC-01 | Secret handling | No credentials, keys, or sensitive values are committed in plaintext | ☐ Pass ☐ Fail ☐ N/A | | | |
| IaC-02 | Validation and scanning | IaC validation and security checks run before deployment | ☐ Pass ☐ Fail ☐ N/A | | | |

Status key: Pass = meets requirement; Fail = gap found; N/A = not applicable, with rationale; Not assessed = evidence unavailable.

## 4. Findings

| Finding ID | Severity | Control ID | Description / evidence | Risk and impact | Recommended remediation | Owner | Due date | Status |
|---|---|---|---|---|---|---|---|---|
| | ☐ Critical ☐ High ☐ Medium ☐ Low | | | | | | | |

## 5. Risk and disposition
- Inherent risk:
- Residual risk:
- Treatment: ☐ Remediate ☐ Accept ☐ Transfer ☐ Avoid
- Risk owner:
- Acceptance rationale / approval:
- Target remediation date:

## 6. Summary and sign-off
- Controls passed / assessed:
- Open findings by severity:
- Key exceptions or limitations:
- Required actions:
- Assessor / date:
- Reviewer / date:
- Risk owner approval / date:

For each result, record the relevant IaC file and line, policy assignment or compliance evidence, and scan output. Don’t treat a passing template scan as proof that the deployed Azure resources are compliant; validate deployed configuration separately.
