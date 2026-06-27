# Graph Report - Portfolio  (2026-06-27)

## Corpus Check
- 34 files · ~12,225 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 202 nodes · 242 edges · 15 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 1 edges (avg confidence: 0.95)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `1ce073b1`
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
- [[_COMMUNITY_Particle Background|Particle Background]]
- [[_COMMUNITY_Scroll + Nav Behavior|Scroll + Nav Behavior]]
- [[_COMMUNITY_ESLint Config|ESLint Config]]
- [[_COMMUNITY_Community 11|Community 11]]

## God Nodes (most connected - your core abstractions)
1. `compilerOptions` - 21 edges
2. `compilerOptions` - 20 edges
3. `compilerOptions` - 19 edges
4. `Portfolio Website` - 13 edges
5. `scripts` - 9 edges
6. `formatText()` - 8 edges
7. `RootState` - 6 edges
8. `toAbsolute()` - 4 edges
9. `ProjectCard()` - 4 edges
10. `ProfileData` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Red-accent favicon set for portfolio — Hanuman font, icon-red directory` --conceptually_related_to--> `Yellow-accent favicon set for portfolio — icon-yellow directory`  [INFERRED]
  public/icon-red/about.txt → index.html
- `index.html — Portfolio entry point` --references--> `Red-accent favicon set for portfolio — Hanuman font, icon-red directory`  [EXTRACTED]
  index.html → public/icon-red/about.txt
- `ExpCard()` --calls--> `formatText()`  [EXTRACTED]
  src/components/Experience/Experience.tsx → src/utils/formatText.tsx
- `Wrap()` --calls--> `formatText()`  [EXTRACTED]
  src/test/formatText.test.tsx → src/utils/formatText.tsx
- `AppContent()` --calls--> `useDynamicFavicon()`  [EXTRACTED]
  src/App.tsx → src/hooks/useDynamicFavicon.ts

## Import Cycles
- None detected.

## Communities (15 total, 0 thin omitted)

### Community 0 - "Design System + Deployment"
Cohesion: 0.15
Nodes (10): ParticleWave(), THEME_COLORS, useDynamicFavicon(), AppContent(), AppDispatch, RootState, store, initialState (+2 more)

### Community 1 - "Projects + Experience UI"
Cohesion: 0.40
Nodes (5): Red-accent favicon set for portfolio — Hanuman font, icon-red directory, Yellow-accent favicon set for portfolio — icon-yellow directory, Open Graph and Twitter card social sharing metadata, icon-red favicon set — Hanuman font, red accent, favicon generation metadata, index.html — Portfolio entry point

### Community 2 - "Hero, About, Contact"
Cohesion: 0.20
Nodes (14): ExpCard(), Experience(), useWindowHeight(), useWindowWidth(), ProjectCard(), ProjectCardProps, ProjectModal(), ProjectModalProps (+6 more)

### Community 3 - "Navbar + Redux Store"
Cohesion: 0.16
Nodes (9): About(), Contact(), Skills(), AccentState, Certification, Education, Experience, ProfileData (+1 more)

### Community 4 - "Skills + Certifications"
Cohesion: 0.11
Nodes (17): homepage, name, packageManager, pnpm, onlyBuiltDependencies, private, scripts, build (+9 more)

### Community 5 - "App Entry + Composition"
Cohesion: 0.11
Nodes (19): devDependencies, baseline-browser-mapping, eslint, @eslint/js, eslint-plugin-react-hooks, eslint-plugin-react-refresh, gh-pages, globals (+11 more)

### Community 6 - "Accent + Type Definitions"
Cohesion: 0.20
Nodes (10): dependencies, lucide-react, react, react-dom, react-redux, redux, @reduxjs/toolkit, sass (+2 more)

### Community 7 - "Particle Background"
Cohesion: 0.08
Nodes (23): compilerOptions, allowImportingTsExtensions, erasableSyntaxOnly, jsx, lib, module, moduleDetection, moduleResolution (+15 more)

### Community 8 - "Scroll + Nav Behavior"
Cohesion: 0.09
Nodes (21): compilerOptions, allowImportingTsExtensions, erasableSyntaxOnly, jsx, lib, module, moduleDetection, moduleResolution (+13 more)

### Community 10 - "ESLint Config"
Cohesion: 0.12
Nodes (16): code:bash (pnpm install), code:bash (pnpm build      # production build → dist/), code:block3 (src/), Section Accent Colors, Accent Colors, Changelog, Deployment, Features (+8 more)

### Community 11 - "Community 11"
Cohesion: 0.09
Nodes (21): compilerOptions, allowImportingTsExtensions, erasableSyntaxOnly, lib, module, moduleDetection, moduleResolution, noEmit (+13 more)

## Knowledge Gaps
- **126 isolated node(s):** `name`, `private`, `version`, `type`, `packageManager` (+121 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `devDependencies` connect `App Entry + Composition` to `Skills + Certifications`?**
  _High betweenness centrality (0.033) - this node is a cross-community bridge._
- **Why does `dependencies` connect `Accent + Type Definitions` to `Skills + Certifications`?**
  _High betweenness centrality (0.018) - this node is a cross-community bridge._
- **What connects `name`, `private`, `version` to the rest of the system?**
  _126 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Design System + Deployment` be split into smaller, more focused modules?**
  _Cohesion score 0.14624505928853754 - nodes in this community are weakly interconnected._
- **Should `Skills + Certifications` be split into smaller, more focused modules?**
  _Cohesion score 0.1111111111111111 - nodes in this community are weakly interconnected._
- **Should `App Entry + Composition` be split into smaller, more focused modules?**
  _Cohesion score 0.10526315789473684 - nodes in this community are weakly interconnected._
- **Should `Particle Background` be split into smaller, more focused modules?**
  _Cohesion score 0.08333333333333333 - nodes in this community are weakly interconnected._