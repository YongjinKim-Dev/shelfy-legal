# Shelfy — Privacy Policy

**App:** Shelfy
**Developer:** Kim Yongjin (individual developer, South Korea)
**Contact:** anfy5118@gmail.com
**Effective date:** April 18, 2026

---

## Table of Contents

1. Information We Collect
2. Why We Collect It
3. Third-Party Sharing
4. Data Retention
5. Data Security
6. Your Rights
7. Children's Privacy
8. Advertising & App Tracking Transparency
9. Changes to This Policy
10. Contact

---

## 1. Information We Collect

Shelfy does not collect directly identifying information (name, email, phone number). Only the minimum data needed to operate the Service is collected.

### 1-1. Anonymous user ID (Firebase Authentication)

When the app is first launched, Firebase Authentication generates an anonymous UID. The UID does not identify you personally and is used only for:

- Verifying Shelfy Pro subscription status
- Metering AI (Gemini) usage limits
- Recording audit logs inside Cloud Functions

### 1-2. Subscription information (RevenueCat)

When you purchase Shelfy Pro, the RevenueCat SDK collects:

- A RevenueCat-generated anonymous identifier
- Purchase receipt data for validation against App Store / Google Play
- Subscription status and transaction history

RevenueCat does not receive your name, email, or payment card details. The actual payment is processed by Apple or Google.

### 1-3. AI usage metering (Cloud Functions)

When you use AI chat features, Firebase Cloud Functions invoke the Google Gemini API on your behalf. The following metadata is recorded in Firestore:

- Anonymous UID and request timestamps
- Token counts and model selection
- Result status (success / error code)

The prompt body and AI response bodies are not stored on our servers. They are only transmitted while the request is in flight.

### 1-4. Usage analytics (Firebase Analytics)

Firebase Analytics collects anonymous usage patterns:

- Screen views and feature events
- Device type, OS version, app version, language
- Advertising identifiers are used only for advertising personalization within the scope granted by App Tracking Transparency (see section 8). Analytics events themselves are not linked to personal identifiers.

### 1-5. Crash logs (Firebase Crashlytics)

When the app crashes, Firebase Crashlytics may automatically collect:

- Stack traces and error type
- Device model, OS version, app version
- Crash timestamp

Crash logs do not include personally identifiable information or user-generated content from inside the app.

### 1-6. On-device data

The following data is stored only on your device and is never transmitted to the Developer's servers:

- Books you add, reading session history, timer data
- Notes and quotes
- Vibe (mood) tracking records

Because this data never leaves the device, the Developer cannot access it, and it is permanently deleted when you uninstall Shelfy.

---

## 2. Why We Collect It

| Data | Purpose |
|---|---|
| Anonymous UID (Firebase Auth) | Subscription verification, AI quota, audit logs |
| Subscription info (RevenueCat) | Managing and verifying Shelfy Pro |
| AI usage logs (Firestore) | Enforcing per-plan usage limits, preventing abuse |
| Usage analytics (Firebase Analytics) | Understanding which features are useful, planning improvements |
| Crash logs (Crashlytics) | Diagnosing and fixing bugs |
| On-device data | Core reading-tracker functionality |

Analytics and log data are used only to improve Shelfy. Advertising is served by Google Mobile Ads as described in section 8.

---

## 3. Third-Party Sharing

Shelfy does not sell or rent personal information. We share data only with the following service providers as required to operate the app:

- **Google / Firebase** (authentication, analytics, crash reporting, remote config, cloud functions, AI proxy) — https://policies.google.com/privacy
- **RevenueCat** (subscription management and receipt validation) — https://www.revenuecat.com/privacy
- **Apple / Google Play** (payment processing for in-app purchases)
- **Google Mobile Ads (AdMob)** (ad serving) — https://policies.google.com/technologies/ads

Each provider handles data under its own privacy policy; we recommend reviewing those policies for details.

---

## 4. Data Retention

- **Cloud Functions audit logs & AI metering:** retained for up to 13 months, then aggregated or deleted.
- **Firebase Analytics events:** retained according to your Firebase project configuration (default 14 months).
- **Crashlytics data:** retained for 90 days by default.
- **RevenueCat subscription records:** retained for the duration of the subscription plus the period required by tax and audit regulations.
- **On-device data:** kept until you uninstall the app or clear its storage.

When you request deletion (see section 6), personal records tied to the anonymous UID are removed from the Developer's servers unless retention is required by law.

---

## 5. Data Security

- All traffic between the app and Firebase / Cloud Functions is protected by HTTPS (TLS).
- Server-side access follows the least-privilege principle. API secrets are stored in Firebase Secret Manager, not in client code.
- Firestore security rules restrict access to authenticated UIDs. Firebase App Check protects backend endpoints from abuse.

No method of electronic storage or transmission is completely secure. We continuously monitor and improve our security controls.

---

## 6. Your Rights

You have the right to:

- Request access to data we hold that is linked to your anonymous UID.
- Request correction of inaccurate data.
- Request deletion of server-side data tied to your UID.
- Request restriction of processing.

To exercise these rights, email **anfy5118@gmail.com** with the UID shown in the app's settings/about page. We respond within 30 days.

On-device data can be removed at any time by uninstalling Shelfy or clearing the app's storage.

---

## 7. Children's Privacy

Shelfy is not directed to children under the age of 14 (in line with South Korea's Personal Information Protection Act). We do not knowingly collect personal information from children under 14. If you believe a child under 14 has used the app, please contact anfy5118@gmail.com and we will delete any associated data.

---

## 8. Advertising & App Tracking Transparency

Shelfy displays Google Mobile Ads (AdMob) to users on the free plan. Advertising and related tracking work as follows:

- **Ad serving:** Ads are delivered by the Google Mobile Ads SDK. Shelfy Pro subscribers do not see ads.
- **App Tracking Transparency (ATT):** On iOS, the system ATT permission prompt is shown at app launch. If you decline, ads still appear but are non-personalized (contextual only).
- **IDFA / GAID:** iOS IDFA and Android advertising ID are used for ad personalization only when you have granted ATT permission on iOS, or have not opted out of personalized ads on Android.
- **Third-party data handling:** Google Mobile Ads processes data under the [Google Privacy Policy](https://policies.google.com/privacy) and [Google Ads Policies](https://policies.google.com/technologies/ads).

Shelfy does not use Firebase Analytics for ad targeting.

---

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. The effective date at the top of this document will always reflect the latest version. Material changes will also be announced inside the app.

---

## 10. Contact

For privacy questions or requests:

- **Email:** anfy5118@gmail.com
- **Developer:** Kim Yongjin
- **Postal address:** 30-6 Bakdong-gil, Osan-si, Gyeonggi-do, Republic of Korea

Last updated: April 18, 2026.
