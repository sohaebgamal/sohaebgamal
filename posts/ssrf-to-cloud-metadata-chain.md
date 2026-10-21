# One URL parameter. One metadata endpoint. Production secrets. ☁️

*Sohaib Gamal · Security QA Engineer & Penetration Tester*

I documented a lab where a simple "fetch image from URL" feature ended with access to a restricted storage bucket. No exploit kit, just a chain of small trust mistakes.

## 🔗 The chain

- An endpoint fetched any URL the user supplied (SSRF)
- The server could reach the cloud instance metadata service
- The metadata service handed out temporary credentials for the instance role
- That role could read a bucket it should never have touched

## 🛠️ What would have broken the chain

- Allowlist the URLs the server may fetch
- Block link-local metadata access from app containers (IMDSv2 with hop limit 1)
- Least-privilege roles: a web role should not read production secrets
- Rotate long-lived keys, and don't leave internal notes publicly readable

## 🎓 Source

Lab environment (TryHackMe), documented as a client-style report: summary, attack chain, remediation.
Full report: [pentest-writeups / cloud-security-fundamentals](https://github.com/sohaebgamal/pentest-writeups/blob/main/emerging-tech/cloud-security-fundamentals.md)

Which of these four fixes do you see missing most often?
