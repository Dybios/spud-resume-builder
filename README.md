# Spud Resume Builder

A 100% free, client-side, privacy-first automated resume engine and builder. Designed to parse, format, and generate clean, ATS-compliant single or multi-page resumes directly in your browser with zero server roundtrips or data storage.

![Spud Resume Builder Workspace](https://img.shields.io/badge/status-active-success.svg)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Privacy](https://img.shields.io/badge/privacy-100%25%20Client--Side-orange.svg)

---

## Key Features

- **Zero-Backend & Local-First:** All processing happens entirely in client memory. Your data never leaves your device.
- **Precision ATS Canvas:** Locked to exact US Letter pixel specifications (`816px` width) matching `html2pdf.js` metrics to eliminate layout regressions and export clipping.
- **Multi-Format Importer & Parser:** 
  - **PDF Parser (`pdf.js`):** Extracts text with advanced coordinate-sorting logic (`Y` baseline grouping and strict left-to-right `X` sorting) to handle complex or multi-column resume layouts cleanly.
  - **Word Parser (`Mammoth.js`):** Direct XML and binary stream parsing for `.docx` and `.doc` files.
  - **JSON Backup:** Fast, lossless local state exports and imports.
- **Live Page Length Tracker:** A reactive floating status pill that computes true content flow heights against printable page limits, letting you effortlessly track 1-page fits or multi-page layouts.
- **Advanced Styling & Typography Toolbar:**
  - Dynamic ATS-safe font switcher (Helvetica/Inter, Times New Roman, Garamond, Arial, Georgia).
  - Real-time **Font Size Scale** slider with dynamic stylesheet injection to scale all headings, body text, and points smoothly.
  - Granular **Page Margin** customizer.
  - One-click primary accent color presets and custom color picker.
- **Word Document DOCX Export:** To allow ATS-based parsers to properly grab all data. Let user create a PDF from the word file if needed.
- **Live Client-Side Telemetry Modal:** Transparent real-time browser proof showing 0 outbound network requests and local storage footprint tracking (`F12` inspection ready).

---

## Tech Stack

- **Framework & UI:** HTML5, Vanilla JavaScript, **Tailwind CSS** (via CDN)
- **Document Parsing:** `pdf.js` (PDF text stream re-construction) & `Mammoth.js` (.docx XML extraction)
- **Icons & Fonts:** FontAwesome 6, Google Fonts

---

## Getting Started

To jump straight in and start building your resume right away, visit the live app here:

**[Spud Resume Builder Live Site](https://spudresume.in)**

### For Advanced Developers (Local Setup & Cloning)
If you want to contribute, run a local development instance, or modify the source code:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dybios/spud-resume-builder.git
