# Graph Report - Portfolio  (2026-06-23)

## Corpus Check
- 29 files · ~9,086 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 115 nodes · 147 edges · 14 communities
- Extraction: 99% EXTRACTED · 1% INFERRED · 0% AMBIGUOUS · INFERRED: 1 edges (avg confidence: 0.95)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `7fb3ecce`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Design System + Deployment|Design System + Deployment]]
- [[_COMMUNITY_Projects + Experience UI|Projects + Experience UI]]
- [[_COMMUNITY_Hero, About, Contact|Hero, About, Contact]]
- [[_COMMUNITY_Navbar + Redux Store|Navbar + Redux Store]]
- [[_COMMUNITY_Skills + Certifications|Skills + Certifications]]
- [[_COMMUNITY_App Entry + Composition|App Entry + Composition]]
- [[_COMMUNITY_Accent + Type Definitions|Accent + Type Definitions]]
- [[_COMMUNITY_ESLint Config|ESLint Config]]

## God Nodes (most connected - your core abstractions)
1. `Portfolio Website` - 12 edges
2. `scripts` - 7 edges
3. `formatText()` - 5 edges
4. `ProfileData` - 4 edges
5. `RootState` - 4 edges
6. `Local Development` - 3 edges
7. `Experience()` - 3 edges
8. `Projects()` - 3 edges
9. `Red-accent favicon set for portfolio — Hanuman font, icon-red directory` - 3 edges
10. `pnpm` - 2 edges

## Surprising Connections (you probably didn't know these)
- `Red-accent favicon set for portfolio — Hanuman font, icon-red directory` --conceptually_related_to--> `Yellow-accent favicon set for portfolio — icon-yellow directory`  [INFERRED]
  public/icon-red/about.txt → index.html
- `index.html — Portfolio entry point` --references--> `Red-accent favicon set for portfolio — Hanuman font, icon-red directory`  [EXTRACTED]
  index.html → public/icon-red/about.txt
- `ExpCard()` --calls--> `formatText()`  [EXTRACTED]
  src/components/Experience/Experience.tsx → src/utils/formatText.tsx
- `Projects()` --calls--> `formatText()`  [EXTRACTED]
  src/components/Projects/Projects.tsx → src/utils/formatText.tsx

## Import Cycles
- None detected.

## Communities (14 total, 0 thin omitted)

### Community 0 - "Design System + Deployment"
Cohesion: 0.21
Nodes (6): AppDispatch, RootState, store, initialState, themeSlice, ThemeState

### Community 1 - "Projects + Experience UI"
Cohesion: 0.40
Nodes (5): Red-accent favicon set for portfolio — Hanuman font, icon-red directory, Yellow-accent favicon set for portfolio — icon-yellow directory, Open Graph and Twitter card social sharing metadata, icon-red favicon set — Hanuman font, red accent, favicon generation metadata, index.html — Portfolio entry point

### Community 2 - "Hero, About, Contact"
Cohesion: 0.24
Nodes (9): ExpCard(), Experience(), useWindowHeight(), useWindowWidth(), Projects(), toAbsolute(), Experience, Project (+1 more)

### Community 3 - "Navbar + Redux Store"
Cohesion: 0.18
Nodes (7): accentSlice, initialState, AccentState, Certification, Education, ProfileData, Skill

### Community 4 - "Skills + Certifications"
Cohesion: 0.12
Nodes (15): homepage, name, packageManager, pnpm, onlyBuiltDependencies, private, scripts, build (+7 more)

### Community 5 - "App Entry + Composition"
Cohesion: 0.13
Nodes (15): devDependencies, baseline-browser-mapping, eslint, @eslint/js, eslint-plugin-react-hooks, eslint-plugin-react-refresh, gh-pages, globals (+7 more)

### Community 6 - "Accent + Type Definitions"
Cohesion: 0.20
Nodes (10): dependencies, lucide-react, react, react-dom, react-redux, redux, @reduxjs/toolkit, sass (+2 more)

### Community 10 - "ESLint Config"
Cohesion: 0.12
Nodes (15): Changelog, code:bash (pnpm install), code:bash (pnpm build      # production build → dist/), code:block3 (src/), Deployment, Features, Local Development, Portfolio Website (+7 more)

## Knowledge Gaps
- **56 isolated node(s):** `name`, `private`, `version`, `type`, `packageManager` (+51 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `devDependencies` connect `App Entry + Composition` to `Skills + Certifications`?**
  _High betweenness centrality (0.071) - this node is a cross-community bridge._
- **Why does `dependencies` connect `Accent + Type Definitions` to `Skills + Certifications`?**
  _High betweenness centrality (0.049) - this node is a cross-community bridge._
- **What connects `name`, `private`, `version` to the rest of the system?**
  _56 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Skills + Certifications` be split into smaller, more focused modules?**
  _Cohesion score 0.125 - nodes in this community are weakly interconnected._
- **Should `App Entry + Composition` be split into smaller, more focused modules?**
  _Cohesion score 0.13333333333333333 - nodes in this community are weakly interconnected._
- **Should `ESLint Config` be split into smaller, more focused modules?**
  _Cohesion score 0.125 - nodes in this community are weakly interconnected._