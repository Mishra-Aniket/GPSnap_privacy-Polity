# GPSnap — Legal, Privacy & Compliance Portal

[![Status](https://img.shields.io/badge/Status-Active-success.svg)](#)
[![Google Play Policy](https://img.shields.io/badge/Google_Play_Policy-Compliant_2026-blue.svg)](#)
[![GDPR Compliant](https://img.shields.io/badge/GDPR-Compliant-008080.svg)](#)
[![CCPA Ready](https://img.shields.io/badge/CCPA-Ready-orange.svg)](#)
[![License](https://img.shields.io/badge/License-Proprietary-lightgrey.svg)](#)

Official Privacy Policy, Terms & Conditions, and Google Play Data Safety documentation for **GPSnap: GPS Map Camera & Geotag Timestamp** (`com.gpsnap.app`), developed by **Aniket Mishra**.

- **Application Name:** GPSnap: GPS Map Camera
- **Package Name:** `com.gpsnap.app`
- **Developer:** Aniket Mishra
- **Official Contact Email:** [contact@aniket.one](mailto:contact@aniket.one)
- **Effective Date:** November 13, 2026
- **Last Updated:** November 13, 2026
- **Hosted Portal:** [https://mishra-aniket.github.io/GPSnap_privacy-Polity/](https://mishra-aniket.github.io/GPSnap_privacy-Polity/)

---

## Table of Contents

1. [Privacy Policy Summary](#privacy-policy-summary)
2. [Full Privacy Policy](#full-privacy-policy)
   - [1. Introduction & Zero-Cloud Architecture](#1-introduction--zero-cloud-architecture)
   - [2. Sensitive Permissions & Clear Purpose Specification](#2-sensitive-permissions--clear-purpose-specification)
   - [3. Foreground Location Usage & Transparency](#3-foreground-location-usage--transparency)
   - [4. Third-Party SDKs & Services](#4-third-party-sdks--services)
   - [5. Advertising & Device Identifier Controls](#5-advertising--device-identifier-controls)
   - [6. Data Storage, Security & Retention](#6-data-storage-security--retention)
   - [7. How to Delete Your Data](#7-how-to-delete-your-data)
   - [8. Regional Privacy Rights (GDPR, CCPA/CPRA, DPDP)](#8-regional-privacy-rights-gdpr-ccpacpra-dpdp)
   - [9. Children’s Privacy (COPPA & Google Play Families Policy)](#9-childrens-privacy-coppa--google-play-families-policy)
   - [10. Policy Changes & Updates](#10-policy-changes--updates)
   - [11. Contact & Data Protection Inquiries](#11-contact--data-protection-inquiries)
3. [Terms & Conditions (Terms of Service)](#terms--conditions)
4. [Google Play Data Safety Reference Matrix](#google-play-data-safety-reference-matrix)
5. [User Guide: Managing Permissions & Deleting Data](#user-guide-managing-permissions--deleting-data)

---

## Privacy Policy Summary

| Category | Policy Commitment |
| :--- | :--- |
| **Photos & Videos** | Processed and stored **100% locally on your device**. GPSnap does not upload your captures to any developer server. |
| **Location Data** | Accessed **only in the foreground** while using the camera or viewing maps to embed coordinates, address, and weather overlays. No background tracking. |
| **Microphone** | Used **only when recording video** with sound enabled. Never active in the background. |
| **Text Recognition (OCR)** | Powered by **on-device Google ML Kit**. No images or recognized text leave your hardware. |
| **Third-Party Ads** | Powered by **Google AdMob**. Ad personalization can be reviewed and adjusted via Android Settings or in-app consent dialogs. |
| **Data Selling** | We **never** sell, rent, or trade your personal information or media to any third party. |

---

# Full Privacy Policy

**Effective Date:** November 13, 2026  
**Applicable Application:** GPSnap (`com.gpsnap.app`)  
**Developer:** Aniket Mishra ([contact@aniket.one](mailto:contact@aniket.one))

### 1. Introduction & Zero-Cloud Architecture

Thank you for choosing **GPSnap: GPS Map Camera & Geotag Timestamp** (hereinafter referred to as "GPSnap", "the App", "we", "our", or "us"). We recognize that your photos, videos, and geographical whereabouts are sensitive and personal. This Privacy Policy details our unwavering commitment to protecting your privacy, describing precisely what data is accessed, how it is processed, and your rights concerning your personal information.

**Core Architecture Principle:** GPSnap is built with a **local-first, on-device architecture**. We do not operate proprietary cloud servers to catalog, harvest, host, or sell your photos, videos, notes, or GPS trajectories. All image capture, geotag metadata burning, compass calculations, video rendering, and PDF report generations take place locally on your device hardware.

---

### 2. Sensitive Permissions & Clear Purpose Specification

To deliver professional GPS camera and field inspection capabilities, GPSnap requests specific Android system runtime permissions. Below is an exhaustive breakdown of each permission and its precise functional purpose:

#### a. Precise & Approximate Location (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`)
- **Purpose:** Used in real time to obtain your device's geographical coordinates (latitude, longitude, altitude, GPS horizontal/vertical accuracy, velocity/speed, and compass heading/azimuth).
- **Functionality Supported:** Stamping real-time coordinates onto your photos and video frames, reverse-geocoding human-readable addresses, fetching current ambient weather and air quality metrics, and rendering interactive mini-map overlays.
- **Scope:** Foreground use only. We **never** track your location in the background or when the app is minimized.

#### b. Camera (`CAMERA`)
- **Purpose:** Grants access to your device camera sensors to display the live viewfinder, capture high-resolution photos, record videos, and calculate optical focus and exposure.
- **Functionality Supported:** Real-time on-screen preview of geotag stamps, photo snapping, video recording, aspect ratio toggling, torch/flash controls, and grid display.
- **Scope:** Camera sensors are only accessed while the viewfinder screen is actively visible.

#### c. Microphone & Audio Recording (`RECORD_AUDIO`)
- **Purpose:** Captures audio tracks during video recording sessions.
- **Scope:** Audio is recorded **only** when the user explicitly triggers video capture. GPSnap never accesses the microphone during photo mode or in the background.

#### d. Photos, Media & Storage (`READ_MEDIA_IMAGES`, `READ_MEDIA_VIDEO`, `READ_MEDIA_VISUAL_USER_SELECTED`, `READ_EXTERNAL_STORAGE`, `WRITE_EXTERNAL_STORAGE`)
- **Purpose:** Reads and writes media files to your device's shared storage utilizing the official Android MediaStore API (Scoped Storage compliant on Android 10, 11, 12, 13, 14, and above).
- **Functionality Supported:** Saving captured geotagged photos, videos, and generated PDF field reports directly to your device storage; displaying your media inside the in-app gallery; and allowing you to pick a custom company or surveyor logo from your gallery to use as a stamp watermark.
- **Scope:** Access is restricted to app-relevant files and user-selected media.

#### e. Device Accounts (`GET_ACCOUNTS`)
- **Purpose:** Used exclusively if you elect to link your Google account for optional Google Drive backup and synchronization of your field captures.
- **Scope:** This is an optional feature. Your Google account details are never transmitted to our servers; communication happens directly between your device and Google's authorized OAuth endpoints.

#### f. Network Access (`INTERNET`, `ACCESS_NETWORK_STATE`)
- **Purpose:** Verifies network availability and provides secure internet connectivity.
- **Functionality Supported:**
  1. Fetching map tiles for the mini-map stamp preview (via Google Maps SDK and OpenStreetMap/OSM).
  2. Converting GPS coordinates into formatted street addresses via reverse geocoding APIs.
  3. Fetching localized ambient weather and Air Quality Index (AQI) values from Open-Meteo API.
  4. Displaying sponsor advertisements via Google AdMob.
  5. Checking for critical application updates via Google Play In-App Updates.

#### g. Vibration (`VIBRATE`)
- **Purpose:** Provides optional tactile haptic feedback when the camera shutter button is pressed or video recording begins.

---

### 3. Foreground Location Usage & Transparency

GPSnap prioritizes battery efficiency and user privacy:
- **No Background Location Tracking:** GPSnap does **not** declare or request the `ACCESS_BACKGROUND_LOCATION` permission.
- **Immediate Cessation:** As soon as you navigate away from the camera screen, minimize the app, or lock your device, GPS hardware listening is terminated immediately.
- **User Control:** You may disable location permissions at any time via Android System Settings. If location permission is denied, GPSnap remains operational as a standard camera app without geotag metadata.

---

### 4. Third-Party SDKs & Services

GPSnap incorporates industry-standard SDKs to provide mapping, weather, ads, and machine learning features. Each provider operates under its respective privacy terms:

| Service / SDK | Provider | Function | Privacy Policy Link |
| :--- | :--- | :--- | :--- |
| **Google Play Services (Location & Maps)** | Google LLC | GPS fusion, map rendering | [Google Privacy Policy](https://policies.google.com/privacy) |
| **Google AdMob** | Google LLC | In-app advertising | [Google Ads Privacy](https://policies.google.com/technologies/ads) |
| **Google ML Kit (Text Recognition)** | Google LLC | On-device OCR for landmark & address detection | [Google ML Kit Terms](https://developers.google.com/ml-kit/terms) |
| **OpenStreetMap & Nominatim** | OSM Foundation | Open-source map tiles & address reverse lookup | [OSMF Privacy Policy](https://wiki.osmfoundation.org/wiki/Privacy_Policy) |
| **Open-Meteo API** | Open-Meteo | Real-time weather and Air Quality Index (AQI) data | [Open-Meteo Privacy](https://open-meteo.com/en/terms) |
| **Google Play In-App Updates** | Google LLC | Seamless app updates via Play Store | [Google Play Terms](https://play.google.com/intl/en_us/about/play-terms/) |

#### Key Safeguards:
- **On-Device ML Kit OCR:** All text recognition for building numbers, street signs, and landmarks is processed **100% on-device**. No camera frames, image pixels, or recognized text strings are sent to Google cloud servers.
- **Weather & Reverse Geocoding:** Coordinate requests sent to Open-Meteo or Nominatim are anonymous HTTP GET requests containing purely numeric latitude/longitude values without user credentials, device IDs, or personal markers.

---

### 5. Advertising & Device Identifier Controls

GPSnap utilizes **Google AdMob** to display banner and app-open advertisements, enabling us to provide regular updates and maintain features free of charge.

- **Data Processed by AdMob:** AdMob may collect your device's Google Advertising ID (AAID), IP address, app interaction logs, and non-sensitive diagnostic information to serve ads and prevent fraudulent clicks.
- **Consent Management (GDPR/UMP):** For users residing in the European Economic Area (EEA), United Kingdom (UK), and Switzerland, GPSnap integrates Google's User Messaging Platform (UMP) to present a compliant consent dialog. You can accept, reject, or customize ad preferences.
- **Opting Out of Personalized Ads:**
  - On your Android device, navigate to **Settings → Google → Ads** (or **Settings → Privacy → Ads**).
  - Tap **Reset advertising ID** or **Delete advertising ID**.
  - Enable **Opt out of Ads Personalization** (on supported Android versions).

---

### 6. Data Storage, Security & Retention

- **Local Storage:** All photos (`.jpg`), videos (`.mp4`), generated PDF reports (`.pdf`), custom logo files, and app settings reside on your device's local storage (typically in `Pictures/GPSnap`, `Movies/GPSnap`, and `Documents/GPSnap`).
- **No Remote Retention:** Because we do not upload your media to developer servers, we retain **zero** copies of your photos, videos, or location data.
- **Security Standards:** Any network requests for maps, weather, geocoding, and ad delivery are performed over encrypted Transport Layer Security (TLS/HTTPS).

---

### 7. How to Delete Your Data

Because your data is stored locally on your device, you possess total control over deletion:

1. **Delete Individual Files:** Open the in-app GPSnap Gallery or your device’s native Gallery/Files app, select unwanted photos, videos, or PDF reports, and tap **Delete**.
2. **Clear Application Cache & Preferences:**
   - Go to **Android Settings → Apps → GPSnap → Storage & cache**.
   - Tap **Clear Cache** and **Clear Storage**. This resets all custom stamp templates, notes, and local configurations.
3. **Full App Uninstallation:** Uninstalling GPSnap permanently removes all sandboxed application files, temporary caches, and local configurations.
4. **Support Inquiries Deletion:** If you have contacted our developer support email (`contact@aniket.one`) and wish to have your support correspondence permanently erased from our mail client, email us with the subject `Data Deletion Request`. We process and confirm all deletion requests within 30 days free of charge.

---

### 8. Regional Privacy Rights

#### a. European Economic Area (EEA) & UK (GDPR Compliance)
Under Regulation (EU) 2016/679 (GDPR) and the UK Data Protection Act:
- **Legal Bases:**
  - *Contractual Necessity:* To provide core camera, geotagging, and report generation features requested by you.
  - *Consent:* For personalized ad serving via Google AdMob and optional Google Drive account linking.
  - *Legitimate Interests:* To diagnose crashes, fix bugs, and prevent fraudulent activity.
- **Your Rights:** Right of Access, Rectification, Erasure ("Right to be Forgotten"), Restriction of Processing, Data Portability, and Objection.
- You have the right to lodge a complaint with your national Data Protection Authority (DPA).

#### b. California Residents (CCPA / CPRA Compliance)
Under the California Consumer Privacy Act (CCPA) and California Privacy Rights Act (CPRA):
- **No Sale of Personal Information:** We **do not sell** your personal information or media to third parties for monetary consideration.
- **Categories Collected:** Geolocation data (processed on-device for stamp rendering), Identifiers (Google Advertising ID collected by Google AdMob).
- **Your Rights:** Right to know, right to delete, right to opt-out of sharing for cross-context behavioral advertising, and right to non-discrimination.

#### c. India (Digital Personal Data Protection Act - DPDP 2023)
- Processing is conducted transparently for specified lawful purposes with user consent.
- For grievances or inquiries, contact our designated Grievance Officer at [contact@aniket.one](mailto:contact@aniket.one).

---

### 9. Children’s Privacy (COPPA & Google Play Families Policy)

GPSnap is designed as a productivity and field photography utility for general audiences. It is **not directed at children under the age of 13** (or under 16 in the European Union). We do not knowingly solicit or collect personal identifiable information from children. If you believe that a child has provided us with personal information, please notify us immediately at [contact@aniket.one](mailto:contact@aniket.one), and we will take expeditious action to delete the information.

---

### 10. Policy Changes & Updates

We may update this Privacy Policy from time to time to reflect modifications in our features, technological updates, or regulatory requirements. Any revisions will be published on this repository and within the application, accompanied by an updated **Effective Date**. Continued use of GPSnap following any posted update constitutes your acknowledgment and acceptance of the revised terms.

---

### 11. Contact & Data Protection Inquiries

If you have questions, feedback, or requests regarding this Privacy Policy or our privacy practices, please contact us:

- **Developer:** Aniket Mishra
- **Application:** GPSnap (`com.gpsnap.app`)
- **Direct Support & Privacy Email:** [contact@aniket.one](mailto:contact@aniket.one)
- **Response Commitment:** Inquiries are acknowledged within 48 to 72 business hours.

---

# Terms & Conditions

**Effective Date:** November 13, 2026  
**Application:** GPSnap (`com.gpsnap.app`)

### 1. Agreement to Terms
By downloading, installing, accessing, or using **GPSnap**, you agree to be bound by these Terms & Conditions ("Terms") and our [Privacy Policy](#full-privacy-policy). If you do not agree to all terms and conditions herein, you must immediately discontinue use and uninstall the application.

### 2. License Grant & Permitted Use
We grant you a personal, worldwide, non-exclusive, non-transferable, revocable license to download and run GPSnap on compatible Android devices. 
- **Permitted Uses:** You may use GPSnap for personal documentation, travel photography, professional field work, engineering inspections, real estate documentation, delivery verification, agricultural surveys, and lawful commercial field recording.
- **Restrictions:** You shall not:
  - Decompile, disassemble, reverse engineer, or attempt to extract source code from GPSnap.
  - Modify, distribute, sell, lease, sublicense, or create derivative works based on the App or its proprietary stamp designs.
  - Circumvent, tamper with, or bypass any security features, ad displays, or update verifications.
  - Use the App for clandestine surveillance, harassment, stalking, trespassing, or any activity that violates the privacy or legal rights of others.

### 3. Disclaimers: Accuracy of GPS, Altitude & Environmental Data
- **Informational & Documentation Purpose Only:** Geolocation coordinates, altitude, compass orientation, street addresses, weather, and air quality metrics stamped onto photos and videos are provided for convenience, reference, and field documentation purposes.
- **Hardware & Environmental Dependence:** Accuracy relies upon your device’s internal sensors (GPS chip, accelerometer, compass magnetometer, barometer), satellite constellation availability, atmospheric interference, and third-party APIs.
- **Critical Operations Disclaimer:** **GPSnap is NOT certified for life-critical navigation, emergency search-and-rescue, aviation flight control, marine navigation in hazardous waters, or certified legal cadastral land boundary surveys.** Do not rely solely on GPSnap where sensor inaccuracy could result in personal injury, death, or severe property/financial damage.

### 4. User-Generated Content & Ownership
- **Your Content Belongs to You:** You retain 100% intellectual property ownership of all photos, videos, notes, audio recordings, and PDF inspection reports created using GPSnap.
- **User Responsibility:** You are solely responsible for ensuring that your photos and recordings comply with local laws, property boundaries, photography permissions, and individuals' privacy rights.

### 5. Intellectual Property Rights
All title, ownership, trademarks, service marks, application code, visual interfaces, stamp layout designs, graphics, and branding associated with **GPSnap** remain the exclusive intellectual property of **Aniket Mishra**. All rights not expressly granted to you are reserved.

### 6. Third-Party Services & Links
GPSnap integrates third-party services, including Google Maps, OpenStreetMap, Open-Meteo, and Google AdMob. We have no control over and assume no liability for the availability, operational accuracy, or policies of third-party platforms.

### 7. Disclaimer of Warranties
**GPSnap is provided on an "AS IS" and "AS AVAILABLE" basis without warranties of any kind, whether express, implied, or statutory, including but not limited to the implied warranties of merchantability, fitness for a particular purpose, non-infringement, and uninterrupted or error-free operation.**

### 8. Limitation of Liability
To the maximum extent permitted by applicable law, in no event shall Aniket Mishra or any contributors be liable for any indirect, incidental, special, consequential, or punitive damages, including loss of profits, loss of data, business interruption, or device failure arising out of or related to your use of or inability to use GPSnap, even if advised of the possibility of such damages.

### 9. Termination
These Terms remain effective until terminated by either you or us. You may terminate these Terms by uninstalling GPSnap. We reserve the right to suspend or terminate your access to the App at our discretion if you violate these Terms.

### 10. Governing Law
These Terms shall be governed by and construed in accordance with the laws of India, without regard to conflict of law principles. Any legal disputes arising under these Terms shall be subject to the exclusive jurisdiction of the competent courts in India.

### 11. Contact Information
For inquiries regarding these Terms & Conditions:
- **Developer:** Aniket Mishra
- **Email:** [contact@aniket.one](mailto:contact@aniket.one)

---

# Google Play Data Safety Reference Matrix

This reference table outlines the exact responses for the **Google Play Console Data Safety questionnaire**:

| Data Type | Collected? | Shared? | Purpose | Ephemeral? | User Can Request Deletion? |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Approximate Location** | Yes | No | App functionality (stamp overlays, weather) | Yes | Yes (revoke permission or clear data) |
| **Precise Location** | Yes | No | App functionality (coordinates, compass, maps) | Yes | Yes (revoke permission or clear data) |
| **Photos & Videos** | **No** (Processed locally) | **No** | Local storage of stamped photos and videos | N/A | Yes (delete directly on device) |
| **Audio Recordings** | **No** (Processed locally) | **No** | Local sound in recorded videos | N/A | Yes (delete directly on device) |
| **Device or other identifiers** (Advertising ID) | Yes (by AdMob SDK) | Yes (Google AdMob partners) | Advertising, analytics, fraud prevention | No | Yes (via Google Ads settings reset) |
| **Crash logs & diagnostics** | No remote upload | No | Handled locally via on-device crash screen | Yes | N/A |

### Data Safety Highlights for Play Store Reviewers:
- **Data Encrypted in Transit:** All external network calls (map tiles, weather, ads) utilize HTTPS encryption.
- **Independent Security Review:** Designed according to Android Scoped Storage and Google Play Data Minimization principles.
- **Account Creation Required:** **No**. GPSnap can be fully utilized without creating any account or submitting personal credentials.

---

# User Guide: Managing Permissions & Deleting Data

### How to Manage Permissions on Android
1. Open your device's **Settings**.
2. Tap **Apps** (or **Application Manager**) → Select **GPSnap**.
3. Tap **Permissions**:
   - **Location:** Select *Allow only while using the app* or *Don't allow*.
   - **Camera:** Select *Allow only while using the app* or *Don't allow*.
   - **Microphone:** Select *Allow only while using the app* or *Don't allow*.
   - **Photos and Videos:** Toggle access as desired.

### How to Request Support Data Deletion
Send an email to [contact@aniket.one](mailto:contact@aniket.one) with:
- **Subject:** `Data Deletion Request - GPSnap`
- **Body:** Please state your request to delete any past email correspondence or support logs. All requests are permanently fulfilled within 30 days.
