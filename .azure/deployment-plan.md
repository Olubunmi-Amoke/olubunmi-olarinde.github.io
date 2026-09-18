# Portfolio Makeover Plan

> **Status:** Validated

Generated: 2026-09-18

---

## 1. Project Overview

**Goal:** Redesign the complete portfolio with a warm editorial and modern-tech visual system, improve responsive behavior and accessibility, and polish existing copy without changing factual claims.

**Path:** Modify an existing static website.

## 2. Requirements

| Attribute | Value |
|-----------|-------|
| Classification | Production personal portfolio |
| Scale | Small |
| Budget | Cost-optimized |
| Scope | All five HTML pages and the shared stylesheet |
| Content | Tighten existing copy; add a sanitized Microsoft TPM role summary; preserve verified claims |
| Hosting | Preserve the existing GitHub Pages architecture |
| Azure subscription | Not applicable; no Azure resources will be added |
| Azure location | Not applicable; no Azure resources will be added |
| Compliance | No user data collection; preserve safe external-link behavior |

## 3. Components Detected

| Component | Type | Technology | Path |
|-----------|------|------------|------|
| Portfolio pages | Static frontend | Semantic HTML | `*.html` |
| Shared design system | Stylesheet | CSS | `assets/style.css` |
| Portfolio media | Static assets | JPG, PDF, MP4 | `assets/` |

There is no package manager, JavaScript framework, backend, database, container, Azure configuration, or build pipeline.

## 4. Deployment Recipe

**Selected:** Preserve GitHub Pages static hosting; no Azure recipe or infrastructure generation.

**Rationale:** The requested work is a presentation and content redesign. Introducing a new cloud platform, framework, or build tool would add cost and complexity without improving the requested outcome.

## 5. Design and Architecture

**Design direction:** Warm editorial + modern tech.

**System:**

- Warm ivory canvas, ink text, terracotta accent, and deep teal technical accent.
- Editorial display typography paired with a clean sans-serif body face, with robust system fallbacks.
- Shared sticky navigation, active-page states, reusable buttons, cards, badges, section headers, and footer.
- Responsive layouts for the homepage hero, project grid, resume timeline, capstone features, media, and screenshot gallery.
- Semantic landmarks, skip links, visible focus states, descriptive labels, reduced-motion support, and accessible color contrast.
- No JavaScript dependency; all pages remain portable static documents.

## 6. Page Work

| Page | Planned changes |
|------|-----------------|
| `index.html` | Introduce a recruiter-focused hero, concise positioning, expertise highlights, featured-work callouts, and polished contact section |
| `projects.html` | Convert the long project list into scannable case-study cards with outcomes, tools, and consistent calls to action |
| `resume.html` | Create an editorial resume layout with summary, experience, education, skills, certifications, and reliable PDF access |
| `scd-diary.html` | Reframe as a detailed flagship case study with problem, evolution, approach, ethics, access, video, and responsive gallery |
| `ethics-scd.html` | Present the ethics capstone as a focused editorial feature with abstract, themes, and downloadable materials |
| `assets/style.css` | Replace the minimal stylesheet with the shared responsive design system |

## 7. Provisioning Limit Checklist

No resources will be provisioned. Quota and capacity validation are not applicable.

| Resource Type | Number to Deploy | Capacity Status | Notes |
|---------------|------------------|-----------------|-------|
| None | 0 | Not applicable | Existing GitHub Pages hosting is unchanged |

## 8. Execution Checklist

### Planning

- [x] Analyze workspace
- [x] Gather redesign requirements
- [x] Scan codebase
- [x] Confirm hosting impact
- [x] Define shared design system
- [x] User approved this plan

### Implementation

- [x] Build shared page shell and design tokens
- [x] Redesign homepage
- [x] Redesign projects page
- [x] Redesign resume page
- [x] Redesign Smart Sickle Cell Diary case study
- [x] Redesign ethics capstone page
- [x] Polish copy without changing factual claims
- [x] Remove page-level presentation styles in favor of shared CSS

### Verification

- [x] Validate all internal asset and page links
- [x] Validate HTML structure
- [x] Verify responsive layouts at mobile, tablet, and desktop widths
- [x] Verify keyboard focus, landmarks, image alternatives, contrast, and reduced motion
- [x] Preview representative pages in a local browser

## Functional Verification

- Status: Verified
- Backend: Not applicable; static site
- UI: All five pages and the shared stylesheet returned HTTP 200 in the local preview
- Accessibility: Skip links, semantic landmarks, visible focus states, image alternatives, reduced-motion handling, and safe external-link attributes verified
- Privacy: No confidential Microsoft project names, internal systems, architecture, operational metrics, or private links published

## Validation Proof

| Check | Command | Result | Timestamp |
|-------|---------|--------|-----------|
| HTML and asset audit | Native PowerShell audit across all `*.html` files | Pass: 5 pages; no missing local targets, duplicate IDs, missing image alternatives, or unsafe `_blank` links | 2026-09-18 |
| Local HTTP preview | `Invoke-WebRequest` for five pages and `assets/style.css` | Pass: all six resources returned HTTP 200 with non-empty content | 2026-09-18 |
| Diff integrity | `git diff --check` | Pass: no whitespace errors | 2026-09-18 |
| Confidential-content guard | Repository search for internal names, systems, architecture, and unpublished metrics | Pass: no matches in published HTML | 2026-09-18 |
| Azure infrastructure and RBAC | Static review | Not applicable: no Azure resources, identities, or role assignments | 2026-09-18 |

**Validated by:** azure-validate

## 9. Files to Modify

| File | Purpose |
|------|---------|
| `.azure/deployment-plan.md` | Track approved scope and completion |
| `assets/style.css` | Shared visual system and responsive layouts |
| `index.html` | Homepage |
| `projects.html` | Project portfolio |
| `resume.html` | Resume |
| `scd-diary.html` | Flagship project case study |
| `ethics-scd.html` | Ethics capstone |

## 10. Next Step

Review the local browser preview. Publishing to GitHub Pages is intentionally deferred until explicitly requested.
