# Aura Peak Sanctuary — Mountain Boutique Hotel

> **A Secluded Luxury Retreat 2,480m Above The Clouds**

An ultra-premium, interactive 6-stage scroll-driven 3D cinematic canvas website built with 1,560 high-definition frames across the complete guest journey from high aerial clouds down into the private hill track veranda.

---

## 🗺️ Chronological Folder Sequence & Frame Breakdown

The website's continuous LERP canvas engine scrubs seamlessly through the 6 chronological folders:

| Order | Folder | Frames | Experience & Scene |
|---|---|---|---|
| **01** | `hero/` | 300 frames (`001`–`300`) | **Above the Clouds** · Aerial drone reveal dropping through mountain fog to the summit chalet |
| **02** | `Section_2/` | 240 frames (`001`–`240`) | **The Arrival Hearth** · Heated cedar deck, sunken granite fire pit, and glass entrance doors |
| **03** | `Section_3/` | 240 frames (`001`–`240`) | **Panoramic Corridor** · Minimalist Scandinavian vertical oak slats & floor-to-ceiling glass gallery |
| **04** | `Section_4/` | 240 frames (`001`–`240`) | **The Master Suite** · King cloud bed, suspended blackened steel hearth & 180° corner mountain view |
| **05** | `Section_5/` | 240 frames (`001`–`240`) | **Volcanic Stone Spa** · Monolithic basalt soaking tub positioned flush against the misty cliff drop |
| **06** | `Section_6/` | 300 frames (`001`–`300`) | **Hill Track Veranda** · Cantilevered wooden balcony, steaming coffee mug & vast green mountain valley |

**Total Cinematic Sequence: 1,560 Full HD Frames**

---

## ✨ Features & Architecture

- **Unified Multi-Stage Canvas Engine**: Mathematically resolves global scroll progress ($0.0 \to 1.0$) across all 1,560 frames without seams or jumps.
- **Two-Stage Preloader**: Paints Frame 1 of `hero` in $<150\text{ms}$, checks 12 strategic keyframes across all 6 sections, dismisses cleanly, and background-pumps proximity frames.
- **Bi-Directional Fallback**: Missing frames immediately fallback to the closest loaded neighbor, eliminating black flashes during fast wheel or touch scrolling.
- **Right-Hand Interactive Timeline Rail**: 6 interactive stage dots highlight dynamically in sync with your scroll position and allow one-click jumping to any section.
- **Luxury Boutique Design Tokens**: Frosted glassmorphism (`backdrop-filter: blur(24px)`), warm amber firelight accents (`#E6A756`), and editorial serif typography (`Cormorant Garamond` + `Outfit`).
- **Live Booking Engine & Modal**: Interactive date picker, suite selector, and reservation confirmation drawer.

---

## 🚀 Running Locally

1. Open your terminal in this directory:
   ```bash
   cd "d:/my company 2026/10k dollar website/hotel on top of the mountain"
   ```

2. Start the zero-dependency dev server:
   ```bash
   node server.js
   ```

3. Open in browser:
   ```
   http://localhost:5175/
   ```

---

## 🌐 Production Deployment (Vercel)

Configured in `vercel.json` with 1-year immutable caching for all 6 image sequence folders:
```bash
npx vercel --prod
```
