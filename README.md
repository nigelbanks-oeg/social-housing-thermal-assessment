# Social Housing Thermal Assessment Tool

A co-branded interactive assessment tool by **Octopus Energy** and **Healthy Homes Hub** for understanding heating costs, thermal comfort, and health compliance in social housing.

## Overview

This repository contains a static GitHub Pages website featuring:

- **Landing page** (`index.html`) — Article contextualizing the tool, methodology, and key insights
- **Interactive dashboard** (`dashboard.html`) — Physics-based thermal assessment model with real-time calculations
- **Co-branded design** — Octopus Energy × Healthy Homes Hub visual identity

## Quick Start: Deploy to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Create a new repository (e.g., `social-housing-thermal-assessment`)
3. Choose "Public" (required for GitHub Pages)
4. Initialize with a README (optional)

### Step 2: Upload Files

Clone the repository locally:
```bash
git clone https://github.com/YOUR_USERNAME/social-housing-thermal-assessment.git
cd social-housing-thermal-assessment
```

Copy these files into the repository:
- `index.html` — Landing page
- `dashboard.html` — Interactive tool

Commit and push:
```bash
git add .
git commit -m "Add co-branded heating assessment tool"
git push origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository → **Settings**
2. Scroll to **Pages** (left sidebar)
3. Under "Build and deployment":
   - Select **Branch**: `main`
   - Select **Folder**: `/ (root)`
   - Click **Save**

GitHub will generate a URL like: `https://YOUR_USERNAME.github.io/social-housing-thermal-assessment`

### Step 4: Customize (Optional)

**Add a custom domain:**
1. In **Pages** settings, add your domain under "Custom domain"
2. Update your domain DNS records to point to GitHub Pages (see [GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))

**Add logos:**
- Open `index.html` and `dashboard.html`
- Replace the `img src` URLs with your own logo paths:
  - Healthy Homes Hub: Update image URL for HHH logo
  - Octopus Energy: Add your own Octopus logo URL or use text branding

## Files & Structure

```
├── index.html              # Landing page with article context
├── dashboard.html          # Interactive thermal assessment tool
├── README.md               # This file
```

## Content & Features

### Landing Page (`index.html`)

- **Hero section** — Co-branded introduction
- **Article body** — Context on thermal comfort, health, and affordability
- **Key topics covered:**
  - The three pillars of thermal comfort (fabric, heating, budget)
  - Clinical evidence & compliance thresholds
  - Energy price cap data
  - Heat pump + tariff economics
  - Real-world scenario example
  - Key insights for housing providers
  - About Octopus Energy and Healthy Homes Hub

### Dashboard (`dashboard.html`)

**Real-time inputs:**
- Available weekly heating budget (£0–80/wk)
- Outdoor winter temperature (-5°C to +12°C)
- Property size & insulation level (30–150 m²)
- Heating system & tariff (17 options including Octopus Cosy, Tenant Power)

**Calculations:**
- **Thermal steady-state:** Achieved indoor temperature given budget and conditions
- **Cost matrix:** Weekly fuel spend across insulation × heating combinations
- **Seasonal model:** 30-week annual heating season (Oct–April) by UK region
- **Compliance:** HHSRS, Awaab's Law, WHO thresholds

**Outputs:**
- Indoor temperature achieved
- Cost to reach 21°C comfort
- Annual heating cost & budget sufficiency
- Seasonal weekly expenditure profile
- Condensation risk & mould hazard assessment

## Branding

The site uses a purple-to-emerald gradient representing Octopus Energy's purple brand and Healthy Homes Hub's emerald accent color.

**Logos:**
- **HHH:** `https://healthyhomeshub.uk/images/logo-white.svg` (white on dark background)
- **Octopus Energy:** Text-based ("Octopus Energy") or add your own logo

To customize branding, edit the color hex codes in the CSS:
- Purple: `#7c3aed`
- Emerald: `#059669`

## Linking from an Article

To link from your article to the assessment tool:

```markdown
[Open the Interactive Heating Assessment Tool](https://your-domain.com/social-housing-thermal-assessment/dashboard.html)
```

Or link to the full site including context:

```markdown
[Explore the Heating Assessment Tool & Methodology](https://your-domain.com/social-housing-thermal-assessment/)
```

## Technical Details

- **Framework:** Tailwind CSS (via CDN)
- **Charts:** Chart.js (via CDN)
- **Icons:** Lucide Icons (via CDN)
- **No backend required:** Fully static HTML + JavaScript
- **Browser support:** Modern browsers (Chrome, Firefox, Safari, Edge)

## Data & Assumptions

The tool is calibrated with:

- **Energy price cap:** October 2026 confirmed + January 2027 forecast (Cornwall Insight)
- **Heat pump COP:** Empirical data from Centre for Net Zero fleet
- **Regional climate:** UK climate zones with weekly external temperatures
- **Tariffs:** Standard SVT, Economy 7, Octopus Cosy, Octopus Tenant Power, Octopus Zero Bills
- **Building fabric:** HLP values from 0.6 (Passivhaus) to 4.5 W/m²K (solid wall)

## Support & Feedback

For questions or suggestions:
- **Healthy Homes Hub:** [info@healthyhomeshub.uk](mailto:info@healthyhomeshub.uk)
- **Octopus Energy:** [info@octopusenergy.com](mailto:info@octopusenergy.com)

## License

This tool is made available for educational and non-commercial use in the social housing sector. Please credit Octopus Energy and Healthy Homes Hub when sharing or adapting.

---

**Built in October 2026** — Combining physics-based thermal modeling with real-world tariff data to bridge policy intent and lived reality for residents in social housing.
