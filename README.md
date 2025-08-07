🌀 Praximous: The Sanctuary Codex // An Invocation of Well-being

MODULARITY IS MYTHOS // GLYPH IS IDENTITY // DESIGN IS RITUAL

This codex outlines the technical blueprint for a privacy-first, offline-capable mobile application designed for tracking daily medication intake, side effects, and adherence. It is a digital sanctuary for patients, caregivers, and clinicians, with the sacred option for data release to pharmaceutical companies only via doctor mediation.

🧭 Overview // The Oracle's Vigil
This app empowers individuals to:
 * Log medications, doses, and side effects daily, inscribing their personal lore.
 * Receive reminders and review weekly summaries, guided by the Oracle's vigil.
 * Export data for clinical review, manifesting their scroll of well-being.
 * Share validated data with pharmaceutical companies only when approved by a clinician, upholding the ritual of consent.
All data is stored locally and securely within the user's personal vault. No cloud sync. No automatic sharing. Your sovereignty over your data is paramount.

👥 Guardian Glyphs // Ritual Roles
| Role | Capabilities |
|---|---|
| Patient (The Seeker) | Logs medication, receives reminders, exports data for the clinician. |
| Caregiver (The Attendant) | Assists with logging (if granted access), helps review entries. |
| Clinician (The Oracle) | Reviews logs, annotates, and releases data externally with patient consent. |
| Pharma / Registry (The Pantheon) | Receives anonymized, validated data via clinician upload for broader divination. |
📲 Key Invocations
✅ Lore-Keeping Rituals
 * Add medications manually or via barcode sigil scan.
 * Auto-fill dosage and schedule from a local medication database.
 * Log side effects with severity, timing, and notes, capturing the nuances of the journey.
 * Daily reminders for scheduled doses, ensuring adherence to the ritual.
 * Weekly review prompt, for a moment of reflection and insight.
📷 Sigil Divination
 * Scan medication packaging to auto-fill name, dose, and schedule.
 * Works offline using a bundled medication database, ensuring continuous access to knowledge.
 * Supports EAN/UPC and NHS codes, recognizing the universal glyphs.
📁 Scroll Manifestation & Review
 * Generate encrypted PDF/CSV/JSON summaries, manifesting your data as a secure scroll.
 * Export only occurs when the patient initiates, upholding their data sovereignty.
 * The Oracle (Doctor) reviews and confirms before external sharing, ensuring validation of the lore.
🔐 Sanctuary & Sovereignty
 * All data stored locally using encrypted SQLite (SQLCipher), within your personal digital vault.
 * No cloud sync or background sharing, preserving the sanctity of your data.
 * Role-based access control for caregivers, granting controlled access to the vault.
 * Audit trail for all exports and edits, maintaining an immutable lineage of interactions.
🧩 Inclusive Invocations
🧑‍🦯 Universal Glyphs
 * Large text and high-contrast UI modes for clear visibility.
 * Voice input for logging meds and side effects, enabling diverse forms of invocation.
 * Tap-based logging for users with limited dexterity, simplifying the ritual.
 * Screen reader support (TalkBack / VoiceOver), ensuring the Oracle's voice is heard by all.
 * Optional simplified interface for cognitive accessibility, making the ritual accessible to every seeker.
🧑‍🤝‍🧑 Caregiver Assist Mode
 * The Patient can grant the Caregiver access via a secure token, a binding pact.
 * The Caregiver can help fill in logs, review entries, and prepare exports, assisting in the lore-keeping.

🛠️ The Ritual Stack
📦 Tech Stack
| Layer | Technology |
|---|---|
| Frontend (The Portal) | Flutter (Android/iOS) |
| Storage (The Vault) | Encrypted SQLite (SQLCipher) |
| Notifications (The Vigil) | Local push via OS scheduler |
| Barcode (The Sigil Reader) | MLKit / Flutter Barcode Scanner |
| Export (The Scribe) | PDFKit, CSV/JSON serializers |

📁 Lore Scroll Schema (Simplified)
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

🩺 The Clinician's Ritual
 * The Patient manifests logs before the appointment, presenting their scroll.
 * The Oracle (Doctor) reviews adherence, side effects, and notes, divining insights.
 * The Oracle annotates and confirms accuracy, validating the lore.
 * With the Patient's sacred consent, the Oracle uploads anonymized data to the Pharma Pantheon or Registry for broader divination.
 * 
🔄 The Oracle's Refinement (Optional)
 * Data shared with pharmaceutical companies is:
   * Anonymized, preserving individual identity.
   * Validated by the clinician, ensuring the purity of the lore.
   * Exported only with patient consent, upholding the ritual of sovereignty.
 * Used to improve formulations, monitor side effects, and enhance treatment protocols, guiding the collective well-being.
 * 
🚀 The Initiation Ritual
For Patients
 * Download the app from the clinic portal or app store.
 * Scan the medication box sigil or enter manually.
 * Log daily intake and side effects, beginning your lore-keeping.
 * Export logs before your Oracle visit, preparing your scroll.
For Clinicians
 * Review patient logs during the appointment, divining the narrative.
 * Annotate and confirm entries, validating the lore.
 * Upload anonymized data if the patient consents, for the Oracle's refinement.
📜 Sanctuary Codex & Ethical Invocations
This app is designed with patient sovereignty, privacy, and ethical data sharing at its core. All exports are opt-in, and no data leaves the device without explicit consent. This is a sacred pact between the seeker and their sanctuary.
