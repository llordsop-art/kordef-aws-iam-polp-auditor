# kordef-aws-iam-polp-auditor

> **Zero-Trust AWS IAM & S3 Posture Auditor** — Detects wildcard (*) privileges, iam:PassRole escalation paths, and public S3 exposures for SOC 2 CC6.1 readiness.

Developed by **KOR DEF (Zero-Trust Cloud & AI Security Architecture)**.

---

## 🔒 Key Capabilities

- **IAM Wildcard Policy Detection**: Scans customer-managed and inline IAM policies for excessive `Action: "*"` or `Resource: "*"` bindings.
- **Privilege Escalation Path Analysis**: Identifies dangerous permission combinations such as `iam:PassRole` with `ec2:RunInstances` or `lambda:CreateFunction`.
- **S3 Public Exposure & Encryption Audit**: Verifies S3 Bucket ACLs, Block Public Access settings, and default SSE-KMS / SSE-S3 encryption posture.
- **SOC 2 CC6.1 Readiness Assessment**: Generates structured JSON/HTML compliance reports mapped to SOC 2 Logical Access controls.

---

## ⚡ Quick Start

```bash
# Clone repository
git clone repo-url
cd kordef-aws-iam-polp-auditor

# Run audit
python3 auditor.py --profile production --output report.json
```

---

## 🛡️ About KOR DEF
**KOR DEF** provides cloud security architecture, zero-trust engineering, and compliance automation.
- **Website**: kordefence.net
- **Contact**: info@kordefence.com
