# Threat Model (Risk-Focused)

## Credible Threat Scenarios
| Threat | Entry Point | Target Asset | Potential Business Impact |
|------|------------|--------------|---------------------------|
| Credential stuffing | Login page | Authentication | Account takeover, fraud losses |
| Phishing | Email/SSO | Employee credentials | Privilege escalation, data exposure |
| Cloud misconfiguration | Public storage / exposed ports | Customer data | Data breach, regulatory penalties |
| Insider misuse | Admin tools | PII / transaction controls | Unauthorized access, fraud |
| Third-party breach | Vendor integration | Customer data | Data leakage, notification obligations |

## Common Weaknesses (Examples)
- MFA not enforced for all users
- Weak password policy or lack of rate-limiting
- Over-permissioned cloud IAM roles
- Incomplete logging (gaps in auth/API logs)
- Alerting thresholds not tuned (late detection)

