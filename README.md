# Vket Boilerplate Nuxt

[![japanese](https://badgen.net/badge/README/in%20日本語/red?icon=github)](./README.ja.md) [![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/PublicHIKKY/vket-boilerplate-nuxt)


This is a production-ready Nuxt4 boilerplate published by HIKKY Ltd., designed for building scalable VR/metaverse web applications.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](/LICENSE)
[![Nuxt](https://img.shields.io/badge/Nuxt-4.0+-00DC82?logo=nuxt.js)](https://nuxt.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9+-3178C6?logo=typescript)](https://www.typescriptlang.org/)
[![Bun](https://img.shields.io/badge/Bun-1.0+-000000?logo=bun)](https://bun.sh/)

## 🤖 For AI Agents

**Before starting development, please read [`AGENTS.md`](./AGENTS.md) for comprehensive development guidelines, coding standards, and project-specific instructions.**

The `AGENTS.md` file contains:
- Project structure and Layer Architecture guidelines
- Component naming conventions (Ha/Hm/Ho/Ht prefixes)  
- TypeScript strict mode requirements
- Testing and quality assurance procedures
- i18n implementation patterns

## ✨ Features

- **🏗️ Nuxt Layer Architecture**: Modular monorepo structure with base/main/showcases layers
- **⚡ Bun Workspaces**: Fast package management and monorepo support
- **🔒 TypeScript Strict Mode**: Zero-tolerance for `any` types, full type safety
- **🎨 Component System**: Atomic design with Ha/Hm/Ho/Ht prefixes
- **🌍 Internationalization**: Built-in i18n support with YAML-based translations
- **📏 Zod Validation**: Schema-first API validation and type inference
- **🎯 RSCSS/BEM**: Structured CSS naming conventions
- **🧪 Testing Ready**: Vitest + Testing Library setup with coverage
- **📦 Auto-imports**: Components, composables, and utilities
- **🛠️ Quality Tools**: ESLint, Stylelint, Husky, lint-staged

## 🚀 Quick Start

### Prerequisites
- [Bun](https://bun.sh/docs/installation) (recommended) or Node.js 22+
- Git

### Installation

1. **Fork this repository**
   ```bash
   # Click "Fork" on GitHub or use GitHub CLI
   gh repo fork hikky-inc/vket-boilerplate-nuxt
   ```

2. **Clone and setup**
   ```bash
   git clone https://github.com/YOUR_USERNAME/vket-boilerplate-nuxt.git
   cd vket-boilerplate-nuxt
   bun install
   ```

3. **Start development**
   ```bash
   # Navigate to main layer (your application)
   cd layers/main
   
   # Start development server
   bun dev
   ```

4. **You're ready!** 🎉
   - Open http://localhost:3000
   - Start building your application with zero configuration

## 📁 Project Structure

```
/layers/
├── base/        # 🏗️ Foundation layer - shared components, utilities
├── main/        # 🎯 Your application - main development area
├── showcases/   # 📚 Component documentation and examples
└── open-api/    # 🔌 API schema definitions
```

### Layer Hierarchy
- **Base Layer**: Reusable components (Ha*, Hm*), utilities, styles
- **Main Layer**: Your application logic, pages, specific components (Ho*, Ht*)
- **Showcases Layer**: Living documentation and component examples




## 🔗 Useful Links

- [HIKKY Ltd.](https://www.hikky.co.jp/) - Company website
- [VRChat](https://hello.vrchat.com/) - VR platform
- [Virtual Market](https://vket.com/) - Virtual event platform

## 📄 License

MIT License - see the [LICENSE](LICENSE) file for details.

