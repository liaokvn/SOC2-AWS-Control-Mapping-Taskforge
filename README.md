# SOC2-AWS-Control-Mapping-Taskforge
SOC 2 Common Criteria mapped to AWS cloud configurations (MFA, encryption, CloudTrail, IAM, backups) for a SaaS startup

# SOC 2 Control Mapping to AWS Cloud Environment — TaskForge

A self-directed GRC project mapping SOC 2 Common Criteria (CC1–CC9) to specific AWS cloud configurations, demonstrating the technical fluency that lets a GRC analyst work directly with engineering teams rather than relying solely on policy-level documentation.

## ⚠️ Current Status: Illustrative / Not Yet Executed on a Live Environment

This project was built as a **Control Implementation Guide** rather than a completed audit evidence package. I do not currently have an active AWS account, so the AWS console images in this guide are **illustrative mockups**, clearly labeled as such throughout the document — not real screenshots. The guide documents exactly what I would configure and capture once I have environment access, so it can be completed with real evidence without rewriting any of the underlying analysis.

This distinction matters and is something I want to be upfront about: the value of this project is in the control mapping and technical reasoning, not in a fabricated claim of hands-on execution I haven't yet performed.

## Project Summary

This project maps five common AWS technical configurations to specific SOC 2 Common Criteria for **TaskForge**, a fictional project management SaaS application hosted on AWS. Rather than treating SOC 2 compliance as a policy-only exercise, the project demonstrates the technical side of GRC work: translating an abstract AICPA criterion into an exact, verifiable cloud configuration.

1. **AICPA criteria reference** — summarizing all nine Common Criteria series (CC1–CC9) from official AICPA-aligned sources
2. **Control-to-configuration mapping** — mapping MFA, S3 encryption, CloudTrail logging, IAM least-privilege policies, and automated backups to their specific SOC 2 criteria (concentrated in CC6 and CC7, the most evidence-intensive series)
3. **Step-by-step implementation guide** — exact AWS console steps for each control, written to be executed by a future version of this project once environment access exists
4. **Illustrative evidence mockups** — AWS console illustrations clearly labeled as mockups, showing what completed evidence should look like
5. **Summary control matrix** — a clean, audit-style table tying each control to its SOC 2 criteria, AWS implementation, and expected evidence type

## Deliverables

| File | Description |
|---|---|
| `TaskForge_SOC2_AWS_Control_Guide.docx` / `.pdf` | Full guide: AICPA CC1–CC9 reference, 5 control implementations with illustrative mockups, summary control matrix, and evidence collection notes |

## What I Did

- Researched the AICPA SOC 2 Common Criteria structure (CC1–CC9, including how many specific criteria fall under each series) from current public sources rather than relying on memory
- Selected five technical AWS configurations explicitly named in the project brief (MFA, S3 encryption, CloudTrail, IAM policies, backups) and mapped each to the specific CC criteria it satisfies, rather than vaguely gesturing at "security"
- Identified that all five configurations cluster into CC6 (Logical and Physical Access Controls) and CC7 (System Operations) — and explained *why*, rather than treating that pattern as a coincidence
- Wrote exact, executable AWS console steps for each control (specific menu paths, specific settings to enable, specific verification steps) so this guide is immediately actionable once I have environment access
- Built illustrative AWS console mockups for all five controls, deliberately and clearly labeled as mockups rather than real screenshots, including realistic technical details (e.g., scoped IAM policy JSON, a CloudTrail event log showing the other four controls being configured)
- Connected this project back to two earlier projects in this portfolio: the S3 public-bucket risk identified in the BudgetWise risk register, and the backup-testing lesson from the Meridian incident response plan — showing the portfolio's projects build on each other rather than existing in isolation
- Wrote evidence collection notes explaining the difference between SOC 2 Type I (design) and Type II (operating effectiveness over time) evidence requirements, since a single screenshot only ever proves the former

## What I Learned

- **Most hands-on cloud security work concentrates in two SOC 2 criteria.** CC6 and CC7 cover access control and system operations respectively, and that's where nearly all console-level technical work lives. CC1–CC5 and CC8–CC9 are real and important, but they're demonstrated through policy, process, and governance documentation, not button-clicks — a distinction that matters when explaining to an engineer *why* a particular control matters to an audit.
- **A control mapping is only useful if it's specific.** "This relates to access control" is not a mapping. "This satisfies CC6.3, which requires authorizing access based on job function" is a mapping an auditor could actually test against.
- **Evidence has a shelf life.** A SOC 2 Type II report requires proof that a control operated effectively over 6–12 months, not just that it was configured once. A single screenshot is necessary but not sufficient — this reframed how I think about "evidence" as something that needs a collection cadence, not a one-time capture.
- **Honesty about gaps is itself a GRC skill.** Recognizing that I couldn't ethically present mockups as real audit evidence — and choosing instead to clearly label them and build a guide for future real execution — mirrors exactly the kind of integrity a GRC analyst is expected to bring to actual audit evidence collection, where overstating control maturity is a real and serious professional risk.
-
