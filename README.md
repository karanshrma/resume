# Karan Sharma — Developer Portfolio

Personal portfolio of **Karan Sharma**, a Flutter Developer building cross-platform mobile apps with Flutter, Dart, and modern backends.

**Live site:** [portfolio-eta-inky-11.vercel.app](https://portfolio-eta-inky-11.vercel.app)

## Features

- **Light & dark themes**: follows the visitor's browser / OS setting by default, with a toggle in the floating nav. A manual choice is remembered; picking the same theme as the browser goes back to following it.
- **Fully responsive**: tuned for small phones (320px), tablets, and large desktops.
- **Conversion-focused layout**: proof-first hero (live-app badge, primary/secondary CTAs) and a featured Snevva case card with store buttons ahead of open-source projects.
- **Animated UI**: GSAP ScrollTrigger horizontal project gallery, Framer Motion reveals, and a Three.js particle hero.
- **Neon ring cursor** (mouse/trackpad only) with interaction states: default, hover, link, text, grab/grabbing (drag the project gallery), resize, disabled, dragging, plus a click ripple. Touch screens keep the native behaviour with a tap ripple. Any element can opt into a state with `data-cursor="grab"` etc.
- **Downloadable CV**, plus contact links (email, phone, LinkedIn, GitHub) and a contact form that opens the visitor's email app.

## Highlights

### Experience

**Flutter Developer — Coretegra Technologies** (Nov 2025 – Present, Zirakpur)

Building **Snevva**, a health & wellness app with authentication, reminders, sleep tracking, step monitoring, mood analytics, and curated wellness content.

- [Get it on Google Play](https://play.google.com/store/apps/details?id=com.coretegra.snevvaa&pcampaignid=web_share)
- [Download on the App Store](https://apps.apple.com/in/app/snevva/id6783282525)

### Projects

| Project | Stack | Link |
| --- | --- | --- |
| ⭐ **Snevva** — Health & Wellness App (live, Coretegra) | Flutter, Dart, Kotlin, Background Services | [Google Play](https://play.google.com/store/apps/details?id=com.coretegra.snevvaa&pcampaignid=web_share) · [App Store](https://apps.apple.com/in/app/snevva/id6783282525) |
| E-Commerce App (Amazon Clone) | Flutter, Node.js, Express.js, MongoDB, Provider, GPay | [amazon_flutter_clone](https://github.com/karanshrma/amazon_flutter_clone) |
| AI Q&A App (Perplexity Clone) | Flutter, FastAPI, Python, Gemini API, RAG | [perplexity_clone](https://github.com/karanshrma/perplexity_clone) |
| Clean Architecture Blog App | Flutter, Bloc, Supabase, Hive, GetIt | [blog_app](https://github.com/karanshrma/blog_app) |

## Tech Stack

- [Vite](https://vitejs.dev/) + [React](https://react.dev/) + TypeScript
- [Tailwind CSS](https://tailwindcss.com/) + [shadcn/ui](https://ui.shadcn.com/)
- [next-themes](https://github.com/pacocoursey/next-themes) for light/dark mode
- [GSAP](https://gsap.com/) (ScrollTrigger) and [Framer Motion](https://www.framer.com/motion/) for animations
- [Three.js](https://threejs.org/) via React Three Fiber for the hero particles

## Getting Started

Requires Node.js 18+ and npm.

```sh
git clone https://github.com/karanshrma/portfolio.git
cd portfolio
npm install
npm run dev      # http://localhost:8080
```

### Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the dev server |
| `npm run build` | Production build to `dist/` |
| `npm run preview` | Preview the production build |
| `npm run lint` | Run ESLint |
| `npm test` | Run tests with Vitest |

## Project Structure

```
public/                 Static assets (favicons, resume PDF, Snevva screenshot)
src/
  components/           Page sections (Hero, Projects, About, Resume, Contact, Footer, FloatingNav)
  components/ui/        shadcn/ui primitives
  pages/                Route pages
  index.css             Light/dark theme tokens and custom styles
index.html              Meta tags and the pre-paint theme script
```

### Customising

- **Content**: each section lives in its own component under `src/components/`.
- **Colours**: edit the CSS variables in `src/index.css` (`:root` = light theme, `.dark` = dark theme).
- **CV**: replace `public/Karan_Sharma_Resume.pdf`.

## Deployment

The site is deployed on [Vercel](https://vercel.com/). Every push to `main` triggers a new production build (`npm run build`, output directory `dist`).

## Contact

- Email: [ks2275863@gmail.com](mailto:ks2275863@gmail.com)
- Phone: [+91 78142 52797](tel:+917814252797)
- LinkedIn: [linkedin.com/in/karanshrma](https://www.linkedin.com/in/karanshrma)
- GitHub: [github.com/karanshrma](https://github.com/karanshrma)
