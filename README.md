# Next.js TypeScript Starter Template

<br/>
<p align="center">
  <img
    src="https://img.shields.io/npm/v/next-ts-app?style=for-the-badge&label=next-ts-app&labelColor=black&logo=npm&color=success"
    alt="next-ts-app version"
  />
  <img
    src="https://img.shields.io/static/v1?label=License&message=MIT&labelColor=000000&color=007ACC&style=for-the-badge&logo=open-source-initiative&logoColor=white"
    alt="License MIT"
  />
</p>

<p align="center">
<img src="https://img.shields.io/badge/Next.js-16.0.10-black?logo=next.js" alt="Nextjs">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwind-css&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/ESLint-4B32C3?logo=eslint&logoColor=white" alt="ESLint">
  <img src="https://img.shields.io/badge/Prettier-F7B93E?logo=prettier&logoColor=black" alt="Prettier">
</p>
<br/>

## 🚀 Why Use This Template?

This starter template is designed for **developers of all levels** — from beginners starting their journey to advanced engineers building scalable applications.

### Key Features

- ⚡️ **Next.js 16+** with App Router
- ✅ **TypeScript** – full type safety and custom config
- 🎨 **Tailwind CSS v4** – preconfigured and responsive
- 🧹 **ESLint + Prettier** – clean, consistent code
- 🌿 **Scalable folder structure** – production standard
- 📦 **Alias support** – easy path management
- 🧪 Ready for unit & integration testing
- ☁️ Vercel ready – just push and deploy

## How to Start

###  Create with CLI **`(Recommended)`**

Quickly set up your Next.js + TypeScript + TailwindCSS project using the CLI tool:

- **📦 using npm**
  ```bash
  npx next-ts-app my-awesome-app
  ```
- Replace my-awesome-app with your desired project name.
- The CLI will scaffold a fully configured Next.js + TypeScript + TailwindCSS starter for you.

### ✅ Fast | 🔧 Pre-configured | 🧪 Ready for development

---

#### CLI Options

During project creation, you'll be prompted to:

1. **Project Name**: What's your project name? (e.g., `my-awesome-app`)
2. **Package Manager**: Choose your preferred package manager:

   - `⚡ bun` (Recommended - Fastest)
   - `🚀 pnpm` (Fast & Efficient)
   - `🧶 yarn` (Reliable)
   - `📦 npm` (Standard)

   ```bash
   git clone https://github.com/[your-username]/[your-repo].git
   cd [your-repo]
   npm install
   pm run dev
   ```

## Project Structure

