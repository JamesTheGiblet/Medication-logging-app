## **Project: MedLog - A Private Medication Tracker**

### **The Problem**

Most health apps are garbage. They're confusing, they require an internet connection, and—worst of all—they sell your personal health data to the highest bidder. That’s not just bad design; it's a violation of trust.

### **The Solution**

MedLog. A simple, offline-first app that helps you track your medications and side effects. **Your data stays on your phone. Period.** It doesn't go to the cloud, and it's not for sale. It's a tool, not a data-mining operation.

### **How It Works**

* **Log Your Meds & Side Effects:** Quickly add your medications, dosages, and schedules. Record any side effects with details like severity and timing.
* **Scan Your Medication Box:** Use the phone's camera to scan the barcode on a medicine box. The app pulls the name and dose from a built-in, offline database.
* **Get Simple Reminders:** The app sends you a local notification when it's time to take a dose. No internet required.
* **Export for Your Doctor:** Generate a simple PDF or data file of your logs to share with your doctor. You are in control of when this happens.
* **Your Data is Yours. Period:** The app stores everything locally on your phone in an encrypted file. There is no cloud sync. We can't see your data, and we don't want to.

### **Who It's For**

The app has a few simple roles, with clear rules.

| Role               | What They Can Do                                             |
| ------------------ | ------------------------------------------------------------ |
| **Patient** | The main user. Logs meds, gets reminders, exports data.       |
| **Caregiver** | Can be given access by the patient to help log entries.        |
| **Doctor** | Can review the exported logs from the patient.               |
| **Researcher** | Can **only** get data if the patient and doctor **both** approve it. |

### **Built for Everyone**

A tool is useless if people can't use it. This app is designed to be accessible.
* Large text and high-contrast modes.
* Voice input for logging.
* Simple tap-based logging for users with limited dexterity.
* Full screen reader support (TalkBack/VoiceOver).

### **The Tech Stack (How It's Built)**

No black boxes. Here’s the tech.

| Layer         | Technology                  | Why?                                      |
| ------------- | --------------------------- | ----------------------------------------- |
| **App** | Flutter (Android/iOS)       | Build for both platforms from one codebase. |
| **Storage** | Encrypted SQLite (SQLCipher)| Strong, local, offline-first encryption.  |
| **Barcode** | MLKit / On-device library   | Scans barcodes without needing the internet.  |
| **Export** | PDF/CSV/JSON serializers    | Standard formats doctors can actually use.  |

### **The Data Sharing Rule (This is Important)**

Data can **only** be shared with researchers (like pharmaceutical companies) if **all three** of these conditions are met:
1.  **You (the patient) explicitly consent** to sharing for a specific purpose.
2.  **Your doctor reviews and approves** the export.
3.  **All data is made 100% anonymous**, stripping out any personal information.

If any of these are not met, nothing is shared. There are no exceptions.

### **How to Use It**

**For Patients:**
1.  Download the app.
2.  Scan your medication box or add it manually.
3.  Log your doses and any side effects each day.
4.  Before your doctor's visit, use the "Export" button to create a log file.

**For Doctors:**
1.  Receive the log file from your patient.
2.  Review it with them to track adherence and side effects.
3.  If the patient agrees to share their data for research, you act as the final check to approve the anonymized export.

No subscriptions, no ads, no selling your data. Just a tool that works. **Build first, ask permission never**—especially when it comes to your own health data.
