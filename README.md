# HTML67
**Released · July 4, 2026

HTML67 is a runtime that extends HTML into a complete application language. It adds semantic elements, native Ul components, layouts, dialogs, Al primitives, and application features while remaining compatible with today's browsers.

Write applications using HTML instead of frameworks. HTML67 introduces native components, layouts, dialogs, forms, AI elements, and application primitives directly as HTML tags—without a build step.
The long-awaited **HTML6** clean-up and the first **HTML7** legal layer, shipped as native elements. One script, no build step, zero dependencies. **122 elements** on top of HTML5.

---

## The living kitchen sink

> "Everything but the kitchen sink, the basin where all of it ends up."

HTML5 calls itself a living standard and a kitchen sink:

```
Graphic 1 — the kitchen sink HTML5

              ┌────────────────────────────────────────┐
              │  CSS    SVG    MathML   ServiceWorkers │ doctypes built on top
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
   alongside  │ HTTP  TLS  DOM  Unicode  WebIDL        │ ← plumbing
              │ MIME  URL  XML  JavaScript  Encoding   │
              └────────────────────────────────────────┘
```

And the picture it draws of itself is exactly that: a sink, plumbed into the web, into HTTP, URL, MIME and the DOM. The soap and sponges on the side; PNG, Opus, AV1, Fetch are the tools you reach for. And then you also wash CSS, SVG and MathML in the same basin. One sink, for everything. It's honest. It's even funny. And it's the whole problem:

```
Graphic 2 — real life HTML5                now used for anything:

              ┌────────────────────────────────────────┐
              │ apps · layouts· interfaces·CMS Systems │
              │ video-players·3d Engines·Complex Tools │
              └────────────────────────────────────────┘
                basin was meant to hold documents:
              ┌────────────────────────────────────────┐
              │  CSS    SVG    MathML   ServiceWorkers │
              └────────────────────────────────────────┘
   ┌───────┐  ┌────────────────────────────────────────┐
   │ IDB   │  │  🗑 tailwind   🗑 bootstrap  🗑 jQuery│ ──cdn #7
   │ Fetch │  │  🗑 react   🗑 vue 🗑 the 14th frmwrk │ ──polyfill
   │ CSP   │  │  💩 widgets   💩 utility-class soup   │ ──shim
   │ PNG   │  │  🗑 dep  🗑 dep  🗑 dep   ☠ css won't │ ──cdn #1
   │ Opus  │  │       ~ ~ ~  grey water  ~ ~ ~ ~ ~     │
   │ AV1   │  │             THE  SINK  (clogged)       │
   └───────┘  └────────────────────────────────────────┘
    tools     ┌────────────────────────────────────────┐
   alongside  │ HTTP  TLS  DOM  Unicode  WebIDL        │
   + webasm   │ MIME  URL  XML  JavaScript  Encoding   │
              └────────────────────────────────────────┘
```

Built for documents, used for literally everything. A standard never changed even when new plumbing arrives, WebAssembly changes what the basin even sits on. From the side, new materials pile up; video, 3D, interactive media, chats, communication and collaboration tools that never seen any markup, so we bolt them onto the rim. And so the basin fills with what doesn't fit: utility classes, widgets, a dozen CDNs that all do the same thing, framework after framework re-solving the same problem. CDN & NPM got the new standard managing libraries HTML once was.

### Living standards can die too

You can do anything in this sink, that's the point, and the catch. It's called a living standard, but living things don't stay alive on their own. A bathroom doesn't get cleaner being alive…

Built as a *living standard*, HTML5 should have been the last HTML version — once and for all. Sometimes your plans may change after you've created life, especially once it starts to stink somewhere. HTML should neither have a bad nor a standard life. It's about having an active, healthy and good life with dreams and visions, especially if you are a living standard 5,500,000,000 people interact with daily.

We want HTML to stay alive, keep learning throughout its life, and actively evolve.

HTML5 was released 12 years ago. Back in 2014, around 2 billion people used smartphones, and only 25% of web traffic came from mobile devices. Today, those numbers have grown to 5.65 billion smartphone users, with nearly 60% of all web traffic coming from mobile.

