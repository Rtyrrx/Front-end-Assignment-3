# Assignment 3 – Flexbox & Grid Report

Date: 2025-10-06

## Overview
This project implements all parts of the assignment using semantic HTML and modern CSS (Flexbox & Grid). The visual theme is minimal and consistent to emphasize layout techniques.

## Part 1. Flexbox

### Task 0. Navigation Bar
- Implemented in all pages (`index.html`, `grid.html`, `portfolio.html`).
- Header container uses Flexbox: `.header-inner { display: flex; align-items: center; justify-content: space-between; gap: 1rem; }`.
- Links spaced with `gap` on `.nav-list`.
- Vertically centered via `align-items: center`.

### Task 1. Card Row
- Section in `index.html` with three cards.
- Container uses Flexbox: `.card-row { display: flex; gap: 1.25rem; align-items: stretch; flex-wrap: wrap; }`.
- Equal heights achieved because cards are flex items with `align-items: stretch` and `.card` uses `display: flex; flex-direction: column;`.
- Hover effect: `.card:hover { transform: translateY(-4px); box-shadow: 0 18px 40px rgba(0,0,0,.35); }`.

## Part 2. Grid System

### Task 2. Page Layout with Grid Areas
- Implemented in `grid.html` with container `.grid-areas` using `grid-template-areas`.
- Areas:
  - Header spans top
  - Sidebar left
  - Main right
  - Footer bottom
- Responsive single-column fallback below 800px.

### Task 3. Image Gallery
- Implemented in `grid.html` as `.gallery` with 3x3 grid and `gap: 12px`.
- Hover caption overlay via `figcaption` translateY animation on `.gallery-item:hover figcaption`.

## Part 3. Combining Flexbox & Grid

### Task 4. Portfolio Page
- Implemented in `portfolio.html`.
- Header: Flexbox nav reused.
- Main: CSS Grid splits `.portfolio-layout` into `1fr 320px` (projects left, info right).
- Projects: `.projects-grid` auto-fills cards; each `.project-card` uses Flexbox inside for title, text, and actions. Buttons are pinned with `.card-actions { margin-top: auto; }`.
- Footer spans full width.

## Design & Code Quality
- Consistent spacing, color variables, and component classes.
- Accessible semantics: header/nav/main/aside/footer, alt text, `aria-current`.
- Responsive behavior for narrow screens.

## Screens (Describe or paste images)
- Flexbox Nav & Cards (index)
- Grid Areas & Gallery (grid)
- Portfolio page layout (portfolio)

## Summary
All tasks and evaluation criteria are covered with clean, readable code. See files:
- `index.html`, `grid.html`, `portfolio.html`
- `css/styles.css`
- `assets/images/*.svg`
- `js/main.js`
