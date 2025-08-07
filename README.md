Medication Logging App

A privacy-first, offline-capable mobile application for tracking daily medication intake, side effects, and adherence. Designed for patients, caregivers, and clinicians, with optional data release to pharmaceutical companies only via doctor mediation.

---

🧭 Overview

This app empowers patients to:
- Log medications, doses, and side effects daily
- Receive reminders and review weekly summaries
- Export data for clinical review
- Share validated data with pharmaceutical companies only when approved by a clinician

All data is stored locally and securely on the user's device. No cloud sync. No automatic sharing.

---

👥 Agent Groups

| Role | Capabilities |
|------|--------------|
| Patient | Logs medication, receives reminders, exports data for doctor |
| Caregiver | Assists with logging (if granted access), helps review entries |
| Clinician | Reviews logs, annotates, and releases data externally with patient consent |
| Pharmaceutical Company / Registry | Receives anonymized, validated data via clinician upload |

---

📲 Features

✅ Core Logging

- Add medications manually or via barcode scan
- Auto-fill dosage and schedule from local medication database
- Log side effects with severity, timing, and notes
- Daily reminders for scheduled doses
- Weekly review prompt

📷 Barcode Scanning

- Scan medication packaging to auto-fill name, dose, and schedule
- Works offline using bundled medication database
- Supports EAN/UPC and NHS codes

📁 Export & Review

- Generate encrypted PDF/CSV/JSON summaries
- Export only occurs when patient initiates
- Doctor reviews and confirms before external sharing

🔐 Privacy & Sovereignty

- All data stored locally using encrypted SQLite
- No cloud sync or background sharing
- Role-based access control for caregivers
- Audit trail for all exports and edits

---

🧩 Accessibility

🧑‍🦯 Inclusive Design

- Large text and high-contrast UI modes
- Voice input for logging meds and side effects
- Tap-based logging for users with limited dexterity
- Screen reader support (TalkBack / VoiceOver)
- Optional simplified interface for cognitive accessibility

🧑‍🤝‍🧑 Caregiver Assist Mode

- Patient can grant caregiver access via secure token
- Caregiver can help fill in logs, review entries, and prepare exports

---

🛠️ Technical Architecture

📦 Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | Flutter (Android/iOS) |
| Storage | Encrypted SQLite (SQLCipher) |
| Notifications | Local push via OS scheduler |
| Barcode | MLKit / Flutter Barcode Scanner |
| Export | PDFKit, CSV/JSON serializers |

📁 Data Schema (Simplified)

`json
{
  "medications": [
    {
      "name": "Metformin",
      "dose": "500mg",
      "schedule": "08:00 daily",
      "taken": "08:15",
      "side_effects": [
        {
          "type": "nausea",
          "severity": "mild",
          "duration": "30min"
        }
      ],
      "notes": "Felt dizzy after breakfast"
    }
  ],
  "reviewed_by": "Dr. Smith",
  "exported_on": "2025-08-06"
}
`

---

🩺 Doctor Workflow

1. Patient exports logs before appointment
2. Doctor reviews adherence, side effects, and notes
3. Doctor annotates and confirms accuracy
4. With patient consent, doctor uploads anonymized data to pharma or registry

---

🔄 Feedback Loop (Optional)

- Data shared with pharmaceutical companies is:
  - Anonymized
  - Validated by clinician
  - Exported only with patient consent
- Used to improve formulations, monitor side effects, and enhance treatment protocols

---

🚀 Getting Started

For Patients

1. Download app from clinic or app store
2. Scan medication box or enter manually
3. Log daily intake and side effects
4. Export logs before doctor visit

For Clinicians

1. Review patient logs during appointment
2. Annotate and confirm entries
3. Upload anonymized data if patient consents

---

📜 License & Ethics

This app is designed with patient sovereignty, privacy, and ethical data sharing at its core. All exports are opt-in, and no data leaves the device without explicit consent.
