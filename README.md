# aws-cloud-security-portfolio
Hands-on AWS projects showcasing cloud security, infrastructure as code, and automation. Includes VPCs, IAM, Lambda, Cloudformation, and more.

# AWS Multi‑Account Setup

To align with AWS best practices, I maintain two separate AWS accounts:

- **General Account** – Management & learning environment
- **Production Account** – Isolated environment for production‑like workloads

## Security Measures

- **MFA enabled** on both root users
- **IAM admin users** created in each account with **MFA**
- **Named CLI profiles** (`iamadmin-general`, `iamadmin-production`) for secure access
- **No long‑term credentials** stored in code – all projects use IAM roles or temporary credentials
