---
layout: page
title: "TurkEye: AI-Powered Content Moderation"
description: "A Chrome extension + backend AI system that detects and blocks deepfakes, explicit AI-generated images, and misinformation in real time."
img: /assets/img/turkeye.gif
importance: 2
category: projects
---

# Welcome to TurkEye 🦃

The internet can be a wild place, and AI isn’t making it any easier. Deepfake images? Misinformation?
AI-generated explicit content? It’s everywhere. **TurkEye** filters out the digital junk before it reaches users
(especially minors).

## Why a Turkey?
Most people associate Harvard's mascot with John Harvard, but did you know that Harvard’s unofficial symbol is
actually a **turkey**? 🦃 Sharp-eyed and always alert—perfect for an AI watchdog that fights deepfakes.

---

## Architecture

![TurkEye Architecture](/assets/img/turkeye_architecture.png)

*Figure: Chrome Extension (frontend) streams media to a FastAPI decision pipeline (backend) which orchestrates
deepfake detection models (CNN/ViT), Google Cloud Vision SafeSearch, and fact-checking services. The pipeline
returns block/blur/allow actions to the browser in real time.*

---

## The Problem: AI-Generated Chaos

### Why Are We Doing This?
- AI-generated deepfakes and explicit content are widely accessible.
- Cybercriminals use AI to deceive people.
- Reliable, automated client-side blocking is still rare.

### Who Needs Protection?
- **Minors & young users** – They don’t always know what’s real.
- **Parents & guardians** – Because explaining deepfakes over dinner is awkward.
- **Non‑tech‑savvy users** – They often trust what they see.

---

## Our Grand Plan: Smarter AI, Safer Internet

### Mission Objectives
- ✅ **Block AI-generated deepfake images** – If it’s fake, it’s gone.
- ✅ **Blur AI-generated explicit content** – Some things are better left unseen.
- ✅ **Flag harmful AI-generated media before it reaches users** – Catch it before it spreads.
- ✅ **Detect fake news and misinformation** – AI-generated nonsense doesn’t belong in your feed.

---

## The Tech Behind TurkEye: Making AI Fight AI

### Frontend: Google Chrome Extension
Our product is a Chrome extension that filters AI-generated junk in real time.  
The mascot (the Harvard Crimson Turkey) has three states:
1. **Resting** – Just chilling. 🦃  
2. **Inspecting** – Searching for sus content. 🤔  
3. **Deepfake Found** – Sound the alarms! 🚨

### Backend: AI-Powered Image/Content Analysis
**Google Cloud Vision API**
- Detects labels, text (OCR), and **SafeSearch** (adult/violent content).
- Flags facial manipulations or suspicious blurs/artifacts.
- Scans for indicative keywords (“fake,” “edited,” “Photoshop”).

**Deepfake Detection Models (Hugging Face)**
- Vision Transformer (ViT) / CNN models trained on real vs. fake datasets.
- Cross-validates predictions with multiple models for robustness.

**Misinformation / Fact-Checking**
- Extracts claims and cross-references using Google Fact Check tools / LLM assistance.

---

## More Features
- 🔞 **Nudes Detection:** Uses Google Cloud’s AI to detect and blur explicit AI-generated imagery.
- 🎬 **AI‑Generated Video Checks:** Pauses or blocks deceptive AI-generated videos.
- 📰 **Fake News Filtering:** Surfaces fact-checks for suspicious articles.

---

## Future Plans
- 🚀 **Real-time moderation for live streams**
- 📱 **Mobile integration**
- 🤝 **Partnerships with social media platforms**

---

## Meet TurkEye: The AI Turkey That Pecks at Fake Content

AI-generated junk doesn’t stand a chance. With TurkEye watching over your screen,
you can browse with confidence.

🦃 **Team TurkEye — Protecting the Web, One Deepfake at a Time**