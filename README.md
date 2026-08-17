# Adhikaar Saathi

Adhikaar Saathi is a student capstone MVP for a privacy-first, multilingual domestic violence support app for India. It gives victims, witnesses, and first responders plain-language rights information, incident reporting, evidence preservation, nearby help, and 24/7 guidance with safety defaults built into every screen.

## Phase Scope

### Phase 1: Demoable MVP

- React Native mobile app, Android first and iOS compatible through Expo.
- Anonymous guest mode and optional PIN lock.
- Quick Exit on every app screen that moves to a neutral calculator screen.
- Multilingual UI picker with English plus 21 Indian languages; curated legal-rights text is available in English and Hindi, with a safe English fallback for languages awaiting legal review.
- Incident report form saved locally first.
- Evidence vault metadata flow with sensitive-screen lock.
- Nearby help directory using safe mock data for demo.
- 24/7 guidance screen with scripted safety triage and emergency contacts.
- Express REST API skeleton for auth, reports, evidence metadata, legal content, and help directory.

### Phase 2: Advanced Features

- PostgreSQL 16 persistence, Redis sessions/cache, and S3-compatible encrypted evidence object storage.
- Firebase Auth or hardened custom JWT with OAuth 2.0.
- Google Maps native SDK integration and location-based provider ranking.
- RAG-based legal chatbot using curated Indian law and service-provider sources.
- ML risk scoring, multilingual voice input, OCR evidence indexing, admin web console, and NGO/police/legal aid integrations.

## Run Locally

Install dependencies:

```bash
npm install
```

Start the mobile app:

```bash
npm run mobile
```

Start the API skeleton:

```bash
npm run api
```

## Safety UX Principles

- Sensitive screens require an app PIN before reports, evidence, or guidance history can be opened.
- Guest mode is a full first-class path.
- Quick Exit is persistent and switches instantly to a neutral calculator.
- No notification preview copy is included in Phase 1.
- Content is written for low digital literacy and avoids legalese.

This is not a substitute for emergency services, legal counsel, or medical care.
