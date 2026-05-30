<h1 align="center">Hey, I'm Hrushikesh 👋</h1>

<p align="center">
  <strong>Founder of <a href="https://tweak.page">Tweak</a></strong> — live website review on the real DOM
</p>

<p align="center">
  <a href="https://tweak.page"><img src="https://raw.githubusercontent.com/hrushikeshvetagiri-tweak/hrushikeshvetagiri-tweak/main/assets/logo.png" width="64" alt="Tweak" /></a>
</p>

<p align="center">
  <a href="https://tweak.page"><img src="https://img.shields.io/badge/→_tweak.page-visit-181717?style=flat-square" alt="tweak.page" /></a>
  <a href="https://chromewebstore.google.com/detail/tweak/fnfobegjifomgobgilaemihpcpidjamc"><img src="https://img.shields.io/badge/Chrome-extension-181717?style=flat-square&logo=googlechrome&logoColor=white" alt="Chrome extension" /></a>
  <a href="https://tweak.page/docs/mcp"><img src="https://img.shields.io/badge/MCP-docs-181717?style=flat-square" alt="MCP docs" /></a>
</p>

---

> **Clients don't send CSS selectors in Slack.** They send screenshots.
> I built Tweak so feedback stays on the **live page** — pinned to real elements — and flows straight to developers (and AI) as structured issues.

<table>
  <tr>
    <td width="50%" valign="top">

### 😩 The old loop

- Screenshot → email → guess the element
- Context lost on every reply
- "Which button?" threads for days
- AI gets a PNG, not a selector

  </td>
  <td width="50%" valign="top">

### ✨ With Tweak

- Client opens your **staging URL**
- Pins land on the **real DOM**
- Dev jumps to exact spot via hub
- Optional **MCP** handoff in Cursor

  </td>
  </tr>
</table>

```mermaid
flowchart LR
  A["👤 Client"] --> B["🔗 Share link / embed"]
  B --> C["📌 Issues on live page"]
  C --> D["🛠 Hub + extension"]
  C --> E["🤖 MCP · Cursor"]
  D --> F["✅ Resolve + PR"]
```

---

<details open>
<summary><strong>What Tweak is</strong></summary>
<br />

**Embed-first website review** — not a screenshot tool, not Jira.

| Who | What they do |
|:--|:--|
| **Clients** | Comment on the live site via share link or embed. No install. |
| **Developers** | Chrome extension + hub — claim, Go To, link PRs, resolve. |
| **AI** | `tweak-mcp` exposes canonical issues to Cursor / Claude. |

```mermaid
flowchart TB
  subgraph live ["On the customer's URL"]
    E["embed overlay"]
  end
  subgraph tools ["Same review, any surface"]
    X["extension"]
    H["hub /s/id"]
    M["tweak-mcp"]
  end
  E --> R[(one review · one ops layer)]
  X --> R
  H --> R
  M --> R
```

<p align="center">
  <a href="https://tweak.page"><strong>Try it → tweak.page</strong></a>
</p>

</details>

<details>
<summary><strong>Stack I ship with</strong></summary>
<br />

`Preact` · `Signals` · `TypeScript` · `Tailwind` · `Cloudflare Workers` · `D1` · `R2` · `Hono` · `WXT` · `MCP` · `Bun` · `Turborepo`

**Right now:** embed-first review for agencies · MCP feedback loop · persist on messy real-world SPAs

</details>

---

<h3 align="center">GitHub</h3>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=hrushikeshvetagiri-tweak&theme=github" alt="Stats" height="160" />
  <img src="https://streak-stats.demolab.com/?user=hrushikeshvetagiri-tweak&theme=default&hide_border=true" alt="Streak" height="160" />
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=hrushikeshvetagiri-tweak&theme=github" alt="Languages" height="160" />
</p>

---

<p align="center">
  <strong>Building in public.</strong><br />
  Review websites for clients? <a href="https://tweak.page">Drop Tweak on your staging URL</a> — takes minutes.
</p>

<p align="center">
  <a href="https://github.com/hrushikeshvetagiri-tweak">@hrushikeshvetagiri-tweak</a>
  ·
  <a href="https://github.com/tweak-page">@tweak-page</a>
</p>
