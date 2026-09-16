# Privacy Policy — YaadHai

**Effective Date:** September 16, 2026  
**Last Updated:** September 16, 2026  
**App Name:** YaadHai  
**Package Name:** com.yaadhai  
**Developer / Data Controller:** YaadHai Team  
**Contact:** ayushishikshaofficial@gmail.com

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
- **AI Processing (Edge Functions)** — When you scan material, your text or image data is sent to Supabase Edge Functions. These functions call **Google Gemini** on your behalf. Your Gemini API key is stored as a server-side secret and is never exposed to the App.

### 4.3 Security Measures

- All data transmission uses **HTTPS / TLS encryption**
- Supabase uses **Row Level Security (RLS)** — your data is only accessible by you
- We do not store raw images on our servers

---

## 5. Third-Party Services

YaadHai integrates the following third-party services:

| Service | Purpose | Privacy Policy |
|---|---|---|
| **Supabase** | Authentication & Edge Functions | [supabase.com/privacy](https://supabase.com/privacy) |
| **Google Sign-In** | User Authentication | [policies.google.com/privacy](https://policies.google.com/privacy) |
| **Google Gemini (via Edge Functions)** | AI Study Pack Generation | [ai.google.dev/terms](https://ai.google.dev/terms) |
| **Google ML Kit** | On-device OCR (Text Recognition) | [developers.google.com/ml-kit](https://developers.google.com/ml-kit) |

---

## 6. Data Sharing

We do **not** sell, rent, or trade your personal information to third parties.

---

## 7. Children's Privacy

YaadHai is intended for users aged **13 and above**. We do not knowingly collect personal data from children under 13.

---

## 8. Account & Data Deletion (Google Play Compliance)

Users have the right to request deletion of their account and associated authentication data at any time:

### How to Request Account Deletion:
1. Send an email to **ayushishikshaofficial@gmail.com** with the subject: `Account Deletion Request - YaadHai`.
2. Please send the request from the same Google email address used to sign in to the app.

### Data Deleted:
- **Authentication Records:** Your user profile, email address, and authentication record in Supabase Auth will be permanently deleted within **7 business days**.
- **On-Device Data:** All study notes, flashcards, and quizzes are stored locally on your device and will be deleted immediately upon clearing app data or uninstalling the app.

---

## 9. Data Retention

| Data Type | Retention Period |
|---|---|
| Local learning data (flashcards, concepts, etc.) | Until you delete it from the App or uninstall |
| Supabase auth records (email, user ID) | Until you request account deletion |
| Images sent for AI processing | Deleted immediately after processing |
| Anonymous analytics | Retained for up to 12 months |

---

## 10. Permissions Used

| Permission | Why We Need It |
|---|---|
| `CAMERA` | Scan physical study material with your camera |
| `READ_EXTERNAL_STORAGE` / `READ_MEDIA_IMAGES` | Select images from your gallery to scan |
| `INTERNET` | Authenticate with Supabase; send content to AI Edge Functions |

---

## 11. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy:

**YaadHai Support**  
📧 Email: **ayushishikshaofficial@gmail.com**  
🌐 Channel: **https://www.youtube.com/@Ayushi-shiksha**  
