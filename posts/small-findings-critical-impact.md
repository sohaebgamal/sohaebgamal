# Small findings. Critical impact. 🔗

*Sohaib Gamal · Security QA Engineer & Penetration Tester*

One thing I keep seeing in real pentests: nobody gets hacked by a "low severity" bug alone. They get hacked by three of them chained together.

## 🧩 The chain I reported (twice, independently confirmed)

- User enumeration on the login flow
- Missing rate-limiting
- IDOR exposing other users' data

Each one looked minor on its own. Together they became a **CRITICAL** account takeover. 🔴

## 🧠 What I take from it

- Score findings as chains, not in isolation
- Fix the cheapest link first (rate-limiting + generic login errors take hours, not weeks)
- Retest after the fix. A fix is only done when the chain no longer works ✅

## 📉 Result

After remediation, the weighted risk score on that platform dropped by ~80%.

**Focus areas:** `Penetration Testing` · `API Security` · `Access Control` · `Business Logic` · `Burp Suite` · `Python`

🔒 *Based on authorized testing only. No client details shared.*
