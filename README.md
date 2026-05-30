<!-- GitHub profile README — dark variant -->
<!-- Repo: github.com/hrushikeshvetagiri-tweak/hrushikeshvetagiri-tweak -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6366f1,100:0d1117&height=160&section=header&text=TWEAK&fontSize=48&fontColor=f4f4f5&animation=fadeIn" alt="TWEAK" width="100%" />

<br />

<a href="https://tweak.page">
  <img src="https://raw.githubusercontent.com/hrushikeshvetagiri-tweak/hrushikeshvetagiri-tweak/main/assets/logo.png" alt="Tweak logo" width="88" />
</a>

<br /><br />

<img src="https://github.com/hrushikeshvetagiri-tweak.png" alt="Vetagiri Hrushikesh" width="100" />

### Vetagiri Hrushikesh

**Founder & builder** · building [**Tweak**](https://tweak.page)

*Review live websites in the browser. Turn feedback into code.*

<br />

[![Tweak](https://img.shields.io/badge/Tweak-tweak.page-6366f1?style=for-the-badge)](https://tweak.page)
[![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://chromewebstore.google.com/detail/tweak/fnfobegjifomgobgilaemihpcpidjamc)
[![MCP](https://img.shields.io/badge/MCP-tweak--mcp-8b5cf6?style=for-the-badge)](https://tweak.page/docs/mcp)
[![Status](https://img.shields.io/badge/Status-Shipping-22c55e?style=for-the-badge)](#)

</div>

---

## About

I build **live website review infrastructure** — the layer between vague client feedback and merged code.

Screenshot threads and Slack messages lose selectors, scroll context, and intent. **Tweak** keeps feedback on the **real DOM**: clients pin issues on staging or production; developers triage in a hub, resolve work, and optionally hand structured issues to AI via MCP.

```mermaid
flowchart LR
  Client["Client"] --> Embed["Embed / share link"]
  Embed --> Issues["Structured issues"]
  Issues --> Hub["Hub + extension"]
  Hub --> Resolve["PR / resolve"]
  Issues --> MCP["tweak-mcp · Cursor"]
```

---

## Tweak at a glance

| Role | Experience |
|------|------------|
| **Clients** | Share link or on-site embed — comment, inspect, draw. No install. |
| **Developers** | Chrome extension + hub `/s/{id}` — claim, Go To, link PRs, resolve. |
| **AI (optional)** | `tweak-mcp` — canonical issues in Cursor, VS Code, Claude. |

```mermaid
flowchart TB
  subgraph site ["Customer site · staging or production"]
    Embed["@tweak/embed · real DOM overlay"]
  end

  subgraph surfaces ["Review surfaces"]
    Ext["Chrome extension"]
    Hub["Hub /s/{id}"]
    MCP["tweak-mcp"]
  end

  subgraph cloud ["Cloud · one review id"]
    API["Workers · D1 · R2 · ops_json"]
  end

  Embed --> API
  Ext --> API
  Hub --> API
  MCP --> API
```

**Live-site-first** · **One review, one truth** · **Embed + extension, one overlay** · **AI-native MCP**

→ [tweak.page](https://tweak.page) · [Chrome Web Store](https://chromewebstore.google.com/detail/tweak/fnfobegjifomgobgilaemihpcpidjamc)

---

## GitHub activity

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=hrushikeshvetagiri-tweak&theme=6366f1" alt="Profile details" height="180" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=hrushikeshvetagiri-tweak&theme=6366f1" alt="GitHub stats" height="180" />

<br />

<img src="https://streak-stats.demolab.com/?user=hrushikeshvetagiri-tweak&theme=dark&hide_border=true&background=0D1117&ring=6366F1&fire=6366F1&currStreakLabel=6366F1&sideLabels=6366F1&dates=71717A" alt="GitHub streak" height="180" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=hrushikeshvetagiri-tweak&theme=6366f1" alt="Top languages" height="180" />

</div>

---

## Stack

```mermaid
mindmap
  root((Tweak stack))
    Frontend
      Preact
      Signals
      Tailwind v4
      TypeScript
    Platform
      Cloudflare Workers
      D1
      R2
      Hono
    Tools
      WXT extension
      tweak-mcp
      Bun
      Turborepo
```

---

## Focus now

```mermaid
flowchart LR
  A["Embed-first review"] --> B["Agencies & dev shops"]
  C["Client feedback"] --> D["Cursor MCP"]
  D --> E["Implementation loop"]
  F["Persist + SPA nav"] --> G["Real client sites"]
```

- Embed-first review for agencies and dev shops
- Client feedback → Cursor MCP → implementation loop
- Persist, SPA navigation, and multi-tab integrity on real client sites

---

<div align="center">

**Building in public.**

[Try Tweak on your staging URL](https://tweak.page) · [GitHub](https://github.com/hrushikeshvetagiri-tweak)

<br />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=6366F1&center=true&vCenter=true&width=480&lines=Live-site+review+%E2%86%92+structured+issues;Feedback+on+the+real+DOM;From+pin+to+merged+PR" alt="Typing animation" />

</div>
