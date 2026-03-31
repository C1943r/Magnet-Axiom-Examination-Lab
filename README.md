# [REDACTED] Forensic Examination Report: Homicide Investigation (MCFE)
**Prepared by:** Rocky Wanek   
**Case Type:** Felony Homicide Investigation Simulation  
**Tools:** Magnet Axiom, Magnet GrayKey (Simulated), HashCalc, Passware/Axiom Password Recovery

Note: This documentation was refined using AI-assisted editing to improve clarity and presentation, while maintaining my original analysis and findings.

---

> ### **NDA & CONFIDENTIALITY NOTICE**
> This report is a sanitized summary of a forensic investigation conducted for the **Magnet Certified Forensics Examiner (MCFE)** certification. Pursuant to the Magnet Forensics NDA, all proprietary scenario identifiers, victim/suspect PII, and specific case prompts have been **redacted or scrubbed**. This document is intended to demonstrate technical proficiency in advanced artifact correlation, encryption bypass, and geolocation analysis in a criminal investigative context.

---

## **1. Executive Summary**
A digital forensic examination was performed on two verified forensic images: a **Windows 10 Workstation** and an **iPhone (iOS [REDACTED])**. The objective was to uncover evidence related to a murder investigation, specifically focusing on premeditation, suspect-victim interactions, and the movements of the suspect during the window of the commission of the crime. 

The analysis successfully bypassed device encryption via brute-force, recovered deleted communications, and established a definitive link between Dark Web research into lethal methods and the physical movements of the suspect.

## **2. Technical Methodology & Evidence Integrity**
* **Hash Verification:** Integrity of the evidence was ensured by validating **MD5 and SHA-256 hashes** of the provided E01 and mobile images. All analysis was conducted on forensic copies to ensure the original data remained pristine.
* **Password Recovery & Brute-Force:** Identified multiple encrypted containers on the Windows 10 image. Utilizing **brute-force and dictionary attacks**, I successfully recovered the password for a hidden volume, revealing a digital "manifesto" and planning documents.
* **Mobile Keychain Analysis:** Extracted the **iOS Keychain** to gain access to end-to-end encrypted messaging applications, which were vital for reconstructing the final communications between the suspect and the victim.

## **3. Critical Forensic Findings**

### **Dark Web Activity & Premeditation**
I performed a deep-dive correlation of **Tor browser sessions** to establish intent.
* **Tor Artifact Recovery:** Despite the suspect's attempt to use anonymized browsing, I recovered **.onion** URL fragments from the `pagefile.sys` and unallocated space.
* **Temporal Correlation:** Matched the timestamps of Dark Web searches for [REDACTED - Lethal Methods] with the Windows 10 **System Resource Usage Monitor (SRUM)** and **Network Usage** logs. This proved the suspect was actively researching the crime days before the event.

### **Geolocation & Pattern of Life (iPhone)**
* **Spatial Tracking:** Extracted and mapped GPS coordinates from **Cell Tower (consolidated.db)** and **ZWAUTHLOCATION** artifacts.
* **Crime Scene Proximity:** Established that the suspect’s iPhone was within a 50-meter radius of the crime scene at the time of the incident, contradicting the "alibi" provided in the initial police interview.
* **Post-Incident Movement:** Tracked the suspect’s movement to a secondary location (potential evidence disposal site) immediately following the commission of the crime.

### **Communication Reconstruction**
* **Encrypted App Recovery:** Decrypted and parsed SQLite databases for Signal/WhatsApp.
* **Deleted Content:** Successfully carved for deleted messages in the mobile image, recovering a deleted conversation thread where the suspect lured the victim to the [REDACTED] location under false pretenses.

## **4. Evidence Matrix**

| Artifact Category | Forensic Significance |
| :--- | :--- |
| **$MFT / File Events** | Identified the creation of a "Planning" folder that was wiped using a secure-delete utility. |
| **iOS Frequent Locations** | Proved the suspect had "cased" the victim's residence three times in the week prior to the murder. |
| **Windows UserAssist** | Confirmed the execution of encryption-wiping software and the Tor Browser. |
| **Powerlog (iOS)** | Correlated device charging/usage states to prove the suspect was awake and active during the late-night hours of the crime. |

## **5. Conclusion**
The forensic evidence provides a high-confidence reconstruction of the events leading up to and following the homicide. The combination of **Dark Web session timestamps**, **brute-forced planning documents**, and **GPS location data** provides a comprehensive "digital fingerprint" of premeditation and presence at the scene. This investigation demonstrates the power of cross-platform correlation in modern criminal forensics.

