# Foundations
The invisible layer behind every great product — tokens, rules, and systems that bridge design and code, 100% free and open-source.

---


### What is Desnify Foundations?

Desnify Foundations is the core design language powering Desnify Elements — a unified set of design tokens, variables, and styles built for scale. It serves as the single source of truth between design and code, ensuring every decision made in Figma translates consistently and accurately into production.

Great products aren't just built with great components — they're built on solid foundations. Consistent spacing, a structured color system, a clear type scale, and a token architecture that scales with your product. That's exactly what Desnify Foundations gives you... whether you're a designer working in Figma or a developer building in code, everything you need to move fast and design with consistency is already here — free and open-source, for everyone.


---


### What’s inside?

A multi-layered token system and practical guidelines that bring structure, clarity, and flexibility together:

🧱 Primitives & Semantic Tokens — The dual-layer token structure is the backbone that connects design and code. Every foundational element follows a clear two-tier system: Primitives define the raw core values, while Semantics give those values meaning and purpose within real use cases.

🎨 Color System — A balanced, accessible color palette designed for clarity and contrast across light and dark modes. It brings consistency to every surface, state, and theme across products.

✍️ Typography — A structured, scalable type system covering display, heading, label, and body styles. Built to adapt across platforms while maintaining legibility and rhythm.

📐 Spacing, Size & Radius — Numeric, predictable scales built for responsive interfaces. Spacing defines consistent padding and margins, size unifies component dimensions, and radius ensures soft, balanced corners that bring visual harmony throughout.

🧭 Layout Grids — Flexible grids and breakpoints that help maintain visual order across screens, ensuring alignment, rhythm, and structure for pages, cards, and components.

🧩 Icons & Assets — 1,500+ icons from [Iconoir.com](https://iconoir.com/) along with a well-curated library of design assets that empowers you to build faster without searching elsewhere.

⚡ Interaction & Motion — A unified interaction framework defining animation types, curves, and durations. Covers core patterns like hover, press, dialog, sheet, snackbar, and page transitions. Adds life to interactions without overwhelming the experience.

Each layer is crafted to reduce complexity, improve consistency, and make scaling across platforms effortless.


---

### Token architecture

Desnify Foundations follows a two-tier token system:

**Primitive tokens**   →   Raw values (e.g. `spacing-12`, `color-purple-500`) 

**Semantic tokens**    →   Meaningful, usage-based aliases (e.g. `--ds-spacing-12`, `--ds-color-fg-brand-primary`)

Primitives are the raw building blocks — colors, spacing values, font sizes — with no context attached. Semantic tokens reference those primitives and add meaning based on how they're actually used (`--ds-color-fg-brand-primary`, not `purple-600`), which is what you'll see and use day to day across Web, iOS, and Android.

This structure means a single primitive change cascades through every semantic token built on top of it — keeping the entire system consistent with one source of truth.


---

### Platform support

One source of truth, built out into ready-to-use formats for every platform:


| Platform | Format | Status |
|---|---|---|
| Web | CSS custom properties | ✅ Shipped |
| iOS | Swift | ✅ Shipped |
| Android | XML / Jetpack Compose-ready | ✅ Shipped |


---


### Getting started with Foundations?

Desnify Foundations is available both as a Figma Community file and as an installable npm package — pick whichever fits your workflow, or use both together to keep design and code in sync.

**For designers — Figma**
Explore the full token system directly in Figma — colors, typography, spacing, border, and corner radius — and start building your design system today. The Figma file mirrors the exact same tokens shipped in the npm package, so anything you see in Figma maps 1:1 to what developers consume in code.

[→ Get Desnify Foundations on Figma Community](https://www.figma.com/community/file/1560015998969232882)

**For developers — npm**
Install the package and bring Desnify's tokens straight into your code. A single source of truth, built out into ready-to-use formats for Web, iOS, and Android.

```bash
npm install @desnify/foundations
```

**Web** — import the CSS file into your project:

```css
@import '@desnify/foundations/dist/web/tokens.css';
```

**iOS** — drop `DesignTokens.swift` from `node_modules/@desnify/foundations/dist/ios/` into your Xcode project, then the `DS` struct is available anywhere in your app:

```swift
import DesignTokens
```

**Android** — copy `tokens.xml` and `tokens-night.xml` from `node_modules/@desnify/foundations/dist/android/` into your project's `res/values/` and `res/values-night/` folders respectively. No import needed — Android automatically picks up resources placed in `res/`.

*Please note: All tokens follow a consistent naming convention and namespace `ds` (standing for Desnify System) across platforms — `--ds-` for CSS, `ds_` for Android, and `DS.` for Swift — so once you learn one, you instantly understand the others.*

**Exploring the source**

- Raw token files (JSON) live in [`/tokens`](./tokens)
- Platform-specific builds live in [`/dist`](./dist) — `dist/web`, `dist/ios`, `dist/android`
- The build pipeline is powered by [Style Dictionary](https://styledictionary.com/), transforming one source of truth into every platform automatically

⭐ If you find this useful, consider starring the repo — it helps more designers and developers discover Desnify, and lets you know the moment new releases drop.


---

### Roadmap

- [x] Figma Community release
- [x] Token directory (.JSON) 
- [x] Figma Design & Github Sync 
- [x] Cross-platform support - Web, Android, and iOS
- [x] npm package (npm install @desnify/foundations)
- [ ] AI-native context (.claude / .cursor support)


---


### Related

[Desnify Elements](https://desnify.com/) — Everything you need to build and maintain your UI in one place, a rich library of customizable components built on top Desnify Foundations.


---

## License

MIT © 2024–2026 [Desnify.com](https://desnify.com)

Desnify Foundations is free and open-source. You're free to use, modify, and distribute it — even commercially. The only requirement is that you keep the copyright notice.

Built and maintained by [Pir Ahmed](https://www.linkedin.com/in/pirahmed/).






