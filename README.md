<h1 align="center">Thibault Lafaurie</h1>

<p align="center">
  <code>@Labault</code>
</p>

<p align="center">
  <em>Backend developer, 7 years in production on PHP/Symfony.</em><br>
  Legacy migrations (PHP 7.0 → 8.3, Symfony 2.8 → 7.4), real-time apps, owned end to end down to the VPS.<br>
  <sub>Turns coffee into features. Fluent in Docker, PostgreSQL, and PHP at 2 a.m. Clean apps, documented decisions.</sub>
</p>

<p align="center">
  🐥 <strong>Quack quack</strong> · 📍 Clermont-Ferrand, France · 🌐 <a href="https://labault.dev"><strong>labault.dev</strong></a>
</p>

---

### Who I actually am, jokes aside

Those **7 years** went into building and growing one real product: gathering
requirements, keeping legacy alive, and migrating a codebase from **PHP 7.0 →
8.3** and **Symfony 2.8 → 7.4** without breaking what people depend on.

I care about the parts nobody sees: APIs that don't wake anyone up at night,
tests you can read like a story, and logs you actually enjoy opening. I'm just
as comfortable past the code **Docker, FrankenPHP, Caddy/Traefik, CI/CD,
self-hosted deployment on a VPS**. Backend forever, but I like owning the whole
chain down to production.

---

### Stack

**Core** &nbsp;
![PHP](https://img.shields.io/badge/PHP_8.3-777BB4?style=flat&logo=php&logoColor=white)
![Symfony](https://img.shields.io/badge/Symfony_7.4-000000?style=flat&logo=symfony&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Doctrine](https://img.shields.io/badge/Doctrine-FC6A31?style=flat&logo=doctrine&logoColor=white)

**Real-time & async** &nbsp;
![Mercure](https://img.shields.io/badge/Mercure-FE6A16?style=flat&logoColor=white)
![Messenger](https://img.shields.io/badge/Symfony_Messenger-000000?style=flat&logo=symfony&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat&logo=redis&logoColor=white)

**Infra & ops** &nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![FrankenPHP](https://img.shields.io/badge/FrankenPHP-00A8E8?style=flat&logoColor=white)
![Caddy](https://img.shields.io/badge/Caddy-1F88C0?style=flat&logo=caddy&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=flat&logo=traefikproxy&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)

**Observability** &nbsp;
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat&logo=opentelemetry&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)

**Also** &nbsp;
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![Stimulus](https://img.shields.io/badge/Stimulus/Turbo-77E8B9?style=flat&logoColor=black)
&nbsp; *(and learning React on the side)*

---

### What I'm building

🎓 **[Docendo](https://docendo.fr)**, *co-founder & backend* · live SaaS

An AI tutor for French primary & middle-school students (CP → 3e). A real product
with real users and a real billing model, not a toy. The interesting engineering:

- An **IRT / Rasch psychometric engine** that calibrates every exercise to pinpoint
  a student's actual gaps, not just their grades.
- **Milo**, an AI tutor that never gives the answer, graded hints, prompt-injection
  filtering, aligned with the official national curriculum.
- **MiloTalk**: spoken answers transcribed by a **self-hosted Whisper**, the child's
  voice never leaves our European servers, audio destroyed right after transcription.
- Stripe billing, GDPR-first data handling, PWA, OCR homework scanning.

> Built with [@Antho](https://github.com/anthomas63), private codebase, product is live at
> **[docendo.fr](https://docendo.fr)**.

---

### Things I've built solo

**Live apps**, real users, shipped solo. Roughly ordered by how much backend runs underneath:

| Project | What it is | Stack highlight |
| ------- | ---------- | --------------- |
| 🎯 **[Red Flag Bingo](https://github.com/Labault/red-flag-bingo)** · [live](https://redflagbingo.fun) | Real-time collaborative bingo for dating red flags | Mercure live sync inside FrankenPHP, worker mode |
| 🦆 **[Le Canard du Vendredi](https://github.com/Labault/FridayDuck)** · [live](https://tibec.labault.dev) | A duck that wakes up on Fridays to remind you not to deploy | Real-time Mercure, hardened multi-stage container, restic backups, full OTel/Grafana stack |
| 🤫 **[Hush](https://github.com/Labault/Hush)** · [live](https://hush.labault.dev) | A timer that scores how long you stay away | Server-authoritative anti-cheat, no-login leaderboard |
| 🧠 **[Humelis](https://humelis.labault.dev)** · [live](https://humelis.labault.dev) | Daily mood logging that turns feelings into trends, shareable with a clinician | QR-code clinician pairing, patient owns the data (revocable any time), mood analytics dashboard |
| 🗣️ **[DevSpeak](https://devspeak.labault.dev)** · [live](https://devspeak.labault.dev) | Turns plain sentences into certified senior-engineer jargon | Bullshit-as-a-service, multiple expert personas, one-click copy |

**Toolchain** that ships the rest:

| Project | What it is | Stack highlight |
| ------- | ---------- | --------------- |
| 💻 **[mac-dev-setup](https://github.com/Labault/mac-dev-setup)** | One-command macOS dev environment | Homebrew, Zsh, PHP/Symfony, small rituals |
| 🧰 **[bootstrap-web-setup](https://github.com/Labault/bootstrap-web-setup)** | Scaffolds code-quality config into a fresh project | PHPStan lvl 9, Rector, PHP-CS-Fixer, `.bootstrap.yaml` |
| 🖥️ **[server-setup](https://github.com/Labault/server-setup)** | Turns a bare VPS into a production-ready host | Server provisioning and hardening, the boring infra nobody documents |
| 🚀 **[push-to-deploy](https://github.com/Labault/push-to-deploy)** | Self-hosted single-VPS deployment platform | Caddy reverse proxy, HMAC webhook CD, encrypted backups |
| 🧩 **[labault-marketplace](https://github.com/Labault/labault-marketplace)** | My Claude Code plugin marketplace, PHP/Symfony-focused | `symfony-forge`: bootstrap skill, reviewer agent, `/quality-gate` command |

<sub><strong>mac-dev-setup → bootstrap-web-setup → server-setup → push-to-deploy</strong>: from a fresh laptop to production on a single VPS, owned end to end. No PaaS, no Kubernetes, no Friday.</sub>

---

### Currently shipping

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Labault&hide_border=true&bg_color=00000000&color=777BB4&line=FE6A16&point=777BB4&area=true&area_color=FE6A16" alt="Thibault's contribution graph" />
</p>

---

### Let's talk

I'm open to projects backend, infra, or the whole pipeline.

📫 **[contact@labault.dev](mailto:contact@labault.dev)** &nbsp;·&nbsp;
🌐 **[labault.dev](https://labault.dev)** &nbsp;·&nbsp;
💼 **[LinkedIn](https://www.linkedin.com/in/thibault-lafaurie-143690151/)**

<sub><em>Never a deploy on a Friday. <a href="https://tibec.labault.dev">The duck is watching</a>. 🦆</em></sub>
