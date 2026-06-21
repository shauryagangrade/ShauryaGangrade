# Shaurya Gangrade

**Building practical systems with AI — across domains**

> I like working on real problems, even outside my main interests — figuring them out, and building something that actually works.

---

## About Me

I’m a developer who enjoys **figuring out messy, real-world problems and turning them into working systems**.

I’m not tied to one domain — I care more about:

* How systems behave in the real world
* How to extract signal from noisy data
* How to go from idea → working prototype quickly

---

## What I've Built

### 🔐 PlaceMate

**A local-first, encrypted system for managing personal physical inventory**

Built PlaceMate as a privacy-first application for tracking real-world items (documents, valuables, storage locations) without relying on cloud infrastructure.

The system is designed around a core principle:

> Sensitive physical inventory data should never leave the user’s device.

---

**What it does:**

* Lets users log items using natural language (e.g., *"Put passport in blue drawer"*)
* Parses and structures item–location relationships automatically
* Enables fast retrieval via conversational queries (e.g., *"Where is my passport?"*)
* Stores all data locally with **AES-256 encryption**

---

**System Design Highlights:**

* **Client-side architecture:** Entire system runs in the browser (no backend, no telemetry)
* **Cryptography pipeline:**

  * PBKDF2-based key derivation from master password
  * AES-256-CBC encryption with randomized IVs
* **Secure password rotation:**

  * Full decrypt → re-encrypt cycle with new key
  * Enforces non-reuse of previous passwords
* **Mnemonic recovery system:**

  * 12-word recovery phrase
  * Used to securely encrypt and recover the master password
* **Local storage engine:**

  * IndexedDB/localStorage for encrypted state persistence

---

**What I built:**

* Designed the **end-to-end client-side architecture** (UI ↔ NLP ↔ crypto ↔ storage)
* Implemented **secure state management and encryption flows**
* Built a lightweight NLP-style parser for extracting structured data from user input
* Developed recovery and export systems with explicit security safeguards
* Focused on making strong security usable in a real product

---

**Key takeaway:**

> PlaceMate is not just a UI app — it’s a system that balances usability with strict security constraints, entirely on the client side.

---

**Tech:** Next.js / Vite · TypeScript · CryptoJS · IndexedDB

↗ GitHub: https://github.com/shauryagangrade/PlaceMate

↗ Live: https://place-mate-weld.vercel.app


### 🔍 Mule Account Detection (POC)

**Applied ML to a real-world financial fraud problem**

Worked on a proof-of-concept system to detect potential mule accounts using transaction behavior.

This wasn’t a domain I originally focused on — I picked it up while helping on a real problem and built a working prototype.

**What I did:**

* Understood the problem space (how mule accounts operate)
* Translated it into a machine learning problem
* Built a pipeline for feature extraction + classification
* Generated risk signals based on behavioral patterns

**Key takeaway:**
This project wasn’t about finance — it was about:

> Taking a vague, real-world problem and turning it into a concrete ML system.

**Tech:** Python · Machine Learning

↗ GitHub: https://github.com/shauryagangrade/mule-account-detection-poc

---

### 🗺️ StudyMap

**A crowdsourced map of student-relevant places across the Mumbai Metropolitan Region**

Co-developed StudyMap with Anay Dhawan — an open-source platform that helps students discover important locations like exam centres, libraries, book shops, stationery stores, internet cafés, and transit points across Mumbai, Thane, and Navi Mumbai.

The system is designed to be **simple, accessible, and community-driven** — with zero setup and a fully GitHub-based contribution model.

**What I did:**

* Worked on structuring location data into a consistent, scalable schema
* Helped design the data ingestion model (JSON-based, category-wise storage)
* Built parts of the frontend map experience and filtering logic
* Contributed to system design for handling crowdsourced data reliably

**Key takeaway:**
StudyMap was about:

> Building a real-world utility by structuring messy, distributed information into a clean, usable system.

**Tech:** Next.js · Leaflet · TypeScript · Tailwind

↗ GitHub: https://github.com/AnayDhawan/StudyMap

↗ Live: https://study-map-psi.vercel.app

---

## Open Source Contribution — Tournament Parser Enhancement

Contributed enhancements to improve tournament parsing accuracy, particularly for South Asian and colloquial contexts.

### Key Improvements

* Added support for Indian/Hinglish synonyms such as *"bijli"*, *"tez"*, *"shastriya"*, and *"jaldi"*
* Expanded detection logic for tournament categories including *blitz*, *rapid*, and *classical* to handle informal naming variations
* Improved FIDE rating recognition to include patterns like *"fide rated"*, *"rating tournament"*, and *"elo"*
* Increased parser accuracy for regional and non-standard tournament formats

### Impact

These changes make the parser more inclusive and robust when handling real-world tournament data, especially from South Asian sources where naming conventions often differ from standard formats.

### Technical Notes

* Fully type-safe (no `any` types introduced)
* Successfully builds with TypeScript
* No credentials or sensitive data included
* Follows existing project conventions for scraper structure and ID generation

Live: https://www.tourneyradar.com
GitHub: https://www.github.com/AnayDhawan/Tourneyradar

---

## Technical Toolkit

**Core:**
Python · Problem-solving · Systems thinking

**Exploring:**
Applied ML · Real-world data systems

---

## How I Think

I like working on problems where:

* The data is messy
* The solution isn’t obvious
* You have to figure things out from scratch

I’m less interested in polished demos, and more in:

> Can I take a real problem and make something that actually works?

This project is one example of that.

## Github Stats

[![GitHub Streak](https://streak-stats.demolab.com/?user=shauryagangrade)](https://git.io/streak-stats)








<!--
**shauryagangrade/ShauryaGangrade** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
