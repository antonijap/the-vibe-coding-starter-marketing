# The Vibe-Coding Starter Marketing Site

A high-converting, single-page landing website for **The Vibe-Coding Starter Kit** - a premium product designed for non-technical founders and side-project enthusiasts who use AI to generate code.

## 🎯 Purpose

This landing page focuses on two primary value propositions:
1. **Instant launch speed** (under 5 minutes)
2. **Guaranteed designer-grade aesthetic** (saving AI tokens)

## 🛠️ Tech Stack

- **Framework:** [SvelteKit](https://kit.svelte.dev/) with Svelte 5
- **Build Tool:** [Vite](https://vitejs.dev/)
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/)
- **Animation:** [Motion](https://motion.dev/) (v11)
- **Language:** TypeScript/JavaScript (ES modules)
- **Deployment:** [Vercel](https://vercel.com/) with `@sveltejs/adapter-vercel`

## 🚀 Getting Started

### Prerequisites

- Node.js 20.x (specified in `.nvmrc`)
- npm or yarn

### Installation

```bash
# Install dependencies
npm install
```

### Development

```bash
# Start development server
npm run dev
```

The site will be available at `http://localhost:5173`

### Build

```bash
# Build for production
npm run build

# Preview production build locally
npm run preview
```

## 📁 Project Structure

```
src/
├── lib/
│   ├── components/     # Reusable Svelte components
│   │   ├── Hero.svelte
│   │   ├── Comparison.svelte
│   │   ├── ValuePillars.svelte
│   │   ├── FinalCTA.svelte
│   │   └── ...
│   └── constants.ts    # App constants
├── routes/
│   ├── +layout.svelte  # Root layout
│   └── +page.svelte     # Home page
└── app.css             # Global styles
```

## 🎨 Design Principles

- **Minimal & Clean:** Ample white space and clean typography
- **Light Theme Only:** White backgrounds with neutral colors
- **Accent Color:** Orange (`bg-orange-600`) for primary elements
- **Typography:** Inter font family
- **Motion:** Subtle animations for a polished feel

## 🚢 Deployment

This project is configured for automatic deployment on Vercel:

- **Production URL:** [View Live Site](https://the-vibe-coding-starter-marketing-23vp1kz50-antonija.vercel.app)
- **Repository:** [GitHub](https://github.com/antonijap/the-vibe-coding-starter-marketing)

### Manual Deployment

```bash
# Deploy to Vercel
vercel --prod
```

## 📝 License

Private project - All rights reserved

