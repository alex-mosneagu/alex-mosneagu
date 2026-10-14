# Hi, I'm Alex — Frontend Tech Lead (JavaScript · Vue · Nuxt)

Frontend Tech Lead based in Bucharest, with 9+ years building and shipping production web and mobile applications. JavaScript is my primary language and the foundation of everything I build.

## About

I started out in 2016 as a freelance web developer, building websites, e-commerce stores and single-page apps for clients across Romania and abroad. In 2019 I founded **[Old Studio Concept](https://oldstudioconcept.ro)**, a product-focused agency where I led the delivery of SaaS platforms, e-commerce systems, education marketplaces and internal CRMs. That meant owning everything end to end: discovery, architecture, frontend and API development, deployment, and long-term maintenance.

Since January 2025 I have been **Technical Lead Frontend at HCLTech**. I lead frontend teams, make and document architecture decisions, set code-quality and testing standards, and work with product, design and backend teams so features ship predictably and the codebase stays maintainable.

What I care about most:

- **Code that outlives its authors.** Clear module boundaries, predictable state, and conventions a new team member can pick up in days.
- **Quality you can measure.** Automated tests, enforced linting, and CI pipelines that catch regressions before review.
- **Pragmatic architecture.** Choosing the simplest design that meets the product's real constraints, and recording why.
- **Teams that grow.** Code review as teaching, written standards, and room for engineers to own decisions.

## Core stack

| Area | Technologies |
|---|---|
| **Languages** | ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) |
| **Frameworks** | ![Vue.js](https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white) ![Nuxt](https://img.shields.io/badge/Nuxt-00DC82?style=flat-square&logo=nuxtdotjs&logoColor=white) ![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square&logo=pinia&logoColor=black) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) |
| **Styling** | ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) ![Sass](https://img.shields.io/badge/Sass-CC6699?style=flat-square&logo=sass&logoColor=white) |
| **Testing** | ![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white) ![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white) ![Cypress](https://img.shields.io/badge/Cypress-17202C?style=flat-square&logo=cypress&logoColor=white) ![Detox](https://img.shields.io/badge/Detox-20232A?style=flat-square&logo=react&logoColor=white) |
| **CI/CD & Tooling** | ![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) ![npm](https://img.shields.io/badge/npm-CB3837?style=flat-square&logo=npm&logoColor=white) ![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white) |

## Other stacks

Technologies I have used in production client and side projects:

| Area | Technologies |
|---|---|
| **Backend** | PHP, Laravel, Filament, Symfony (Twig), Go, Python, Express |
| **Data** | MySQL, MariaDB, Firebase |
| **Platforms** | WordPress, Shopify (custom apps), Chrome extensions |
| **Infrastructure** | Nginx, Apache, Cloudflare, Linux VPS deployments, cPanel |
| **Other** | TypeScript (basic), Raspberry Pi Pico (Python), Electron |

## What I do

| Area | In practice |
|---|---|
| **Frontend architecture** | Structuring Vue/Nuxt and React codebases into feature modules with clear ownership; choosing rendering strategy (SSR, SSG, SPA) per route; state design with Pinia; performance budgets and bundle analysis. |
| **Design systems** | Building reusable component libraries on Tailwind with shared tokens, accessible defaults and documented usage, so product teams move faster and the UI stays consistent. |
| **Test strategy** | A layered approach: fast unit tests (Vitest, Jest) for logic and components, Cypress for critical web flows, Detox for React Native, and clear rules for what each layer covers. |
| **CI/CD** | GitLab CI pipelines for linting, type checks, tests, preview environments and versioned releases; keeping pipelines fast enough that people don't skip them. |
| **Technical leadership** | Architecture decision records, code review standards, estimation and technical planning, working with backend and product on API contracts. |
| **Mentoring** | Onboarding engineers, pairing on hard problems, and turning review feedback into shared team conventions. |

## Featured projects

### [ActTrace](https://github.com/alex-mosneagu/ActTrace)

> Drop in one script. Understand every frontend interaction.

A zero-config browser library that intercepts **DOM events, network calls and DOM mutations** and correlates them into **one readable trace per user interaction**. You can see exactly what happens after a click, submit or keystroke, with no dashboard, no backend and no framework required.

- Works from plain JavaScript (ESM, CommonJS, or a CDN `<script type="module">`)
- Patches `fetch` (and optionally XHR) to attach requests, status codes and timings to the triggering interaction
- Uses `MutationObserver` to summarize DOM changes (nodes added, removed, attributes changed)
- Optional HTML hints: `data-act` to name interactions, `data-act-boundary` to group them by module
- Privacy by default: never records input values, auth/cookie headers, request/response bodies or sensitive fields
- Small controller API: `stop()`, `flush()`, `getSnapshot()`

```
ActTrace #1 — customer.save
  event    click
  target   button[data-act="customer.save"]
  boundary CustomerModule
  network  POST /api/customers -> 201 (142ms)
  dom      7 mutations (3 added, 1 removed, 3 attr)
  duration 318ms
```

Status: experimental (v0.0.1), MIT licensed.

### [annoying-design](https://github.com/alex-mosneagu/annoying-design)

A deliberately chaotic typing challenge built with **Vue 3**. You have to type one sentence correctly while the input field moves around and keeps changing under you. It's a playful look at how much UX depends on stable, predictable interfaces, and an exercise in reactive state and DOM manipulation in Vue.

## Selected client work

*Private repositories. Built through Old Studio Concept.*

| Project | Scope |
|---|---|
| **Pasion Digital** | Full platform rebuild: Laravel API with a Filament admin and a Nuxt frontend, replacing a legacy Symfony/Twig stack. |
| **GeniusMind Academy** | Education platform: public site, Vue admin CMS, and PHP API on MariaDB. |
| **LiveFlow Academy** | Udemy-style online course marketplace built with Nuxt 4. |

## Languages

| Language | |
|---|---|
| Romanian | Native |
| Italian | Fluent |
| English | Fluent |

## Contact

- Website: [oldstudioconcept.ro](https://oldstudioconcept.ro)
- LinkedIn: [linkedin.com/in/andrei-alexandru-mosneagu](https://www.linkedin.com/in/andrei-alexandru-mosneagu)

---

![GitHub stats](https://github-readme-stats.vercel.app/api?username=alex-mosneagu&show_icons=true&hide_border=true)
