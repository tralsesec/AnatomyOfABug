# #! Anatomy of a Bug

> **Autopsy of a Zero-Day.**
> High-fidelity technical analyses of critical vulnerabilities, kernel exploits, and architectural failures.

<div align="center">

![License: CC BY-ND 4.0](https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg)
![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen.svg)
![Author: @tralsesec](https://img.shields.io/badge/Author-%40tralsesec-blue.svg)

</div>

## 📜 Manifesto

**#! Anatomy of a Bug** is a weekly research series dedicated to deconstructing the most sophisticated exploits in the wild. We move beyond the "what" and focus on the "how" and "why."

Each report follows a strict forensic structure:
1.  **The Patient:** The target system and its architectural context.
2.  **The Diagnosis:** The precise root cause (e.g., Integer Overflow, Race Condition, Logic Flaw).
3.  **The Kill-Chain:** Step-by-step reconstruction of the exploit flow (from entry to root/kernel).
4.  **The Fix:** Code-level remediation and developer takeaways.

## 📂 Case Files

| ID | Case Title | CVE(s) | Target | Severity |
| :--- | :--- | :--- | :--- | :--- |
| **#006** | **Cisco AsyncOS Quarantine Collapse** | `CVE-2025-20393` | Cisco Secure Email Gateway | **10.0** |
| **#005** | **The Fortinet 0days** | `CVE-2025-64446`<br>`CVE-2025-58034` | FortiWeb WAF | **9.8** |
| **#004** | **"Liquid Glass" Zero-Days** | `CVE-2025-14174`<br>`CVE-2025-43529`<br>`CVE-2025-46285` | iOS 26 (WebKit/Kernel) | **10.0** |
| **#003** | **The Firefox IPC Sandbox Escape** | `CVE-2025-2857` | Mozilla Firefox | **10.0** |
| **#002** | **Lazarus 0-Day** | `CVE-2024-21338` | Windows AppLocker (`appid.sys`) | **7.8** |
| **#001** | **React2Shell** | `CVE-2025-55182` | React Server Components | **10.0** |

*> Full archive available in the `/pdfs` directory.*

## 🔬 Methodology

This repository serves as a knowledge base for Exploit Developers, Security Researchers, and Reverse Engineers. The goal is not just to document the vulnerability, but to understand the **mindset** of the attacker and the **design failures** of the defender.

Tools and techniques often referenced:
* **Static Analysis:** Binary diffing, control flow graph reconstruction.
* **Dynamic Analysis:** Kernel debugging, heap spraying visualization.
* **De-obfuscation:** Unpacking custom malware layers and polyglott payloads.

## ⚖️ License & Usage

This work is licensed under a **Creative Commons Attribution-NoDerivatives 4.0 International License (CC BY-ND 4.0)**.

**You are free to:**
* **Share:** Copy and redistribute the material in any medium or format.
* **Commercial Use:** You may use these reports for educational or commercial training purposes.

**Under the following terms:**
* **Attribution:** You must give appropriate credit to **@tralsesec**, provide a link to the license, and indicate if changes were made (note: changes are not permitted under ND).
* **NoDerivatives:** If you remix, transform, or build upon the material, you may not distribute the modified material. The integrity of the analysis must remain intact.

See the [LICENSE](./LICENSE) file for the full legal text.

---

> *"Security is not inherited. Every layer must defend itself."* — AOAB #6
