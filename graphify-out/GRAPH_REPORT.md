# Graph Report - .  (2026-05-14)

## Corpus Check
- Corpus is ~7,776 words - fits in a single context window. You may not need a graph.

## Summary
- 65 nodes · 105 edges · 10 communities (7 shown, 3 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 5 edges (avg confidence: 0.93)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_App Shell and Theme Toggle|App Shell and Theme Toggle]]
- [[_COMMUNITY_Project Docs and Concepts|Project Docs and Concepts]]
- [[_COMMUNITY_Content Sections and Utilities|Content Sections and Utilities]]
- [[_COMMUNITY_Hero and About|Hero and About]]
- [[_COMMUNITY_Skills and Type Definitions|Skills and Type Definitions]]
- [[_COMMUNITY_Accent Color State|Accent Color State]]
- [[_COMMUNITY_Education Section|Education Section]]

## God Nodes (most connected - your core abstractions)
1. `README.md — Portfolio project documentation` - 8 edges
2. `formatText()` - 5 edges
3. `ProfileData` - 4 edges
4. `RootState` - 4 edges
5. `index.html — Portfolio entry point` - 4 edges
6. `React 19 + TypeScript + Vite tech stack` - 4 edges
7. `Experience()` - 3 edges
8. `Projects()` - 3 edges
9. `Red-accent favicon set for portfolio — Hanuman font, icon-red directory` - 3 edges
10. `ThemeState` - 2 edges

## Surprising Connections (you probably didn't know these)
- `Vite logo SVG — official Vite brand icon, purple-to-cyan gradient chevron with amber flame` --conceptually_related_to--> `React 19 + TypeScript + Vite tech stack`  [INFERRED]
  public/vite.svg → README.md
- `React logo SVG — official React brand icon, cyan atomic orbit design` --conceptually_related_to--> `React 19 + TypeScript + Vite tech stack`  [INFERRED]
  src/assets/react.svg → README.md
- `index.html — Portfolio entry point` --conceptually_related_to--> `README.md — Portfolio project documentation`  [INFERRED]
  index.html → README.md
- `Red-accent favicon set for portfolio — Hanuman font, icon-red directory` --conceptually_related_to--> `Yellow-accent favicon set for portfolio — icon-yellow directory`  [INFERRED]
  public/icon-red/about.txt → index.html
- `index.html — Portfolio entry point` --references--> `React 19 + TypeScript + Vite tech stack`  [EXTRACTED]
  index.html → README.md

## Communities (10 total, 3 thin omitted)

### Community 0 - "App Shell and Theme Toggle"
Cohesion: 0.19
Nodes (6): AppDispatch, RootState, store, initialState, themeSlice, ThemeState

### Community 1 - "Project Docs and Concepts"
Cohesion: 0.15
Nodes (15): React logo SVG — official React brand icon, cyan atomic orbit design, Dark/light mode theme system with system preference detection, Red-accent favicon set for portfolio — Hanuman font, icon-red directory, GitHub Pages deployment strategy, Google-inspired section accent color system, Yellow-accent favicon set for portfolio — icon-yellow directory, JSON files as data source instead of CMS, Open Graph and Twitter card social sharing metadata (+7 more)

### Community 2 - "Content Sections and Utilities"
Cohesion: 0.24
Nodes (9): ExpCard(), Experience(), useWindowHeight(), useWindowWidth(), Projects(), toAbsolute(), Experience, Project (+1 more)

### Community 5 - "Accent Color State"
Cohesion: 0.5
Nodes (3): accentSlice, initialState, AccentState

## Knowledge Gaps
- **14 isolated node(s):** `initialState`, `accentSlice`, `initialState`, `themeSlice`, `AppDispatch` (+9 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What connects `initialState`, `accentSlice`, `initialState` to the rest of the system?**
  _14 weakly-connected nodes found - possible documentation gaps or missing edges._