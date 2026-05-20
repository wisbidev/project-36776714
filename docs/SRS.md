# Software Requirements Specification — Hello Word Website

## 1. Overview

A minimal single-page static website that displays the text **"Hello Word"** centered on screen. The site is built with plain HTML and CSS — no backend, no database, no JavaScript frameworks. Its purpose is to serve as a clean, presentable landing page with responsive design.

## 2. Scope

The entire deliverable is a single `index.html` file with embedded CSS. No server-side logic, no external dependencies, no build tooling.

## 3. Functional Requirements

### Function 1 — Static HTML Page

| ID | Requirement | Acceptance Criteria |
|---|---|---|
| FR-1.1 | The page shall display the heading **"Hello Word"** centered both horizontally and vertically. | The text appears in the middle of the viewport; the layout uses a flexbox or grid centering technique. |
| FR-1.2 | The page shall have a pleasant visual style. | Background colour is soft/neutral (e.g. a light pastel or off-white); font is clean and readable (e.g. system UI stack or a Google Font); heading has appropriate sizing and spacing. |
| FR-1.3 | The page shall be a valid HTML5 document. | DOCTYPE is `<!DOCTYPE html>`, includes `<html>`, `<head>`, and `<body>` tags, and has a `<title>`. |

### Function 2 — Responsive Styling

| ID | Requirement | Acceptance Criteria |
|---|---|---|
| FR-2.1 | The page shall adapt to different screen sizes via CSS media queries. | On screens **≥ 768 px** (desktop/tablet): the heading font size is larger (e.g. 3–4 rem). On screens **< 768 px** (mobile): the heading font size scales down appropriately (e.g. 1.8–2.5 rem) and padding/margins adjust so the layout remains clean and unclipped. |
| FR-2.2 | The page shall not have horizontal scrollbars on any common device width (320 px – 1920 px). | Tested by inspecting the page at 320 px, 768 px, and 1920 px widths. |

## 4. Constraints

- Zero external runtime dependencies (no CDN links, no libraries).
- Single HTML file — all CSS must be inlined in a `<style>` block within `<head>`.
- No JavaScript required.

## 5. Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (no pre-processors) |
| Hosting | Static file hosting (e.g. GitHub Pages / Netlify / any S3) |
| Version Control | Git + GitHub |

## 6. Design

Design: see attached spec.

No Figma design file was created for this project; the visual direction is intentionally minimal (centered text, clean typography, soft background). The styling decisions are left to the developer's discretion, guided by the acceptance criteria above.
