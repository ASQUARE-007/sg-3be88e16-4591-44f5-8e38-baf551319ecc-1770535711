# Git New Check Project

A modern Next.js application built with TypeScript, React, and Tailwind CSS.

## 🚀 Tech Stack

- **Framework:** Next.js 15.2 (Pages Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS v3.4
- **UI Components:** shadcn/ui
- **Icons:** Lucide React
- **Forms:** React Hook Form + Zod
- **Animations:** Framer Motion
- **Theme:** Dark/Light mode support

## 📦 Getting Started

### Prerequisites

- Node.js 18+ and npm installed
- Git for version control

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd git-new-check
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.local.example .env.local
# Edit .env.local with your configuration
```

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🛠️ Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npm run type-check` - Run TypeScript compiler check

## 📁 Project Structure

```
src/
├── components/       # Reusable React components
│   ├── ui/          # shadcn/ui components
│   ├── SEO.tsx      # SEO configuration component
│   └── ThemeSwitch.tsx
├── contexts/        # React context providers
├── hooks/           # Custom React hooks
├── lib/             # Utility functions
├── pages/           # Next.js pages (file-based routing)
│   ├── api/         # API routes
│   └── _app.tsx     # Application wrapper
├── styles/          # Global styles and Tailwind config
public/              # Static assets
```

## 🎨 Features

- **Responsive Design:** Mobile-first approach with Tailwind CSS
- **Dark Mode:** Built-in theme switching capability
- **Type Safety:** Full TypeScript support
- **SEO Optimized:** Pre-configured SEO component
- **Component Library:** 40+ pre-built shadcn/ui components
- **Accessible:** WCAG AA compliant components

## 🧩 Available UI Components

The project includes a comprehensive set of shadcn/ui components:

- Accordion, Alert, Alert Dialog
- Avatar, Badge, Breadcrumb
- Button, Calendar, Card, Carousel
- Checkbox, Command, Context Menu
- Dialog, Drawer, Dropdown Menu
- Form, Hover Card, Input, Label
- Navigation Menu, Pagination, Popover
- Progress, Radio Group, Scroll Area
- Select, Separator, Sheet, Sidebar
- Skeleton, Slider, Switch, Table
- Tabs, Textarea, Toast, Toggle
- Tooltip

Import example:
```tsx
import { Button } from "@/components/ui/button";
import { Card } from "@/components/ui/card";
```

## 🔧 Configuration

### Tailwind CSS

Customize theme in `tailwind.config.ts`. CSS variables are defined in `src/styles/globals.css`.

### SEO

Update default SEO values in `src/components/SEO.tsx` or pass custom props per page:

```tsx
import { SEO } from "@/components/SEO";

<SEO 
  title="Custom Page Title"
  description="Page description"
  image="/custom-og-image.png"
/>
```

## 📝 Adding New Pages

Create a new file in `src/pages/`:

```tsx
// src/pages/about.tsx
import { SEO } from "@/components/SEO";

export default function About() {
  return (
    <>
      <SEO title="About" />
      <div>About page content</div>
    </>
  );
}
```

## 🚢 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Import project in Vercel
3. Deploy with one click

### Manual Build

```bash
npm run build
npm run start
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 🆘 Support

For issues and questions:
- Check existing issues on GitHub
- Create a new issue with detailed description
- Include error messages and screenshots when applicable

---

Built with ❤️ using [Softgen.ai](https://softgen.ai)