---
layout: page
title: Privacy Policy
include_in_header: false
---

# Chorex Privacy Policy

**Last Updated:** November 15, 2025

## Introduction

Chorex ("we", "our app") is an iOS and watchOS application designed for fair and organized distribution of household chores among members of a single group (house). We take your privacy seriously and are committed to protecting your personal data.

This privacy policy explains what data we collect, how we use, store, and protect it.

## 1. Data We Collect

### 1.1 Account Data
When you register, we collect:
- **Email address** — for authentication and sign-in
- **Password** — stored encrypted via Supabase Auth
- **Username** — displayed to other members of your house

### 1.2 House and Chore Data
During app usage, we store:
- **House information**: house name, owner ID
- **Chore information**: chore name, first due date, repeat interval, executor queue
- **House membership**: list of participants in each house
- **Completion history**: records of completed chores with date and executor

### 1.3 Technical Data
To ensure app functionality, we collect:
- **Push notification tokens** — for sending chore notifications and data synchronization
- **Platform information** (iOS/watchOS) — for correct notification delivery
- **JWT tokens** — for API request authentication (stored locally in Keychain)

### 1.4 Notification Settings
- **Notification time** — preferred time for receiving chore reminders
- **Per-chore notification parameters** — individual settings for each chore

## 2. How We Use Your Data

### 2.1 Core Functionality
- Creating and managing houses and chores
- Distributing chores among house members using a cyclic queue system
- Synchronizing data between your devices (iPhone, Apple Watch)
- Displaying current chore information in widgets

### 2.2 Notifications
- Sending reminders about upcoming chores
- **Silent push notifications** — automatic data synchronization between house members' devices without visible notifications
- Background data updates when other participants modify chores

### 2.3 Shared Usage
- Providing access to your houses and chores to other participants you've added
- Displaying your name to other house members
- Sharing chore completion data within your house

## 3. How We Store and Protect Your Data

### 3.1 Data Storage
- **Supabase (PostgreSQL)** — primary database for storing users, houses, and chores
- **Keychain** — local secure storage for JWT tokens and identifiers on your device
- **UserDefaults** — local caching of non-sensitive data for offline access
- **App Groups** — data sharing between main app, widgets, and Apple Watch

### 3.2 Security
- **Encryption in transit**: all data transmitted via secure HTTPS connection
- **Row Level Security (RLS)**: database-level access policies ensure users can only access their own data
- **Authentication**: time-limited JWT tokens for all API requests
- **Apple Keychain Services**: system-level encryption for token storage on device
- **APNS (Apple Push Notification Service)**: secure notification delivery through Apple infrastructure

### 3.3 Access Policies
- Only you and members of your house can see that house's chores
- House owner can add and remove participants
- Each participant can view and complete chores assigned to them
- Push tokens are only accessible for sending notifications and automatically deleted on sign-out

## 4. Third-Party Data Sharing

We **DO NOT sell or transfer** your personal data to third parties.

### 4.1 Service Providers
We use the following services to ensure app functionality:
- **Supabase** — database hosting and user authentication
- **Apple Push Notification Service (APNs)** — notification delivery to devices

These services use your data exclusively for providing app functionality and comply with strict security standards.

### 4.2 In-App Sharing
Your data (name, completed chores) is visible only to users with whom you share a house. You control who to add to your houses.

## 5. Your Rights

### 5.1 Data Access
You can view all your data in the app at any time:
- List of your houses and chores
- Chore completion history
- Profile information

### 5.2 Data Modification
You can:
- Change username in profile settings
- Edit chores and house settings
- Manage notification settings

### 5.3 Data Deletion
You can:
- Delete specific chores
- Leave a house (your data will be removed from that house)
- Delete your house (if you're the owner)
- **Complete account deletion** — by contacting us via email (see "Contact" section), all your data will be permanently deleted

### 5.4 Data Export
To receive a copy of your data, contact us via email (see "Contact" section).

## 6. Data Retention

### 6.1 Retention Period
- **Active accounts**: data stored while you use the app
- **Inactive accounts**: we may delete inactive account data after 2 years of inactivity with prior notification
- **Push tokens**: automatically deleted on sign-out
- **Chore history**: stored indefinitely until house or chore deletion

### 6.2 Deletion on Sign-Out
When signing out:
- JWT tokens removed from Keychain
- Push notification tokens deleted from database
- Local cache cleared

## 7. Cookies and Tracking

**We DO NOT use cookies, analytics, or tracking systems.**

The app does not contain:
- Advertising
- Analytics systems (Google Analytics, Facebook Pixel, etc.)
- User behavior tracking systems

The only technical data we collect is what's necessary for app functionality (see Section 1).

## 8. Children

The app is not intended for children under 13 years old. We do not knowingly collect personal data from children under 13. If you learn that a child has provided us with personal data, please contact us, and we will delete that information.

## 9. Privacy Policy Changes

We may periodically update this privacy policy. For significant changes, we will notify you:
- Through in-app notification
- Via email (if applicable)
- By updating the "Last Updated" date at the top of this document

We recommend regularly reviewing this policy to stay informed about how we protect your data.

## 10. International Data Transfer

The app uses Supabase for data storage. Supabase servers may be located in different countries. By using the app, you consent to transferring your data to these jurisdictions. We ensure compliance with international data protection standards, including GDPR (where applicable).

## 11. Legal Compliance

### 11.1 GDPR (General Data Protection Regulation)
For users in the European Union:
- **Legal basis for processing**: contractual obligations and consent
- **Data subject rights**: access, rectification, erasure, portability, restriction of processing
- **Retention period**: only as long as necessary
- **Right to object**: you can object to processing of your data

### 11.2 CCPA (California Consumer Privacy Act)
For users in California:
- We do not sell personal data
- You have the right to know what data we collect
- You have the right to deletion of data
- You have the right to opt-out of data sales (not applicable, as we don't sell data)

## 12. Data Security

### 12.1 Our Security Measures
- Data encryption in transit (TLS/HTTPS)
- Secure password storage (bcrypt hashing via Supabase Auth)
- Row Level Security in database
- Regular dependency updates to address vulnerabilities
- Data minimization principle

### 12.2 Your Responsibility
To protect your account:
- Use a strong password
- Don't share your credentials with others
- Keep the app updated
- Report suspicious activity to us

## 13. Logging and Debugging

During operation, the app maintains local logs for debugging. These logs:
- Stored only on your device
- Do not contain personal data (passwords, email)
- Not transmitted to external servers
- Can be disabled in the app's Debug Menu settings

Logging categories include:
- Storage operations (data handling)
- Watch synchronization (Apple Watch)
- Notifications (scheduling and delivery)
- Widget updates
- Authentication
- General debug information

## 14. Contact

If you have questions, concerns, or requests regarding this privacy policy or handling of your data, please contact us:

**Email**: [dmytro.bahinskyi@gmail.com]

**Response time**: we strive to respond to all requests within 14 business days.

---

## Quick Summary

**What we collect:**
- Email, name (username)
- Chore data
- Push notification tokens

**Why:**
- App functionality
- Device synchronization
- Chore notifications

**Protection:**
- HTTPS encryption
- Keychain for tokens
- Row Level Security in database
- No advertising or tracking

**Your rights:**
- Data access
- Data modification
- Account deletion
- Data export

**Third parties:**
- Supabase (database hosting)
- Apple (APNS notifications)
- No data sales

---

*Privacy Policy created: November 15, 2025*
