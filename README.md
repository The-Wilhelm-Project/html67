# html67

# HTML67 — HTML, thought further

> The kitchen sink.

Cards, charts, legal and domain elements as native tags: one script, no build step. **122 elements, 0 build steps**, built on top of HTML5.

HTML67 is part of [Project Wilhelm](https://html67.de).

---

## Overview

The official HTML standard [calls itself a kitchen sink](https://html.spec.whatwg.org/#introduction) — everything but the kitchen sink, the basin where all of it ends up. And the picture it draws of itself is exactly that: a sink, plumbed into the web.

```
Graphic 1 — the kitchen sink (HTML5, the specification)

              ┌────────────────────────────────────────┐
              │  CSS    SVG    MathML   ServiceWorkers  │   built on top
              └────────────────────────────────────────┘
   ┌───────┐  ┌────────────────────────────────────────┐
   │ IDB   │  │                                        │
   │ Fetch │  │             THE  SINK                  │   ← HTML
   │ CSP   │  │         "this specification"           │
   │ PNG   │  │                                        │
   │ Opus  │  │                                        │
   │ AV1   │  │                                        │
   └───────┘  └────────────────────────────────────────┘
    tools     ┌────────────────────────────────────────┐
   alongside  │ HTTP  TLS  DOM  Unicode  WebIDL         │   the plumbing
              │ MIME  URL  XML  JavaScript  Encoding    │   it stands on
              └────────────────────────────────────────┘
```

The sink is plumbed into HTTP, URL, MIME, the DOM. The soap and sponges on the side — PNG, Opus, AV1, Fetch — are the tools you reach for. And then you also wash CSS, SVG and MathML in the same basin. One sink, for everything. It's honest. It's even funny. And it's the whole problem.

### A living standard still needs tending

You can do anything in this sink — that's the point, and the catch. It's called a living standard, but living things don't stay alive on their own. A bathroom doesn't stay clean because it's alive. It stays clean because someone tends it. And lately, no one has. The pressure comes from all three sides at once — and the basin fills with everything that doesn't fit.

```
Graphic 2 — real life HTML5

      we now build ▸  documents · apps · layouts · interfaces
                          (far more than the basin was meant to hold)
                                       ▲
   sink-embeds ◂ <model-viewer> ◂ threejs ◂ iframes ◂ video-players
        ╲          ╲           │           ╱          ╱
              ┌────────────────────────────────────────┐
              │  CSS    SVG    MathML   ServiceWorkers  │   still on top
              └────────────────────────────────────────┘
   ┌───────┐  ┌────────────────────────────────────────┐
   │ IDB   │  │  🗑 tailwind   🗑 bootstrap   🗑 jQuery   │ ──cdn #7
   │ Fetch │  │  🗑 react   🗑 vue   🗑 the 14th frmwrk  │ ──polyfill
   │ CSP   │  │  💩 widgets   💩 utility-class soup      │ ──shim
   │ PNG   │  │  🗑 dep  🗑 dep  🗑 dep   ☠ css won't    │ ──cdn #1
   │ Opus  │  │       ~ ~ ~  grey water  ~ ~ ~ ~ ~      │
   │ AV1   │  │             THE  SINK  (clogged)        │ ← HTML
   └───────┘  └────────────────────────────────────────┘
    tools     ┌────────────────────────────────────────┐
   alongside  │ HTTP  TLS  DOM  Unicode  WebIDL         │   the plumbing
   + webasm   │ MIME  URL  XML  JavaScript  Encoding    │   (ground shifting)
              └────────────────────────────────────────┘
```

From below, new plumbing arrives — WebAssembly changes what the basin even sits on. From the side, new materials pile up — video, 3D, interactive media with no real home in the markup, so we bolt them onto the rim. From above, we ask it to do far more than show a document. And so the basin fills with what doesn't fit: utility classes, widgets, a dozen CDNs that all do the same thing, framework after framework re-solving the same problem. The one line that held it together — the clean separation of meaning, structure, and design — is no longer a standard anyone agrees on. The sink still works. But the water's gone grey.

### So we're upgrading the sink

We're not here to tear it out. HTML is a living standard, and we want to keep it that way — without letting it sprawl. We respect the ideas underneath and give them room to breathe again. Everything that used to balance on the rim moves inside, as native elements. Every filetype gets a home.

```
Graphic 3 — HTML6

        ┌──────────────────────────────────────────────────┐
        │  CSS   SVG   MathML   ServiceWorkers              │
        │  + Markdown  + Webapps  + Documents  + Editors    │   built on top
        └──────────────────────────────────────────────────┘
   ┌────────┐  ┌──────────────────────────────────────────────────┐
   │ IDB    │  │                                                  │
   │ Fetch  │  │                                                  │
   │ CSP    │  │                                                  │
   │ PNG    │  │              A  CLEANER  BASIN                   │  ← HTML6
   │ Opus   │  │          meaning · structure · design            │
   │ AV1    │  │                                                  │
   │ MP4    │  │                                                  │
   │ OBJ    │  │                                                  │
   │ GLB    │  │                                                  │
   │ ICS    │  │                                                  │
   │ PDF    │  │                                                  │
   │ WEBP   │  │                                                  │
   └────────┘  └──────────────────────────────────────────────────┘
   tools +     ┌──────────────────────────────────────────────────┐
   filetypes,  │ HTTP  TLS  DOM  Unicode  WebIDL                   │  the plumbing
   now native  │ MIME  URL  XML  JavaScript  Encoding  + WebAssembly│  it stands on
               └──────────────────────────────────────────────────┘
```

The basin is empty again — clean ceramic. CSS, SVG, MathML and ServiceWorkers still sit on top, now joined by Markdown, web-apps, documents and editors: everything the modern web is actually used for. The filetypes that used to be bolted on from outside — MP4, OBJ, GLB, ICS, PDF, WEBP — are native tools on the side, no embed, no third-party player. And WebAssembly joins the plumbing at the bottom, because the foundation moved and now the basin sits on it on purpose. **122 elements, 0 build steps.**

### HTML7 — connect it to the water

Here's the thing almost everyone forgets about the kitchen sink: the most beautiful basin is useless until someone connects it to the water. HTML7 is the line going down — to law, to region, to the living world the page lives in. Same basin as HTML6, now plumbed in.

```
Graphic 4 — HTML7

        ┌──────────────────────────────────────────────────┐
        │  CSS   SVG   MathML   ServiceWorkers              │
        │  + GlyphMarkdown  + Webapps  + Documents + Editors │   built on top
        └──────────────────────────────────────────────────┘
   ┌────────┐  ┌──────────────────────────────────────────────────┐
   │ IDB    │  │                                                  │
   │ Fetch  │  │                                                  │
   │ CSP    │  │                                                  │
   │ PNG    │  │              THE  LIVING  BASIN                  │  ← HTML7
   │ Opus   │  │          meaning · structure · design            │
   │ AV1    │  │       + <norm> <cite> <unit> <license>           │
   │ MP4    │  │                                                  │
   │ OBJ    │  │                                                  │
   │ GLB    │  │                                                  │
   │ ICS    │  │                                                  │
   │ PDF    │  │                                                  │
   │ WEBP   │  │                                                  │
   └────────┘  └─────┬─┬────────────┬─┬──────────────────┬─┬──────┘
   tools +           │ │            │ │                  │ │
   filetypes,        │ │            │ │                  │ │
   now native       (   )─(⏱)      (   )─(⏱)            (   )─(⏱)
                   analytics      legal               legal
                   + OpenGraph    regulatories        standards (in)
        ┌────────────┴─┴────────────┴─┴──────────────────┴─┴──────┐
        │  Law · Rights · Invoices · Bathrooms · Local Adapters    │
        │  DSGVO · SEPA · BGB · currency · OpenGraph · SEO · meta   │  the water main
        └──────────────────────────────────────────────────────────┘
             the community · the city · the state · the EU
```

The basin is the same one from HTML6 — identical ceramic. What changes is that it's finally connected. The pipes running down carry the things a page owes to the world it lives in: one valve meters analytics and OpenGraph, one legal regulatories, one is the intake for legal standards — and the timers (⏱) are the joke with a true core: law changes, deadlines run, mandates expire, SEO and meta drift. The legal components keep the water clean and check that every adapter for your region is connected and current. `<consent>` knows the DSGVO, `<sepa-mandate>` the SEPA rulebook, `<norm>` resolves § 433 BGB or Art. 6 DSGVO to your jurisdiction. The water main below — DSGVO, SEPA, BGB, currency, OpenGraph, SEO, meta — is the city it taps into. One basin anyone can install. Water only an HTML7 region adapter can turn on.

---

## Performance

### How it compares

|                                              | HTML + CSS · 2000s              | HTML5 · average today                                | HTML67                       |
| -------------------------------------------- | ------------------------------- | ---------------------------------------------------- | ---------------------------- |
| Typical build                                | hand-written HTML, one CSS file | framework + bundler + utility CSS + component libs   | native elements, no build    |
| Total page weight                            | ~50–200 KB                      | ~2–5 MB                                              | ~150–400 KB                  |
| Loading time                                 | ~1–3 s (slow line)              | 3–10 s                                              | < 1 s                        |
| External servers / origins                   | 0–1 (just your own)             | 8–20+ (CDNs, fonts, analytics, embeds, ads)         | 1 (your own)                 |
| CDNs / third parties                         | none, or one for jQuery later   | 5–150                                               | none                         |
| HTTP requests                                | 5–15                            | 70–150+                                             | 1–10                         |
| Legal (DSGVO · DMA · accessibility)          | no                              | no                                                   | **yes — built in**           |
| Renders without server / network             | yes                             | rarely (CDN-dependent)                              | yes                          |
| AI- & SEO-ready (machine-readable meaning)   | no                              | no                                                   | yes                          |
| Universal standard (web · print · apps)      | no                              | no                                                   | yes                          |

### Why it saves

Data centres are racing toward 950 TWh a year — near 3% of the world's electricity by 2030, growing more than four times faster than demand overall (IEA, Energy & AI 2025). And most of what they move isn't meaning. Around 70% of all web traffic now flows through CDNs — by some counts over 80%. Much of that is video, but for the pages, apps and documents people actually read, a large share of every transfer isn't content at all. It's scaffolding: framework code, duplicate libraries, dependencies, trackers — markup written to be rendered, not understood. HTML67 ships the meaning and drops the scaffolding. Here's what that saves.

#### –90% energy & data waste — meaning, not scaffolding

A modern page ships ~3 MB to deliver ~20 KB of real meaning — the HTML is barely 1% of the download; the rest is frameworks, fonts and images. HTML67: ~200–400 KB.

> Source: HTTP Archive / Web Almanac 2025 — median desktop page ~2.6 MB, ~180× heavier than the 90s; JS ~25% of weight.

#### –99% HTTP requests — not 5–15 servers

A typical page fires 70–150+ requests across 10–20 origins — CDNs, fonts, trackers, embeds. HTML67: 1–10, from one server, zero CDNs in front.

> Source: HTTP Archive / Web Almanac 2025 — median page ~70+ requests; 92% of sites load third-party scripts.

#### –75% server computing power — self-hosted, zero third parties

Servers are ~60% of data-centre electricity; every framework re-render, duplicate dependency and third-party call adds load. Fewer bytes and no third parties means less to process.

> Source: IEA Energy & AI 2025 — servers ~60% of data-centre power; data centres ~1.5% of global electricity, doubling to ~950 TWh by 2030.

#### –50% AI tokens — compressed context, better indexing

A semantic `<price>` or `<norm>` says in one tag what class-soup takes twenty to imply — so a crawler indexes less and a model reads fewer tokens for the same meaning.

> Source: IEA Energy & AI 2025/26 — a simple AI query draws ~10× a web search; per-page token savings measured vs. a typical framework + utility-CSS build.

---

HTML67 is part of **Project Wilhelm** — a standard is only the first stone, and this is just the beginning.

© Bekesi GmbH · Rablstraße 21b, 81669 München · [sven@bekesi.group](mailto:sven@bekesi.group)
