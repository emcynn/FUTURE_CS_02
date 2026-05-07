# FUTURE_CS_02
> Task 02: Phishing Analysis &amp; Risk Evaluation Project

## 📌 Project Overview
This repository contains a comprehensive analysis of various email threats, ranging from highly sophisticated phishing to multi-stage social engineering. The goal of this project is to strengthen organizational defenses by uncovering attacker infrastructure and providing actionable mitigation strategies for non-technical users.

## 🛠 Tools & Methodology
### Tools Used
- Google Admin Toolbox (Messageheader): For parsing raw headers to verify SPF, DKIM, and DMARC status.- 
- MXToolbox: To analyze email routing, sender IP reputation, and blacklist status.

### Analysis Approach
The project follows a standard SOC (Security Operations Center) Triage workflow:
1. Ingestion: Sourcing authentic phishing samples from verified security archives.
2. Header Analysis: Inspecting metadata to detect spoofing and delivery path discrepancies.
3. Content Inspection: Identifying psychological triggers (Fear, Urgency, Ego-bait) and mismatched visual branding.
4. Risk Categorization: Classifying emails into Phishing, Suspicious, or Safe based on technical and contextual indicators.

## 🔍 Samples & Resources
The analysis was performed using real-world samples sourced from the following verified archives:
- **Phishing Sample (MFA/Account Trap)**
  - Resource: phishing_pot repository by rf-peixoto.
  - Reference: [phishing_pot/email/sample-10.eml](https://github.com/rf-peixoto/phishing_pot/blob/main/email/sample-10.eml)
- **Suspicious Sample (AI-Generated Request)**
  - Resource: UC Berkeley Information Security Office.
  - Reference: [Phony AI-Generated LLM Request Messages | Berkeley ISO](https://security.berkeley.edu/news/phony-ai-generated-llm-request-messages)
- **Safe Sample (Google Security Alert)**
  - Resource: Standardized Google Account Security notification.

## 🚀 Key Insights
- **Technical Failures**: Even "clean" looking emails often fail basic authentication protocols like SPF and DKIM.
- **Social Engineering**: Attackers are increasingly moving from "Panic" (Phishing) to "Rapport" (Suspicious/AI-generated) to bypass traditional filters.
- **Verification**: Legitimate alerts are characterized by transparency, TLS encryption, and lack of coercive calls to action.

