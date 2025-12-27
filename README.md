# ssdhaliwal.dev

Portfolio website for Sarabjit Singh Dhaliwal - No-Code/Low-Code AI Developer.

Built with [Astro](https://astro.build), [Tailwind CSS](https://tailwindcss.com), and deployed on [Netlify](https://netlify.com).

## Features

- 🌍 **Multi-language**: English (EN) and German (DE)
- 🌓 **Dark Mode**: Native toggle with persistence
- 📱 **Fully Responsive**: Mobile-first design
- 🚀 **Fast**: Static site generation for optimal performance
- 📧 **Contact Forms**: Powered by Netlify Forms
- ♿ **Accessible**: WCAG AA compliant
- 🎨 **Modern Design**: Gradient accents and smooth animations

## Project Structure

```
ssdhaliwal/
├── public/           # Static assets
├── src/
│   ├── components/   # Reusable components
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Services.astro
│   │   ├── Portfolio.astro
│   │   └── Contact.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/        # English pages
│   │   ├── index.astro
│   │   ├── privacy.astro
│   │   └── success.astro
│   └── de/           # German pages
│       ├── index.astro
│       ├── impressum.astro
│       └── datenschutz.astro
├── docs/             # Documentation
├── astro.config.mjs
├── tailwind.config.mjs
└── netlify.toml
```

## Quick Start

### Prerequisites

- Node.js 20+ installed
- npm or yarn package manager

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

Visit `http://localhost:4321` to see the site.

## Deployment

### Netlify (Recommended)

1. Push to GitHub
2. Connect repository to Netlify
3. Build settings:
   - **Build command**: `npm run build`
   - **Publish directory**: `dist`
   - **Node version**: `20`

### Manual Deploy

```bash
npm run build
# Drag the /dist folder to Netlify drop
```

## Customization

### Update Personal Info

Edit these files:
- `src/components/Hero.astro` - Name, tagline, avatar
- `src/components/About.astro` - Your story and skills
- `src/components/Services.astro` - Your offerings and pricing
- `src/components/Portfolio.astro` - Your projects
- `src/de/impressum.astro` - Your address and legal info

### Add Your Avatar

Replace the placeholder in `src/components/Hero.astro`:

```astro
<!-- Replace this SVG with your image -->
<img src="/images/your-avatar.jpg" alt="Your Name" class="w-64 h-64 rounded-full" />
```

### Update Contact Email

Find and replace `freundly.apps@gmail.com` with your email throughout the project.

### Add Calendly Link

Update the Calendly URL in:
- `src/components/Hero.astro`
- `src/components/Contact.astro`

## Languages

### Add a New Language

1. Create `src/[lang]/` directory
2. Add `index.astro` with translations
3. Update `astro.config.mjs` i18n config
4. Add language switcher link in `Header.astro`

## Performance

Lighthouse Scores:
- Performance: 95+
- Accessibility: 95+
- Best Practices: 95+
- SEO: 95+

## License

© 2025 Sarabjit Singh Dhaliwal. All rights reserved.

## Credits

Built with ❤️ using [Astro](https://astro.build) + [Tailwind CSS](https://tailwindcss.com)
