# Shelfy — Privacy Policy

**App:** Shelfy
**Developer:** Kim Yongjin (individual developer, South Korea)
**Contact:** yongjin.dev@gmail.com
**Effective date:** April 18, 2026

---

## Table of Contents

1. Information We Collect
2. Why We Collect It
3. Information We Do Not Collect
4. Service Providers & Third-Party Sharing
5. Data Retention
6. Data Security
7. Your Rights (incl. California residents)
8. Children's Privacy
9. Advertising & App Tracking Transparency
10. Changes to This Policy
11. Contact

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

### 1-3. AI usage metering and Google Gemini (Cloud Functions)

When you use AI chat features, Firebase Cloud Functions invoke the Google Gemini API on your behalf. The following metadata is recorded in Firestore:

- Anonymous UID and request timestamps
- Token counts and model selection
- Result status (success / error code)

**Shelfy does not store prompt bodies or AI response bodies on our servers.** They are transmitted to Google only while the request is in flight.

**Google's handling of AI content:** Prompts and responses are sent to Google's Gemini API for processing. Google may log requests for short-term caching, quality and safety monitoring. According to Google's current policy for the paid Gemini API (used by Shelfy), your prompts are not used to train Google's models. See the [Google AI / Gemini API Additional Terms of Service](https://ai.google.dev/gemini-api/terms) for details.

Please avoid sending any personal, sensitive, or confidential information to the AI chat. Treat AI conversations as if they could be reviewed by a third-party provider.

### 1-4. Usage analytics (Firebase Analytics)

Firebase Analytics collects anonymous usage patterns:

- Screen views and feature events
- Device type, OS version, app version, language
- Advertising identifiers are used only for advertising personalization within the scope granted by App Tracking Transparency (see section 8). Analytics events themselves are not linked to personal identifiers.

### 1-5. On-device data

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
| On-device data | Core reading-tracker functionality |

Analytics and log data are used only to improve Shelfy. Advertising is served by Google Mobile Ads as described in section 9.

---

## 3. Information We Do Not Collect

Shelfy does not collect any of the following:

- Real name, email address, phone number, or postal address from inside the app
- Government identifiers (Social Security Number, resident registration number, driver's license, passport)
- Payment card numbers or bank account details (processed entirely by Apple or Google)
- Biometric data (fingerprint, face scan, voiceprint)
- Precise location (GPS coordinates)
- Health, medical, financial, religious, political, or sexual orientation information
- Microphone or camera input
- Contacts, calendar, or photo library

We do not sell your personal information and we do not share it with third parties for their own marketing.

---

## 4. Service Providers & Third-Party Sharing

Shelfy relies on a small number of service providers ("processors") to operate. Each provider is contractually bound to process data only for the purposes we specify:

- **Google / Firebase** — authentication, analytics, remote config, cloud functions, AI (Gemini) proxy. Privacy policy: https://policies.google.com/privacy
- **RevenueCat** — subscription management and receipt validation. Privacy policy: https://www.revenuecat.com/privacy
- **Apple / Google Play** — payment processing for in-app purchases.
- **Google Mobile Ads (AdMob)** — ad serving. Privacy policy: https://policies.google.com/technologies/ads

We do not sell or rent your personal information to any third party.

---

## 5. Data Retention

- **Cloud Functions audit logs & AI metering:** retained for up to 13 months, then aggregated or deleted.
- **Firebase Analytics events:** retained according to your Firebase project configuration (default 14 months).
- **RevenueCat subscription records:** retained for the duration of the subscription plus the period required by tax and audit regulations.
- **On-device data:** kept until you uninstall the app or clear its storage.

When you request deletion (see section 6), personal records tied to the anonymous UID are removed from the Developer's servers unless retention is required by law.

---

## 6. Data Security

- All traffic between the app and Firebase / Cloud Functions is protected by HTTPS (TLS).
- Server-side access follows the least-privilege principle. API secrets are stored in Firebase Secret Manager, not in client code.
- Firestore security rules restrict access to authenticated UIDs. Firebase App Check protects backend endpoints from abuse.

No method of electronic storage or transmission is completely secure. We continuously monitor and improve our security controls.

---

## 7. Your Rights

You have the right to:

- Request access to data we hold that is linked to your anonymous UID.
- Request correction of inaccurate data.
- Request deletion of server-side data tied to your UID.
- Request restriction of processing.
- Object to processing.
- Receive your data in a portable format.

To exercise these rights, email **yongjin.dev@gmail.com** with the UID shown in the app's settings/about page. We respond within 30 days.

On-device data can be removed at any time by uninstalling Shelfy or clearing the app's storage.

### 7-1. California residents (CCPA / CPRA)

California residents have additional rights under the California Consumer Privacy Act (CCPA) as amended by the California Privacy Rights Act (CPRA):

- **Right to know** what personal information we collect and how it is used.
- **Right to delete** personal information we hold about you.
- **Right to correct** inaccurate personal information.
- **Right to opt out of sale or sharing** of personal information.
- **Right to limit use of sensitive personal information.**
- **Right to non-discrimination** for exercising any of these rights.

**Shelfy does not sell or share personal information** for cross-context behavioral advertising, and we do not collect sensitive personal information as defined by CCPA. To exercise your rights, email **yongjin.dev@gmail.com**.

### 7-2. EEA / UK residents (GDPR)

If you are in the European Economic Area or the United Kingdom, you can also lodge a complaint with your local data protection authority. Our lawful basis for processing is (a) performance of the Service contract under these Terms, and (b) our legitimate interest in maintaining a functional, abuse-resistant product.

---

## 8. Children's Privacy

Shelfy is not directed to children. We do not knowingly collect personal information from children under 13 (United States — COPPA) or under 16 (European Economic Area and United Kingdom — GDPR minimum). If you believe a child below these ages has used the app, please contact yongjin.dev@gmail.com and we will delete any associated data.

---

## 9. Advertising & App Tracking Transparency

Shelfy displays Google Mobile Ads (AdMob) to users on the free plan. Advertising and related tracking work as follows:

- **Ad serving:** Ads are delivered by the Google Mobile Ads SDK. Shelfy Pro subscribers do not see ads.
- **App Tracking Transparency (ATT):** On iOS, the system ATT permission prompt is shown at app launch. If you decline, ads still appear but are non-personalized (contextual only).
- **IDFA / GAID:** iOS IDFA and Android advertising ID are used for ad personalization only when you have granted ATT permission on iOS, or have not opted out of personalized ads on Android.
- **Third-party data handling:** Google Mobile Ads processes data under the [Google Privacy Policy](https://policies.google.com/privacy) and [Google Ads Policies](https://policies.google.com/technologies/ads).

Shelfy does not use Firebase Analytics for ad targeting.

---

## 10. Changes to This Policy

We may update this Privacy Policy from time to time. The effective date at the top of this document will always reflect the latest version. Material changes will also be announced inside the app.

---

## 11. Contact

For privacy questions or requests:

- **Email:** yongjin.dev@gmail.com
- **Developer:** Kim Yongjin

Last updated: April 18, 2026.
