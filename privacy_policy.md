# Privacy Policy — YaadHai

**Effective Date:** September 16, 2026  
**Last Updated:** September 16, 2026  
**App Name:** YaadHai  
**Package Name:** com.yaadhai  
**Developer / Data Controller:** YaadHai Team  
**Contact:** [ayushishikshaofficial@gmail.com]

---

## 1. Introduction

Welcome to **YaadHai** ("the App", "we", "our", or "us"). YaadHai is an AI-powered learning, memory, and mastery application that helps students scan study material, generate AI study packs, create flashcards, take quizzes, and manage spaced-repetition revision schedules.

We are committed to protecting your privacy. This Privacy Policy explains what information we collect, how we use it, who we share it with, and your rights regarding your data.

By using YaadHai, you agree to the terms outlined in this Privacy Policy.

---

## 2. Information We Collect

### 2.1 Information You Provide Directly

| Data | Purpose |
|---|---|
| **Google Account (Name, Email, Profile Photo)** | Sign-in via Google Sign-In and Supabase Auth |
| **Study Content (text, photos/images of study material)** | Processing via AI to generate summaries, flashcards, quizzes, and concepts |
| **Subject, Chapter, Concept, Flashcard and Quiz Data** | Stored locally on your device for your learning experience |

### 2.2 Information Collected Automatically

| Data | Purpose |
|---|---|
| **Device identifiers (anonymous)** | App stability and crash diagnostics |
| **App usage data** (features used, session duration) | Improving app performance and user experience |
| **Mastery and revision progress** | Spaced-repetition scheduling and mastery tracking |

### 2.3 Camera and Photo Library Access

The App requests access to your **camera** and **photo library** solely to allow you to scan physical study material (notes, textbooks, handouts). Images are processed using **Google ML Kit** for on-device OCR (text recognition) and optionally sent to our secure Supabase Edge Functions for AI analysis via Google Gemini.

> **We do NOT store your photos on our servers permanently.** Images sent to our Edge Functions are processed in real-time and discarded immediately after the AI response is generated.

---

## 3. How We Use Your Information

We use the information we collect to:

- **Authenticate you** securely via Google Sign-In and Supabase Auth
- **Generate AI Study Packs** (summaries, key concepts, flashcards, quizzes) from your scanned material using Google Gemini AI
- **Store your learning data** locally on your device (Drift / SQLite — fully offline-first)
- **Schedule and track revisions** using the spaced-repetition engine
- **Display insights** such as mastery charts and retention curves
- **Export PDFs** of your study packs
- **Improve the App** through anonymous usage analytics
- **Provide support** when you contact us

---

## 4. Data Storage and Security

### 4.1 Local Storage (On-Device)

The majority of your data — subjects, chapters, concepts, flashcards, quizzes, revision schedules, and mastery progress — is stored **entirely on your device** using Drift (SQLite). This data does **not** leave your device under normal operation.

### 4.2 Cloud Services (Supabase)

We use **Supabase** for:
- **Authentication** — Your Google account credentials are managed by Supabase Auth. We store your user ID, email, display name, and avatar URL securely on Supabase servers.
- **AI Processing (Edge Functions)** — When you scan material, your text or image data is sent to Supabase Edge Functions (hosted in the region you connect to). These functions call **Google Gemini** on your behalf. **Your Gemini API key is stored as a server-side secret and is never exposed to the App.**

### 4.3 Security Measures

- All data transmission uses **HTTPS / TLS encryption**
- Supabase uses **Row Level Security (RLS)** — your data is only accessible by you
- The Supabase `anon` key included in the App is public by design and is protected by RLS policies
- We do not store raw images on our servers

---

## 5. Third-Party Services

YaadHai integrates the following third-party services. Please review their respective privacy policies:

| Service | Purpose | Privacy Policy |
|---|---|---|
| **Supabase** | Authentication & Edge Functions | [supabase.com/privacy](https://supabase.com/privacy) |
| **Google Sign-In** | User Authentication | [policies.google.com/privacy](https://policies.google.com/privacy) |
| **Google Gemini (via Edge Functions)** | AI Study Pack Generation | [ai.google.dev/terms](https://ai.google.dev/terms) |
| **Google ML Kit** | On-device OCR (Text Recognition) | [developers.google.com/ml-kit](https://developers.google.com/ml-kit) |

> **Important:** The Gemini API is called **server-side only** via Supabase Edge Functions. Your Gemini API key is never bundled in or transmitted by the App.

---

## 6. Data Sharing

We do **not** sell, rent, or trade your personal information to third parties.

We may share data only in the following circumstances:

- **Service Providers:** With Supabase and Google (as listed above) to operate core functionality
- **Legal Obligations:** If required by law, regulation, or valid legal process
- **Business Transfer:** In the event of a merger or acquisition, your data may be transferred (you will be notified)
- **With Your Consent:** For any other purpose not listed here, only with your explicit consent

---

## 7. Children's Privacy

YaadHai is intended for users aged **13 and above** (or the applicable minimum digital age in your country). We do not knowingly collect personal data from children under 13. If you believe a child under 13 has provided us with personal data, please contact us immediately and we will delete that data.

---

## 8. Your Rights and Choices

Depending on your location, you may have the following rights:

### 8.1 Access & Portability
You can export your study packs as PDFs directly from the App at any time.

### 8.2 Deletion
You can delete individual subjects, chapters, flashcards, and quizzes from within the App. To delete your entire account and all associated cloud data (Supabase auth records), contact us at [your-support-email@yaadhai.com].

### 8.3 Opt-Out of Analytics
Where applicable, you may opt out of anonymous analytics via your device's privacy settings or by contacting us.

### 8.4 Withdrawal of Consent
You may revoke camera/gallery permissions at any time through your device's **Settings → Apps → YaadHai → Permissions**.

### 8.5 GDPR / CCPA Rights
If you are in the EU or California, you additionally have the right to:
- Request a copy of your personal data
- Request correction of inaccurate data
- Object to or restrict certain processing
- Lodge a complaint with a supervisory authority

To exercise any of these rights, contact us at [your-support-email@yaadhai.com].

---

## 9. Data Retention

| Data Type | Retention Period |
|---|---|
| Local learning data (flashcards, concepts, etc.) | Until you delete it from the App or uninstall |
| Supabase auth records (email, user ID) | Until you request account deletion |
| Images sent for AI processing | Deleted immediately after processing (not persisted on server) |
| Anonymous analytics | Aggregated; retained for up to 12 months |

---

## 10. Permissions Used

| Permission | Why We Need It |
|---|---|
| `CAMERA` | Scan physical study material with your camera |
| `READ_EXTERNAL_STORAGE` / `READ_MEDIA_IMAGES` | Select images from your gallery to scan |
| `INTERNET` | Authenticate with Supabase; send content to AI Edge Functions |
| `WRITE_EXTERNAL_STORAGE` (Android < 10) | Save exported PDF study packs to your device |

---

## 11. Cookies and Tracking

YaadHai is a **mobile application** and does not use browser cookies. Supabase Auth uses secure, server-managed session tokens to keep you signed in.

---

## 12. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. When we make significant changes, we will:

1. Update the **"Last Updated"** date at the top of this document
2. Notify you via an in-app notification or email (where applicable)

Your continued use of the App after changes are posted constitutes acceptance of the updated policy.

---

## 13. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy, please contact us:

**YaadHai Support**  
📧 Email: [ayushishikshaofficial@gmail.com]  
🌐 Website: [www.youtube.com@Ayushi-shiksha]  
 
