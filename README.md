# Cars.com Mystery Shop Evaluation Tool

Interactive web tool for evaluating dealer lead response quality across phone, text, email, and chat channels. Used by field representatives to score dealership mystery shops on a 100-point scale with real-time feedback, industry benchmarks, and downloadable PDF reports.

**[Live Demo](https://jakec86.github.io/mystery-shop/)**

## Features

- **100-Point Scoring Rubric** across 8 categories: Text/Voicemail/Email Introductions, Engagement & Conversion, Communication Style, Knowledge, Responsiveness, and Follow-Up
- **Conditional Criteria** by lead type (Internet, Phone, Chat, Walk-In) with automatic section filtering
- **N/A Toggle** on any criterion to remove it from the scoring denominator
- **Real-Time Live Score** updates as criteria are checked
- **Bento Grid Results Dashboard** with animated score ring, expandable section breakdown, and ranked coaching recommendations
- **Industry Benchmarks** calibrated against Pied Piper PSI 2025 (national avg: 65) and top brand scores
- **Financial Impact Estimates** citing DAS Technology NADA 2025 and Foureyes 2025 data
- **Trend Tracking** with sparkline visualization across multiple shops per dealership
- **PDF Report Download** with infographic-style cover, bar chart scorecard, strengths/gaps analysis, and embedded response attachments
- **Response Attachments** upload system for email/text screenshots (base64-embedded in reports)
- **Session Persistence** via localStorage with auto-restore
- **Accessibility** with ARIA roles, keyboard navigation, and screen reader support
- **Responsive Design** for desktop, tablet, and mobile field use

## Scoring Categories

| Category | Max Points | Weight |
|---|---|---|
| Text Introductions | 3 | 3% |
| Voicemail Introductions | 3 | 3% |
| Email Introductions | 4 | 4% |
| Engagement & Conversion | 20 | 20% |
| Communication Style | 10 | 10% |
| Knowledge & Information | 10 | 10% |
| Responsiveness | 25 | 25% |
| Follow-Up | 25 | 25% |
| **Total** | **100** | **100%** |

Rating tiers: **Great** (80%+) | **Average** (50-79%) | **Needs Work** (<50%)

## Benchmark Sources

- [Pied Piper PSI 2025](https://www.piedpiperpsi.com/psi/) — National ILE average: 65, Top brand (Subaru): 77
- [DAS Technology NADA 2025](https://dastechnology.com/) — 61% respond within 15 min, 78% of buyers purchase from first responder
- [Foureyes 2025 Benchmarks](https://foureyes.io/resources/2025-automotive-dealer-benchmarks-report) — 40% internet lead appointment-set rate, 43.2% of leads mishandled

## Tech Stack

Single-file React 18 application — no build step required.

- React 18.3.1 + ReactDOM (CDN)
- Babel Standalone 7.26.9 (in-browser JSX transpilation)
- html2pdf.js 0.10.2 (client-side PDF generation)
- DM Sans + Inter (Google Fonts)
- Cars.com Spark design system tokens

## Usage

Open `index.html` in any modern browser, or visit the [live demo](https://jakec86.github.io/mystery-shop/).

1. **Shop Info** — Enter dealership name, auditor, date, and lead type
2. **Evaluation** — Score each section by checking criteria; upload response screenshots
3. **Results** — Review scores, benchmarks, impact estimates, and coaching recommendations
4. **Download PDF** — Generate a branded infographic report for the dealer

## License

Internal tool — Cars.com
