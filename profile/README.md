<p align="center">
  <img src="../logo.png" alt="Kivora" width="64" />
</p>

<h1 align="center">Kivora</h1>

<p align="center">
  A multi-framework UI component library designed for consistency, accessibility, and developer experience.
</p>

<p align="center">
  <a href="https://github.com/kivora-ui/react"><img src="https://img.shields.io/badge/React-available-blue?logo=react" alt="React" /></a>
  <a href="https://github.com/kivora-ui/react-native"><img src="https://img.shields.io/badge/React_Native-coming_soon-lightgrey?logo=react" alt="React Native" /></a>
  <a href="https://github.com/kivora-ui/solid"><img src="https://img.shields.io/badge/Solid.js-coming_soon-lightgrey?logo=solid" alt="Solid.js" /></a>
  <a href="https://github.com/kivora-ui"><img src="https://img.shields.io/badge/GitHub-kivora--ui-181717?logo=github" alt="GitHub" /></a>
</p>

---

## What is Kivora?

Kivora is a **multi-framework design system** built from the ground up to provide a consistent set of UI primitives across different JavaScript frameworks. Whether you're building a web app with React, a mobile app with React Native, or a site with Solid.js — Kivora aims to give you the same tokens, patterns, and components.

The core design tokens (colors, sizes, variants) live in a shared `@kivora/core` package, which every framework adapter consumes. This ensures visual consistency regardless of the framework you choose.

> **Current status:** The React package is fully implemented. React Native and Solid.js support is planned for future releases.

---

## Monorepo Structure

This repository is a [pnpm](https://pnpm.io) workspace managed with [Turborepo](https://turbo.build).

```
kivora/
├── apps/
│   └── web/                  # Documentation & showcase site (Next.js)
└── packages/
    ├── core/                 # Shared tokens, types, and utilities
    ├── react/                # @kivora/react  ✅ Available
    ├── react-native/         # @kivora/react-native  🚧 Coming soon
    └── solid/                # @kivora/solid  🚧 Coming soon
```

---

## Packages

### `@kivora/react` — [GitHub](https://github.com/kivora-ui/react) · ✅ Available

Full-featured React component library with TypeScript support, built for web applications.

**Components**

| Category | Components |
|---|---|
| Buttons | `Button`, `ActionIcon` |
| Inputs | `Input`, `Checkbox`, `RadioGroup`, `Switch` |
| Typography | `Text` |
| Feedback | `Spinner`, `Toaster` |
| Navigation | `Tabs` |
| Overlays | `Modal`, `Tooltip` |
| Data Display | `Badge`, `Avatar`, `Tag`, `Card`, `Accordion` |
| Misc | `Divider`, `Icon` |

**Hooks**

Utility hooks organized by category: `async`, `browser`, `dom`, `focus`, `persistence`, `state`, `ui`, and `utils`.

**Install**

```bash
npm install @kivora/react
# or
pnpm add @kivora/react
```

---

### `@kivora/react-native` — [GitHub](https://github.com/kivora-ui/react-native) · 🚧 Coming soon

Mobile-first component library for React Native and Expo, sharing the same design tokens as `@kivora/react`.

---

### `@kivora/solid` — [GitHub](https://github.com/kivora-ui/solid) · 🚧 Coming soon

Component library for [Solid.js](https://www.solidjs.com), using the same `@kivora/core` foundations.

---

### `@kivora/core` — Internal

Shared package that provides design tokens, type definitions, and base utilities. Consumed internally by all framework adapters and not meant to be installed directly by end users.

---

## Development

### Prerequisites

- [Node.js](https://nodejs.org) 18+
- [pnpm](https://pnpm.io) 9+

### Setup

```bash
# Clone the repository
git clone https://github.com/kivora-ui/react
cd kivora

# Install dependencies
pnpm install

# Build all packages
pnpm build

# Start the docs site
pnpm --filter web dev

# Run tests (React package)
pnpm --filter @kivora/react test
```

### Useful Commands

| Command | Description |
|---|---|
| `pnpm build` | Build all packages |
| `pnpm dev` | Start all packages in watch mode |
| `pnpm type-check` | Type-check all packages |
| `pnpm --filter @kivora/react test` | Run React package tests |
| `pnpm --filter web dev` | Start the docs site locally |

---

## Versioning & Releases

This project uses [Changesets](https://github.com/changesets/changesets) for versioning. See [RELEASING.md](./RELEASING.md) for the full release workflow.

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request on the relevant repository:

- React: [github.com/kivora-ui/react](https://github.com/kivora-ui/react)
- React Native: [github.com/kivora-ui/react-native](https://github.com/kivora-ui/react-native)
- Solid: [github.com/kivora-ui/solid](https://github.com/kivora-ui/solid)
- Organization: [github.com/kivora-ui](https://github.com/kivora-ui)

---

## License

MIT © Kivora
