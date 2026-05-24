# EduHub — O'qituvchilar uchun ta'lim platformasi

O'zbekistondagi o'qituvchilar uchun 1-sinfdan 11-sinfgacha barcha materiallar bir joyda.

## Tech Stack

- **Next.js 14** (App Router)
- **TypeScript**
- **Tailwind CSS**
- **shadcn/ui** components
- **Zustand** — state management
- **Lucide React** — icons

## Installation

### 1. Clone or download the project

```bash
git clone https://github.com/YOUR_USERNAME/eduhub.git
cd eduhub
```

### 2. Install dependencies

```bash
npm install
# or
yarn install
# or
pnpm install
```

### 3. Run development server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 4. Build for production

```bash
npm run build
npm start
```

---

## Project Structure

```
eduhub/
├── app/
│   ├── globals.css          # Global styles + Tailwind
│   ├── layout.tsx           # Root layout with LangProvider
│   └── page.tsx             # Main page
├── components/
│   ├── LangProvider.tsx     # Language context (O'z / Рус)
│   ├── layout/
│   │   ├── Navbar.tsx       # Sticky header with nav + language toggle
│   │   └── Footer.tsx       # Footer
│   ├── sections/
│   │   ├── Hero.tsx         # Hero banner
│   │   ├── StatsBar.tsx     # 4 stat cards
│   │   ├── ClassSelector.tsx # 1-11 sinf pills
│   │   ├── SubjectsGrid.tsx # 8 subject cards + content panel
│   │   ├── GamesSection.tsx # 6 educational games
│   │   └── FeaturesSection.tsx # Why EduHub?
│   └── ui/
│       └── ContentPanel.tsx # Tabs: Interaktiv / Darsliklar / Testlar
├── lib/
│   ├── data.ts              # All content data (uz + ru)
│   ├── store.ts             # Zustand store
│   └── utils.ts             # cn() helper
├── public/                  # Static assets
├── package.json
├── tailwind.config.ts
├── next.config.js
└── tsconfig.json
```

---

## GitHub Upload Instructions

### Option A — New repository

```bash
cd eduhub
git init
git add .
git commit -m "Initial commit: EduHub platform"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/eduhub.git
git push -u origin main
```

### Option B — GitHub Desktop

1. Open GitHub Desktop
2. File → Add Local Repository → select `eduhub` folder
3. Click "Publish repository"

### Option C — GitHub CLI

```bash
cd eduhub
gh repo create eduhub --public --source=. --push
```

---

## Deploying to Vercel (free)

```bash
npx vercel
```

Or connect your GitHub repo at [vercel.com](https://vercel.com) — it auto-deploys on every push.

---

## Features

- ✅ 1-sinf to 11-sinf class selector
- ✅ 8 subjects (Matematika, Fizika, Kimyo, etc.)
- ✅ Content panel with 3 tabs: Interaktiv darslar / Darsliklar / Testlar
- ✅ O'yinlar (Games) section with 6 educational games
- ✅ O'zbek / Rus language toggle
- ✅ Fully responsive (mobile + desktop)
- ✅ Clean green brand design
