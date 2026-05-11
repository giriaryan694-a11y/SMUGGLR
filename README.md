# SMUGGLR

Invisible Unicode Payload Toolkit 🔓

SMUGGLR is a fully client-side Unicode steganography playground built for security researchers, red teamers, detection engineers, CTF players, and curious developers exploring text obfuscation techniques.

🌐 Live Demo: [https://giriaryan694-a11y.github.io/SMUGGLR/](https://giriaryan694-a11y.github.io/SMUGGLR/)

---

## Overview

Modern platforms trust text too much.

Invisible Unicode characters, homoglyph substitutions, and combining marks can be abused to:

* Hide hidden messages inside normal-looking text
* Bypass naive keyword filters
* Poison datasets or prompts
* Obfuscate payloads in chats, markdown, or documents
* Demonstrate Unicode security risks in a safe lab environment

SMUGGLR packages multiple Unicode smuggling techniques into a single browser-based toolkit with zero backend infrastructure.

Everything runs locally in your browser.
No uploads. No telemetry. No network calls.

---

# Features

## 6 Built-In Techniques

### 1. Zero-Width Encoding

Hides binary-encoded payloads using invisible Unicode characters:

* U+200B → Zero Width Space
* U+200C → Zero Width Non-Joiner

The payload is stitched invisibly inside cover text.

### 2. Tag Block Encoding

Uses the Unicode Tags block (`U+E0000`) to embed hidden text.

This is similar to techniques seen in:

* AI watermarking research
* Unicode metadata tricks
* Invisible annotation systems

Completely invisible in most:

* Browsers
* Chats
* Documents
* Markdown renderers

### 3. Homoglyph Obfuscation

Swaps Latin characters with visually identical:

* Cyrillic
* Greek
* Unicode lookalikes

Examples:

| Normal | Homoglyph |
| ------ | --------- |
| a      | а         |
| o      | о         |
| p      | р         |
| c      | с         |

Useful for demonstrating:

* Filter bypasses
* Phishing risks
* Detection evasion
* Unicode normalization issues

### 4. Zalgo Generator

Adds combining Unicode marks:

* Above text
* Below text
* Through text

Includes adjustable intensity controls.

### 5. Whitespace Cipher

Encodes binary using:

* EM Space (`U+2003`)
* EN Space (`U+2002`)

The encoded payload hides between words while remaining visually invisible.

### 6. Inspector

Paste suspicious text and SMUGGLR scans for:

* Zero-width payloads
* Tag block abuse
* Homoglyph substitutions
* Zalgo combining marks
* Whitespace binary ciphers

Automatic decoding included.

---

# UI Highlights

* 🌑 Dark Theme
* ☀️ Light Theme
* 👁 Eye-Saver Theme
* Sticky technique selector navbar
* Encode + Decode actions per panel
* One-click copy output
* Animated glitch logo
* Scanline overlay terminal aesthetic
* Responsive browser UI

---

# Why SMUGGLR Exists

Unicode abuse is massively underestimated.

Most developers assume text is harmless.
In reality, invisible Unicode characters can:

* Alter parsing behavior
* Break moderation systems
* Hide instructions inside prompts
* Poison LLM datasets
* Evade detection pipelines
* Create phishing lookalikes
* Confuse logging and SIEM systems

SMUGGLR exists to help researchers understand these risks through hands-on experimentation.

---

# Example Use Cases

## Security Research

Analyze:

* Unicode obfuscation
* Prompt injection tricks
* AI watermarking concepts
* Detection evasion methods

## CTF Challenges

Create:

* Hidden payloads
* Unicode puzzles
* Invisible clues
* Stego-based tasks

## Detection Engineering

Test:

* Unicode normalization
* Filtering systems
* Logging pipelines
* Alerting mechanisms

## Awareness & Education

Demonstrate:

* Homoglyph phishing
* Invisible characters
* Unicode parser confusion
* Text security pitfalls

---

# Tech Stack

* HTML
* CSS
* Vanilla JavaScript
* Pure client-side execution

No frameworks.
No backend.
No dependencies.

---

# Project Philosophy

SMUGGLR is designed as:

* A research tool
* A learning playground
* A Unicode security lab
* A detection-testing utility

The goal is understanding Unicode abuse — not malicious deployment.

---

# Security Notes

Some techniques demonstrated here may trigger:

* Spam filters
* Unicode sanitizers
* Security tooling
* Content moderation systems

This project is intended for:

* Educational use
* Research
* Defensive testing
* Security experimentation

---

# Future Ideas

Potential future additions:

* Bidirectional override attacks
* UTF-8 corruption demos
* Unicode normalization analyzer
* AI prompt watermark detector
* Regex bypass visualizer
* Unicode entropy scoring
* Multi-layer payload chaining

---

# Credits

Made By Aryan Giri

GitHub: giriaryan694-a11y


---

# Final Note

Text is an attack surface.

Unicode is bigger, weirder, and more dangerous than most systems assume. 🎯