We set out to build the next generation of HTML. But while we were working on HTML6, our long-awaited update was already being overtaken by the rapid advances in AI, which is why we're proudly releasing two major updates at once.

## HTML6 — clean the sink

Cleans and modernizes HTML's legacy components and brings them up to today's standards. We're not here to tear it out. HTML5 is a living standard, and we want to keep it that way, without letting it sprawl. We respect the ideas underneath and give them room to breathe again. Everything that used to balance on the rim moves inside, as native elements. Every filetype gets a home.

```
Graphic 3 — HTML6

               ┌──────────────────────────────────────────────────┐
               │  CSS   SVG   MathML   ServiceWorkers             │
               │  + Markdown  + Webapps  + Documents  + Editors   │
               └──────────────────────────────────────────────────┘
   ┌────────┐  ┌──────────────────────────────────────────────────┐
   │ IDB    │  │                                                  │
   │ Fetch  │  │                                                  │
   │ CSP    │  │                                                  │
   │ PNG    │  │                                                  │
   │ Opus   │  │                                                  │
   │ AV1    │  │                                                  │ ← clean
   │ MP4    │  │                                                  │
   │ OBJ    │  │                                                  │
   │ GLB    │  │                                                  │
   │ ICS    │  │                                                  │
   │ PDF    │  │                                                  │
   │ WEBP   │  │                                                  │
   └────────┘  └──────────────────────────────────────────────────┘
   tools +     ┌──────────────────────────────────────────────────┐
   filetypes,  │ HTTP  TLS  DOM  Unicode  WebIDL                  │
   now native  │ MIME  URL  XML JavaScript Encoding  + WebAssembly│
               └──────────────────────────────────────────────────┘
```

How a clean ceramic should look: structural components added for web-apps, documents and editors. HTML, its text use-case UI-maxxed with native markdown and state of the art components. Added filetypes that used to be bolted on from outside: MP4, OBJ, GLB, ICS, PDF, WEBP are native tools on the side, no embed, no third-party player. And WebAssembly joins the plumbing at the bottom, because the foundation moved and now the basin sits on it on purpose.

## HTML7 — connect it to the water

Introducing new native components, legal and accessibility extensions and an entirely new built-in AI chat environment. Here's the thing almost everyone forgets about the kitchen sink: the most beautiful basin is useless until someone connects it to the water. HTML7 is the line going down; to law, to region, to the living world the page lives in. Same basin as HTML6, now plumbed in.

```
Graphic 4 — HTML7

              ┌──────────────────────────────────────────────────┐
              │  CSS   SVG   MathML   ServiceWorkers             │
              │  + GlyphMarkdown  + Webapps+ Documents + Editors │
              └──────────────────────────────────────────────────┘
   ┌────────┐  ┌──────────────────────────────────────────────────┐
   │ IDB    │  │                                                  │
   │ Fetch  │  │                                                  │
   │ CSP    │  │                                                  │
   │ PNG    │  │                                                  │
   │ Opus   │  │                                                  │
   │ AV1    │  │                                                  │
   │ MP4    │  │                                                  │  ← still
   │ OBJ    │  │                                                  │    clean
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

The basin is the same one from HTML6 — identical ceramic. What changes is that it's finally connected. The legal components keep the water clean and check that every adapter for your region is connected and current. `<consent>` knows the GDPR, `<sepa-mandate>` the SEPA rulebook, `<norm>` resolves § 433 BGB or Art. 6 DSGVO to your jurisdiction. The water main below — DSGVO, SEPA, BGB, currency, OpenGraph, SEO, meta — is the city it taps into. One basin anyone can install. Water only an HTML7 region adapter can turn on.

*One more thing… a native HTML map and an address picker… am I dreaming?*

---

## Quickstart

No install, no build, no bundler. Drop three lines into any HTML page and start writing `<wl-*>` elements:

```html
<link rel="stylesheet" href="https://cdn.html67.org/src/tokens.css" />
<script type="importmap">
  { "imports": { "@wilhelm/ui": "https://cdn.html67.org/src/wilhelm.js", "@wilhelm/ui/": "https://cdn.html67.org/src/" } }
</script>
<script type="module" src="https://cdn.html67.org/src/wilhelm.js"></script>

