🛡️ Project 02: Transaction Monitoring "Watchtower" Dashboard

📌 Project Overview

This project simulates a Transaction Monitoring System (TMS) Rule Engine designed to detect financial crime typologies specific to the UAE banking sector.

Unlike standard "out-of-the-box" monitoring, this system demonstrates the Calibration & Tuning process required to reduce False Positives while maintaining regulatory coverage.

Live Demo: Launch Watchtower Dashboard

Status: ✅ Active Detection

⚙️ Detection Logic (The "Brain")

The system runs real-time checks against three calibrated rules:

🔴 Rule 1: Sanctions Screening (Critical)

Logic: Checks beneficiary country against a simulated "Sanctions List" (North Korea, Iran).

Regulatory Basis: Cabinet Decision No. 74 of 2020 (Terrorist List Regulation).

Action: Immediate "Critical" Alert (Asset Freeze simulation).

🟠 Rule 2: Structuring / Smurfing (High)

Logic: Flags cash deposits between AED 40,000 and AED 49,999.

Why this range? The mandatory reporting threshold in the UAE is AED 55,000. Criminals often deposit just below this limit to avoid detection.

Action: "High" Alert for investigation.

🟡 Rule 3: Velocity Check (Medium)

Logic: Flags accounts with >5 outbound transfers in <60 minutes.

Typology: Indicates "Pass-Through Accounts" (Layering phase of Money Laundering).

Action: "Medium" Alert for review.

📂 Project Artifacts

tm_dashboard.html: The source code for the simulation engine.

Rule_Tuning_Methodology.pdf: A technical memo explaining how I calibrated the thresholds to achieve a 65% True Positive rate.

🚀 How to Run the Simulation

Click the Live Demo link above.

Click the blue "Run Batch Simulation" button.

Watch the "Live Feed" populate with random transactions.

Observe the "Alerts Queue" catch suspicious activity based on the rules above.
