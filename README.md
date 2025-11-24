📌 Project Overview

This project demonstrates a Risk-Based Approach (RBA) to Anti-Money Laundering (AML) compliance, designed specifically for the UAE regulatory environment. It operationalizes the requirements of Federal Decree-Law No. (20) of 2018 and Cabinet Decision No. (10) of 2019.

The repository contains two key artifacts:

Interactive Customer Risk Assessment Matrix (CRAM): A web-based tool that calculates Inherent Risk scores using a weighted-average algorithm.

Mock Suspicious Activity Report (SAR): A procedural document demonstrating the analysis and reporting of "Structuring" typologies to the UAE Financial Intelligence Unit (FIU).

🛠️ Technical & Legal Logic

The Risk Engine is built to automate the mandates of Article 4 (Risk Identification) of Cabinet Decision No. 10.

1. Risk Weighting Methodology

The tool calculates risk based on four statutory pillars, weighted by their impact on financial crime vulnerability:

Risk Factor

Weight

Legal Basis (Cabinet Decision No. 10)

Customer Type

30%

Article 15: Mandates specific EDD for PEPs and complex structures.

Geography

30%

Article 22: Requires enhanced measures for High-Risk Jurisdictions (FATF list).

Product/Service

25%

Article 4.1.a: Assessing product vulnerability (e.g., Cash vs. Wire).

Channel

15%

Article 4.1.a: Face-to-face vs. Non-face-to-face onboarding risks.

2. Decision Logic

Low Risk (< 2.0): Triggers Simplified Due Diligence (SDD) as per Article 4.3.

High Risk (> 3.5): Automatically triggers Enhanced Due Diligence (EDD) requirements, including:

Source of Wealth (SOW) corroboration.

Senior Management Approval (Article 15).

UBO Unwrapping (Article 9 - 25% ownership threshold).

📂 Contents

risk_matrix.html: The source code for the assessment engine.

SAR_Analysis_Report.pdf: A sample investigation into high-velocity cash deposits suspected of placement/layering.

🚀 How to Use

Download risk_matrix.html.

Open the file in any web browser (Chrome/Edge).

Select different client parameters (e.g., "PEP" + "High Risk Jurisdiction") to see the automated risk scoring and compliance triggers.

Disclaimer: This project is a portfolio demonstration of compliance logic and is not a live production system.