<wl-card>
  <h3 slot="title">Hello HTML67</h3>
  A card as a native tag. No framework. No build step.
</wl-card>
```

Or self-host — clone this repo and serve the folder:

```bash
git clone https://github.com/The-Wilhelm-Project/html67.git
cd html67 && npm run dev   # zero-dependency live-reload dev server
```

## What's in the box

- **122 native elements** on top of HTML5 — cards, charts, layouts, media, editors and domain tags, no React, no Vue, no Tailwind.
- **HTML6** — legacy clean-up, native Markdown, filetypes (MP4, OBJ, GLB, ICS, PDF, WEBP) with no embeds or third-party players.
- **HTML7** — legal & accessibility components (`<consent>`, `<sepa-mandate>`, `<norm>`, `<cite>`, `<unit>`, `<license>`) and a built-in AI chat environment.
- **Zero dependencies.** One script, one origin, no CDNs in front, renders offline.

## The components

Every component is a native `<wl-*>` tag with light-DOM children — you write markup, not JSX. A few from each family:

**Layout & shell** — `<wl-app-shell>` `<wl-panel>` `<wl-sidebar>` `<wl-stack>` `<wl-resizable>` `<wl-drawer>` `<wl-paper>` `<wl-aspect-ratio>`

**Content & feedback** — `<wl-card>` `<wl-product-card>` `<wl-badge>` `<wl-tag>` `<wl-alert>` `<wl-toast>` `<wl-stat>` `<wl-timeline>` `<wl-empty-state>` `<wl-skeleton>`

**Forms & inputs** — `<wl-input>` `<wl-select>` `<wl-combobox>` `<wl-checkbox>` `<wl-radio-group>` `<wl-switch>` `<wl-slider>` `<wl-date-picker>` `<wl-color-picker>` `<wl-file-upload>` `<wl-rating>` `<wl-signature-pad>` `<wl-form>`

**Navigation & overlays** — `<wl-nav-menu>` `<wl-menubar>` `<wl-breadcrumb>` `<wl-tabs>` `<wl-command>` `<wl-context-menu>` `<wl-dropdown-menu>` `<wl-dialog>` `<wl-popover>` `<wl-tooltip>` `<wl-tour>` `<wl-stepper>`

**Data & charts** — `<wl-chart>` `<wl-donut>` `<wl-pie>` `<wl-treemap>` `<wl-force-graph>` `<wl-bar-race>` `<wl-calendar-heatmap>` `<wl-data-table>` `<wl-vector-map>` `<wl-legend>`

**Media, maps & 3D** — `<wl-image-gallery>` `<wl-carousel>` `<wl-player>` `<wl-waveform>` `<wl-map>` `<wl-place>` `<wl-model-viewer>` `<wl-geo3d>` `<wl-pointcloud>` `<wl-deepzoom>` `<wl-pdf>` `<wl-qr>` `<wl-lottie>`

**Editors & markup** — `<wl-editor>` `<wl-codemirror>` `<wl-code>` `<wl-mermaid>` `<wl-excalidraw>` `<wl-glyph-editor>` `<wl-equation>` `<wl-document>` `<wl-annotatable>`

**HTML7 — legal, region & domain** (the layer no other markup has):

| Tag | What it does |
| --- | --- |
| `<wl-consent>` | GDPR-aware cookie/consent, region-correct out of the box |
| `<wl-sepa-mandate>` | SEPA mandate that knows the rulebook |
| `<wl-norm>` | resolves § 433 BGB or Art. 6 DSGVO to your jurisdiction |
| `<wl-cite>` | citations with machine-readable source metadata |
| `<wl-license>` | license terms as a first-class element |
| `<wl-unit>` `<wl-price>` `<wl-quantity>` | semantic units, currency and amounts |
| `<wl-iban>` `<wl-phone>` `<wl-contact>` `<wl-event>` | validated domain data, no libraries |

Full catalogue: **266 elements** across native tags, 21 web components and 19 composed components — see the [element reference](html67/reference/).

## The release to unite them all: HTML67

Let's talk about performance.

|                                    | HTML5 · average today | HTML67          | delta            |
| ---------------------------------- | --------------------- | --------------- | ---------------- |
| Total page weight                  | ~2–5 MB               | ~150–400 KB     | ~10× lighter     |
| Loading time                       | 3–10 s                | < 1 s           | ~5–10× faster    |
| External origins                   | 8–20+                 | 1               | one server       |
| CDNs / third parties               | 5–150                 | none            | zero             |
| HTTP requests                      | 70–150+               | 1–10            | ~10× fewer       |
| Legal (DSGVO · DMA · a11y)         | no                    | **yes**         | built in         |
| Renders offline without server     | rarely                | **yes**         | —                |
| AI- & SEO-ready (machine meaning)  | no                    | **yes**         | −50% AI context  |

Not another bulky library, more like a cheatsheet containing all libraries ever needed.

- **–90% energy & data waste.** A modern page ships ~3 MB to deliver ~20 KB of real meaning — the HTML is barely 1% of the download; the rest is frameworks, fonts and images. HTML67: ~200–400 KB.
- **–99% HTTP requests.** A typical page fires 70–150+ requests across 10–20 origins — CDNs, fonts, trackers, embeds. HTML67: 1–10, from one server, zero CDNs in front.
- **–75% server computing power.** Servers are ~60% of data-centre electricity; every framework re-render, duplicate dependency and third-party call adds load. Fewer bytes and no third parties means less to process.
- **–50% AI tokens.** Compressed context, better indexing. A semantic `<price>` or `<norm>` says in one tag what class-soup takes twenty to imply — so a crawler indexes less and a model reads fewer tokens for the same meaning. It's like folding an origami out of your context in the shape of your conversation topic, keeping the information needed on the surface and the context available on demand.

Data centres are racing toward 950 TWh a year — near 3% of the world's electricity by 2030, growing more than four times faster than demand overall (IEA, Energy & AI 2025). And most of what they move isn't meaning. Around 70% of all web traffic now flows through CDNs — by some counts over 80%. Much of that is video, but for the pages, apps and documents people actually read, a large share of every transfer isn't content at all. It's scaffolding: framework code, duplicate libraries, dependencies, trackers — markup written to be rendered, not understood. HTML67 ships the meaning and drops the scaffolding.

## What do HTML and SixSeven have in common?

There is no meaning in SixSeven, just as there is no meaning in HTML. And that's exactly the point.

HTML was designed to not contain meaning. To separate semantics from structure and design. Beyond its many technical advantages, this allows creators to focus on content, letting meaning emerge from the content itself rather than from the markup.

What nobody anticipated was just how versatile a markup language could become. Perhaps too versatile. It became the foundation for CMSs, blogging platforms, visual editors, and even closed content ecosystems — uses it was never originally intended to support. Along the way, HTML lost sight of its original purpose in an attempt to capture more and more meaning, chasing the illusion of endless life.

SixSeven puts that illusion to rest. It doesn't live forever because it keeps evolving — it stays alive because people continue to give it meaning.

Freedom is not self-maintaining, the internet needs to be accessible for anyone, programmer or not. HTML67 empowers every person to create sites that are highly functional, legally solid and technically state of the art. Out of the box. With zero dependencies. With zero coding skills.

---

## Docs & reference

- **Element reference & gallery** — [`html67/reference/`](html67/reference/) · live at [www.html67.org](https://www.html67.org)
- **Overview** — the kitchen-sink story, HTML6 & HTML7 in full
- **Performance** — the numbers and their sources
- **Playground** — try elements live in the browser

## Roadmap

HTML6 ships with this release at [www.html67.org](https://www.html67.org); HTML7 follows in Q3 2026, uniting HTML67. Project Wilhelm will ship three further major updates on the road to 2030, when HTML is anchored as its first stable **1.0** release.

## Who's behind it

HTML67 and all future successor versions are maintained by **Project Wilhelm**, a European non-profit dedicated to the upkeep and evolution of the web standard and to completing the digitalisation of the world by 2030.

*HTML67 continues HTML5: the same living standard, now tended, extended and connected to the world it runs in.*

## Contributing

Issues and pull requests welcome — new elements, region adapters (HTML7 legal standards for your jurisdiction), docs and bug reports. See the reference for the element conventions before opening a PR.

## License

Released under the terms in [LICENSE](LICENSE).
