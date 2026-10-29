# PracticalCover

A free web app that helps engineering and diploma students create a professional **practical / lab record cover page** in seconds. Fill in your details, watch the A4 cover update live, then download it as a PDF or print it.

Built for students of **Odisha University of Technology and Research (OUTR), Bhubaneswar**, and fully editable for any institution.

## Features

- **Live A4 preview** (210 × 297 mm) that updates as you type
- **6 cover templates**
  - Classic Formal
  - Minimal Clean
  - OUTR Official
  - Modern Bold
  - Technical Drawing
  - Elegant Serif
- **Course, branch and semester selectors**: 20+ engineering branches, with a custom option for course, branch and semester
- **Student and subject fields**: name, registration no., roll no., section, group, sub-group, subject, subject code, faculty, session
- **Optional fields** you can show or hide, plus a one-click **Reset**
- **Download PDF** (jsPDF + html2canvas) and **Print Cover** (dedicated A4 print CSS)
- Responsive layout, light and dark theme, `prefers-reduced-motion` support
- **Privacy first**: no account, no backend, no tracking. Your details never leave your browser.

## Tech Stack

| Part | Tool |
| --- | --- |
| UI | React 18 (UMD build via CDN) |
| Styling | Vanilla CSS (custom properties, grid, print styles) |
| PDF | jsPDF 2.5.1 + html2canvas 1.4.1 |
| Fonts | Outfit, IBM Plex Mono (Google Fonts, with system fallbacks) |

The whole app is a single `index.html` file. There is no build step.

## Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/practicalcover.git
   cd practicalcover
   ```
2. Open `index.html` in a browser, or serve it locally:
   ```bash
   python3 -m http.server 8000
   ```
   Then visit `http://localhost:8000`.

An internet connection is needed on first load for the CDN scripts and fonts.

## Deploy

Any static host works:

- **GitHub Pages**: Settings → Pages → deploy from the `main` branch, root folder
- **Netlify / Vercel**: drag and drop the folder, or connect the repo (no build command, publish directory `.`)

## Usage Tips

- **Download PDF** renders the cover as a high-resolution A4 PDF.
- **Print Cover** prints only the cover page. In the print dialog, set **Margins: None**, untick **Headers and footers**, and choose **Save as PDF** to export.
- Leave any field empty and it is simply left off the cover.

## Project Structure

```
practicalcover/
├── index.html   # the complete app (markup, styles, React code, embedded logo)
└── README.md
```

## Roadmap

- Convert to a Vite + TypeScript project with separate components
- Open Graph preview image
- Optional saved profiles in localStorage (with a clear reset)
- More institution presets

## Disclaimer

PracticalCover is an unofficial student tool. It is not affiliated with or endorsed by OUTR or any other university. The OUTR logo belongs to its respective owner and is used here only to help OUTR students format their own records.

## Author

**Ajit Kumar Patra**, B.Tech CSE, OUTR Bhubaneswar

© PracticalCover
