# Valdoria-Votes-Investigation
This repository documents a hands‑on cybersecurity investigation into a phishing‑driven compromise of Valdoria's air‑gapped voting systems. It covers reconnaissance, credential theft, lateral movement, AI chatbot exploitation, and social engineering.
## 📱 LinkedIn Post Summary

*Below is the professional summary I shared on LinkedIn about this investigation:*

---

**🔍 Case Study: Valdoria Votes – A Digital Election Investigation**

I recently completed a deep‑dive investigation into an attempted breach of Valdoria's air‑gapped voting systems. What started as a hacker's boast online turned into a full‑scale threat hunt spanning reconnaissance, phishing, credential theft, and social engineering.

**Here's what the investigation uncovered:**

🕵️ **Reconnaissance** – The attacker searched for new hires, security measures, and voting machine technical details – all from a separate IP to avoid detection.

🎣 **Phishing Infrastructure** – Fraudulent domains were registered (`valdoriavotesgov.com`, `shadow-hackers-r.us`), hosted on attacker‑controlled IPs.

🔐 **Credential Theft** – A newly hired employee, Anderson Snooper, fell victim to the phishing site. Within hours, the attacker logged into his account.

📧 **Lateral Movement** – Posing as Snooper, the attacker emailed a colleague asking how to access voting machines, then probed internal systems until finding an AI chatbot.

🤖 **AI Intelligence Gathering** – The chatbot revealed critical information: voting machines are air‑gapped, votes are manually counted, and the vendor (Dominos Voting Systems) only communicates with the Election Commissioner.

👤 **Account Takeover** – The attacker socially engineered the helpdesk to reset the Election Commissioner's password, gaining access to Arrack Bobama's account.

📎 **The Payload** – Posing as Bobama, the attacker emailed the vendor and received a sensitive PDF: **`ValdoriaVotingMachinesNetworkGuide.pdf`** – a roadmap to the very systems they claimed to have breached.



**Why this matters:**

Air‑gapped systems are not immune. The human element remains the most vulnerable attack surface. Strong documentation, thorough log analysis, and a structured investigation approach made it possible to trace every step of this attack chain – from initial recon to the final PDF.

This investigation reinforced my belief in the power of **methodical documentation**. Using a structured investigation log (with clear sections for IOCs, timeline, findings, and open items) kept me organized and ensured no evidence was missed.



**Key takeaways for defenders:**
✅ Enable MFA everywhere – it would have stopped both account takeovers.
✅ Monitor for anomalous outbound traffic – even to seemingly legitimate domains.
✅ Train employees on phishing – Snooper was a new hire, exactly the target the attacker researched.
✅ Restrict AI chatbot access – sensitive information should never be disclosed without verification.

---

**#Cybersecurity #IncidentResponse #ThreatHunting #DFIR #ElectionSecurity #Phishing #SocialEngineering #InfoSec**

💡 *This investigation was part of a hands‑on lab simulating real‑world election interference. The names and data are fictional, but the techniques are very real.*