```
public/                      # Public static assets that are served directly
├── assets/                  # Static assets directory
│   ├── images/             # Image files (png, jpg, svg, etc.)
│   └── data/               # Static JSON data files
│
src/                        # Source code directory
├── app/                    # Next.js 13+ App Router directory
│   ├── (landing)/         # Landing page route group (optional)
│   │   ├── _components/    # Page-specific components
│   │   ├── error.tsx      # Error boundary for landing page
│   │   ├── loading.tsx    # Loading state for landing page
│   │   └── page.tsx       # Landing page entry point
│   │
│   ├── (dashboard)/       # Dashboard route group
│   │   ├── _components/    # Dashboard-specific components
│   │   ├── error.tsx      # Error boundary for dashboard
│   │   ├── loading.tsx    # Loading state for dashboard
│   │   └── page.tsx       # Dashboard page entry
│   │
│   ├── layout.tsx         # Root layout (shared across all pages)
│   ├── template.tsx       # Template for per-page layouts
│   └── providers.tsx      # Global context providers (Theme, Auth, etc.)
│
├── components/            # Reusable components directory
│   ├── ui/               # UI primitives (buttons, inputs, cards)
│   │   ├── button.tsx    # Button component
│   │   ├── input.tsx     # Input component
│   │   └── card.tsx      # Card component
│   │
│   ├── layout/           # Layout components
│   │   ├── header.tsx    # Header component
│   │   ├── footer.tsx    # Footer component
│   │   └── sidebar.tsx   # Sidebar component
│   │
│   ├── shared/           # Shared components across features
│   │   ├── ThemeToggle.tsx  # Theme toggle component
│   │   └── Analytics.tsx    # Analytics component
│   │
│   ├── forms/            # Form-related components
│   │   ├── FormInput.tsx    # Form input component
│   │   └── FormSelect.tsx   # Form select component
│   │
│   └── icons/            # SVG icon components
│       ├── index.tsx     # Icon exports
│       └── SocialIcons/  # Social media icons
│
├── config/               # Application configuration
│   ├── site.ts          # Site metadata and configuration
│   ├── routes.ts        # Route definitions and constants
│   └── theme.ts         # Theme configuration and tokens
│
├── hooks/               # Custom React hooks
│   ├── useAuth.ts       # Authentication hook
│   ├── useAnalytics.ts  # Analytics hook
│   ├── useDebounce.ts   # Debounce utility hook
│   └── useLocalStorage.ts # Local storage hook
│
├── lib/                 # Utility libraries and helpers
│   ├── api/            # API client configurations
│   │   ├── axios.ts    # Axios instance and interceptors
│   │   └── trpc/       # tRPC client setup
│   │
│   ├── utils/          # Utility functions
│   │   ├── formatter.ts # Data formatting utilities
│   │   └── validators.ts # Validation utilities
│   │
│   └── constants.ts    # Application constants
│
├── styles/             # Global styles and CSS
│   ├── globals.css     # Global CSS styles
│   ├── theme/          # Theme variables and tokens
│   └── components/     # Component-specific styles
│
├── types/              # TypeScript type definitions
│   ├── index.d.ts      # Global type declarations
│   ├── next.d.ts       # Next.js type extensions
│   └── custom-types.ts # Custom type definitions
│
├── services/           # Business logic and services
│   ├── auth.service.ts    # Authentication service
│   └── analytics.service.ts # Analytics service
│
├── contexts/           # React Context providers
│   ├── ThemeContext.tsx  # Theme context
│   └── AuthContext.tsx   # Authentication context
│
└── __tests__/         # Test files directory
    ├── components/     # Component tests
    ├── hooks/         # Hook tests
    ├── services/      # Service tests
    └── utils/         # Utility function tests
```

## Code Quality Tools

These tools keep your code neat:

- **ESLint**: Finds code mistakes.
- **Prettier**: Formats code nicely.
- **Tailwind CSS**: Organizes styles.

Example rule for imports:

```javascript
"import/order": [
  "error",
  {
    "groups": ["builtin", "external", "internal"],
    "alphabetize": { "order": "asc" }
  }
]
```

## Deployment

This template works with:

- Vercel
- Netlify
- AWS
- Docker

Copy `.env.example` to `.env` for production settings.

## Changelog

### v1.4.0 (Latest)

- **Major Update**: Upgraded to Next.js 16.0.10
- **React 19**: Full support for React 19 features
- **Tailwind CSS v4**: Using the latest Tailwind CSS version
- **TypeScript**: Updated to ES2022 target for better performance
- **ESLint**: Updated to latest Next.js 16 compatible version
- **Prettier**: Updated to v3.4.2
- **Performance**: Improved build times and runtime performance
- **Breaking Changes**:
  - Removed `next lint` command (use `eslint .` directly)
  - Node.js 20.9.0+ now required
- **Dependencies**: Added missing ESLint plugins (@typescript-eslint/eslint-plugin, @typescript-eslint/parser, eslint-plugin-import)
- **Configuration**: Improved .gitignore with IDE and OS entries

### v1.3.0

- **New Feature**: Interactive Husky selection during project creation
- **Template Branches**: Support for both `main` and `without-husky` branches
- **Enhanced CLI**: Better argument handling and help documentation
- **Improved UX**: Clear feedback about which template is being used
- **Better Progress**: Enhanced progress indicators and user feedback
- **Professional Prompts**: Beautiful emojis and improved messaging throughout
- **Default Behavior**: Husky disabled by default for simpler setup

### v1.2.40

- **Initial Release**: Basic CLI functionality
- **Package Manager Selection**: Support for bun, pnpm, yarn, npm
- **Beautiful UI**: Progress indicators and colorful output
- **Fast Setup**: Quick project initialization with degit


