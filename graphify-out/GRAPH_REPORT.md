# Graph Report - .  (2026-05-15)

## Corpus Check
- 14 files · ~7,797 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 63 nodes · 120 edges · 12 communities (9 shown, 3 thin omitted)
- Extraction: 92% EXTRACTED · 8% INFERRED · 0% AMBIGUOUS · INFERRED: 9 edges (avg confidence: 0.87)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Design System + Deployment|Design System + Deployment]]
- [[_COMMUNITY_Projects + Experience UI|Projects + Experience UI]]
- [[_COMMUNITY_Hero, About, Contact|Hero, About, Contact]]
- [[_COMMUNITY_Navbar + Redux Store|Navbar + Redux Store]]
- [[_COMMUNITY_Skills + Certifications|Skills + Certifications]]
- [[_COMMUNITY_App Entry + Composition|App Entry + Composition]]
- [[_COMMUNITY_Accent + Type Definitions|Accent + Type Definitions]]
- [[_COMMUNITY_Particle Background|Particle Background]]
- [[_COMMUNITY_Scroll + Nav Behavior|Scroll + Nav Behavior]]
- [[_COMMUNITY_Theme Redux Slice|Theme Redux Slice]]

## God Nodes (most connected - your core abstractions)
1. `AppContent()` - 13 edges
2. `Experience` - 9 edges
3. `README.md — Portfolio project documentation` - 8 edges
4. `ProfileData` - 7 edges
5. `Project` - 7 edges
6. `RootState` - 6 edges
7. `ParticleWave()` - 6 edges
8. `Skills()` - 5 edges
9. `ThemeState` - 4 edges
10. `Education` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Vite logo SVG — official Vite brand icon, purple-to-cyan gradient chevron with amber flame` --conceptually_related_to--> `React 19 + TypeScript + Vite tech stack`  [INFERRED]
  public/vite.svg → README.md
- `React logo SVG — official React brand icon, cyan atomic orbit design` --conceptually_related_to--> `React 19 + TypeScript + Vite tech stack`  [INFERRED]
  src/assets/react.svg → README.md
- `themeUniforms()` --shares_data_with--> `ThemeState`  [INFERRED]
  components/Background/ParticleWave.tsx → src/types/index.ts
- `AppContent()` --calls--> `ParticleWave()`  [EXTRACTED]
  src/App.tsx → components/Background/ParticleWave.tsx
- `ParticleWave()` --references--> `RootState`  [EXTRACTED]
  components/Background/ParticleWave.tsx → src/store/store.ts

## Hyperedges (group relationships)
- **Components Consuming ProfileData** — hero_hero_hero, about_about_about, contact_contact_contact, types_index_profiledata [EXTRACTED 1.00]
- **Theme Redux State Pipeline** — store_store_store, store_store_rootstate, src_app_appcontent, background_particlewave_particlewave [EXTRACTED 1.00]
- **Section Layout Pattern (Section + Container + Title)** — hero_hero_hero, about_about_about, education_education_education, experience_experience_experience, projects_projects_projects, skills_skills_skills, contact_contact_contact [INFERRED 0.95]

## Communities (12 total, 3 thin omitted)

### Community 0 - "Design System + Deployment"
Cohesion: 0.15
Nodes (15): React logo SVG — official React brand icon, cyan atomic orbit design, Dark/light mode theme system with system preference detection, Red-accent favicon set for portfolio — Hanuman font, icon-red directory, GitHub Pages deployment strategy, Google-inspired section accent color system, Yellow-accent favicon set for portfolio — icon-yellow directory, JSON files as data source instead of CMS, Open Graph and Twitter card social sharing metadata (+7 more)

### Community 1 - "Projects + Experience UI"
Cohesion: 0.25
Nodes (7): Project Detail Modal Pattern, Windowed Card Display with Timeline Nav, ExpCard(), toAbsolute(), truncate(), Experience, Project

### Community 2 - "Hero, About, Contact"
Cohesion: 0.43
Nodes (4): About(), Contact(), Hero(), ProfileData

### Community 3 - "Navbar + Redux Store"
Cohesion: 0.53
Nodes (4): AppDispatch, RootState, store, ThemeToggle()

### Community 4 - "Skills + Certifications"
Cohesion: 0.6
Nodes (4): Certifications Remainder-Based Grid Spanning, Skills(), Certification, Skill

### Community 7 - "Particle Background"
Cohesion: 0.67
Nodes (3): ParticleWave(), themeUniforms(), Theme-Aware Three.js Background

### Community 8 - "Scroll + Nav Behavior"
Cohesion: 0.67
Nodes (3): Scroll-Based Active Section Tracking, Navbar(), scrollToSection Function

## Knowledge Gaps
- **14 isolated node(s):** `AppDispatch`, `icon-red favicon set — Hanuman font, red accent, favicon generation metadata`, `Vite logo SVG — official Vite brand icon, purple-to-cyan gradient chevron with amber flame`, `React logo SVG — official React brand icon, cyan atomic orbit design`, `GitHub Pages deployment strategy` (+9 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `AppContent()` connect `App Entry + Composition` to `Projects + Experience UI`, `Hero, About, Contact`, `Navbar + Redux Store`, `Skills + Certifications`, `Accent + Type Definitions`, `Particle Background`, `Scroll + Nav Behavior`, `Theme Redux Slice`?**
  _High betweenness centrality (0.144) - this node is a cross-community bridge._
- **Why does `Experience` connect `Projects + Experience UI` to `App Entry + Composition`, `Accent + Type Definitions`?**
  _High betweenness centrality (0.100) - this node is a cross-community bridge._
- **Why does `Project` connect `Projects + Experience UI` to `App Entry + Composition`, `Accent + Type Definitions`?**
  _High betweenness centrality (0.050) - this node is a cross-community bridge._
- **What connects `AppDispatch`, `icon-red favicon set — Hanuman font, red accent, favicon generation metadata`, `Vite logo SVG — official Vite brand icon, purple-to-cyan gradient chevron with amber flame` to the rest of the system?**
  _14 weakly-connected nodes found - possible documentation gaps or missing edges._