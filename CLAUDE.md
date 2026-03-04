# Website Repo — Claude Instructions

This repository is the legal compliance website for **OPAL HARMONY Ι.Κ.Ε.**, a Greek private capital company (Ιδιωτική Κεφαλαιουχική Εταιρεία). Greek law requires IKE companies to publish certain company information and annual financial statements publicly.

## Repo Overview

- **GitHub:** `opalharmonyco/website` (public)
- **Deployed at:** https://opalharmony.gr/ (custom domain via CNAME)
- **GitHub Pages source:** root `/` on `main` branch
- **Status:** Built and live

## Files

```
website/
├── index.html              # Main page (Greek) — company info + balance sheet
├── CNAME                   # opalharmony.gr — custom domain config
└── isologismos-2024.pdf    # 2024 annual balance sheet PDF (downloadable)
```

## What the Site Contains

The site is a single static HTML page in Greek with:

- **Company details:** Name, GEMI number (176908106000), AFM (802467746), DOY (E' Thessalonikis), registered address (Olympou 9, 54630, Thessaloniki), phone (2313 252248), founding date (17/04/2024)
- **Purpose (Skopos):** IT application design/development, online advertising, sales consulting
- **Partners (Etairoi):**
  - Hro Palampougioukis — 100 shares, 5%
  - Orestis Palampougioukis — 1,900 shares, 95% (also sole manager/Diacheiristis)
- **2024 Balance Sheet (Isologismos):** Summary table inline + PDF download link
  - Total assets: €38,930.57
  - Equity + reserves: €19,944.99
  - Short-term liabilities: €18,985.58
- **Status:** Not in liquidation

## Deploy Behavior

GitHub Pages auto-deploys on every push to `main`. No manual deploy step needed.
Custom domain `opalharmony.gr` is configured via the `CNAME` file and GitHub Pages settings.

**After any push to `main`, confirm with the user that the live site updated correctly.**

## When to Update This Repo

- Annual balance sheet updates (new year → update inline table + replace PDF)
- Company detail changes (address, phone, legal status)
- Legal requirement changes that affect what must be published

## Key Rules

- Keep the page in Greek — it's a legal document for Greek authorities
- Do not remove required fields (GEMI, AFM, DOY, partners, balance sheet)
- The PDF `isologismos-2024.pdf` must remain accessible for download
- Never auto-commit. User manages git manually.
