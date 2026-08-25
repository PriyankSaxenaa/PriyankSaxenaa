<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0d1117,50:1f6feb,100:3fb950&height=180&section=header&text=priyank.saxena&fontSize=48&fontColor=ffffff&fontAlignY=42&desc=backend%20engineer%20%C2%B7%20status%3A%20200%20OK&descSize=16&descAlignY=62&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=2800&pause=700&color=3FB950&center=true&vCenter=true&width=760&lines=%24+curl+-X+GET+api.priyank.dev%2Fv1%2Fprofile;%3E+200+OK+%E2%80%94+backend+engineer%2C+accepting+offers;%3E+700%2B+DSA+problems+%C2%B7+LeetCode+1700%2B+%C2%B7+CF+1214;%3E+shipping+HireSync+to+production+right+now" />

<br/>

<a href="https://www.linkedin.com/in/priyank---saxena/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white&labelColor=0d1117"/></a>
<a href="mailto:priyank0saxena@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white&labelColor=0d1117"/></a>
<a href="https://leetcode.com/u/priyanksaxenaa01/"><img src="https://img.shields.io/badge/LeetCode_1700+-FFA116?style=flat-square&logo=leetcode&logoColor=white&labelColor=0d1117"/></a>
<a href="https://github.com/PriyankSaxenaa"><img src="https://img.shields.io/badge/Codeforces_1214-1F8ACB?style=flat-square&logo=codeforces&logoColor=white&labelColor=0d1117"/></a>
<img src="https://komarev.com/ghpvc/?username=PriyankSaxenaa&style=flat-square&color=3fb950&label=visitors&labelColor=0d1117"/>

</div>

---

## `GET /v1/profile`

<img align="right" width="330" src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif"/>

```http
HTTP/1.1 200 OK
Content-Type: application/json
X-Powered-By: Node.js, C++, and an unreasonable amount of chai
Cache-Control: no-cache, always-shipping
```

```json
{
  "name": "Priyank Saxena",
  "role": "Backend Engineer (SDE)",
  "education": "B.Tech CSE — Final Year",
  "location": "India · open to relocate",
  "primary_stack": ["Node.js", "Express", "MongoDB", "Redis", "Socket.IO"],
  "algorithms": { "solved": "700+", "leetcode": 1700, "codeforces": 1214 },
  "currently_deploying": "HireSync → production",
  "availability": "IMMEDIATE",
  "open_to": ["Backend Internships", "Full-time SDE"]
}
```

<br clear="right"/>

---

## `GET /v1/architecture` — how I'm built

> Not a skill list. This is the actual request path through everything I've shipped.

```mermaid
flowchart LR
    C([Client]) --> LB{{Express Router}}
    LB --> AUTH[Auth Layer<br/>JWT · Passport · bcrypt · RBAC]
    AUTH --> CORE[Core Services<br/>Node.js · REST · MVC]
    CORE --> CACHE[(Redis<br/>cache + sessions)]
    CORE --> DB[(MongoDB Atlas<br/>Mongoose ODM)]
    CORE --> SQL[(MySQL<br/>relational workloads)]
    CORE --> RT[Socket.IO<br/>real-time events]
    CORE --> MEDIA[Cloudinary / ImageKit<br/>Multer pipelines]
    CORE --> MAIL[Nodemailer<br/>transactional mail]
    RT --> C
    CACHE -.hit.-> CORE
    MEDIA --> CDN([CDN Delivery])

    style AUTH fill:#1f6feb,stroke:#3fb950,color:#fff
    style CORE fill:#161b22,stroke:#3fb950,color:#3fb950
    style CACHE fill:#DC382D,stroke:#fff,color:#fff
    style DB fill:#47A248,stroke:#fff,color:#fff
```

<div align="center">

<img src="https://skillicons.dev/icons?i=nodejs,express,mongodb,redis,mysql,js,cpp,git,github,postman,vscode,linux&theme=dark" />

</div>

---

## `GET /v1/services` — deployed & running

<table>
<tr><th>Service</th><th>What it does</th><th>Status</th></tr>
<tr>
  <td><b>HireSync</b></td>
  <td>Unified campus + off-campus recruitment platform</td>
  <td><img src="https://img.shields.io/badge/shipping-3fb950?style=flat-square&labelColor=0d1117"/></td>
</tr>
<tr>
  <td><b>SoundWave</b></td>
  <td>Production-grade music streaming API backend</td>
  <td><img src="https://img.shields.io/badge/live-1f6feb?style=flat-square&labelColor=0d1117"/></td>
</tr>
</table>

<br/>

<img align="right" width="340" src="https://user-images.githubusercontent.com/74038190/218863487-e6c6f8f0-1dba-46ca-8d30-dbe6fe6f6c1d.gif"/>

### 🏢 HireSync — Unified Recruitment Platform

> **Picture a final-year student.** 12 tabs open — Internshala, LinkedIn, Naukri, the college portal, three WhatsApp groups, and 847 unread emails.
> Their dream placement is somewhere in that mess.
> **They will never see it.**

```diff
- Opportunities scattered across 10+ platforms
- Campus drives buried in Gmail threads
- Zero unified view of applications
+ One platform. Every opportunity. Zero missed deadlines.
```

<details>
<summary><b>▸ Engineering breakdown</b> — click to expand</summary>

<br/>

| Subsystem | Implementation |
|---|---|
| **Access control** | 4 roles (Candidate · Recruiter · TPO · Admin), every route gated by RBAC middleware |
| **Resume pipeline** | PDF upload → parse → automatic skill extraction → indexed profile |
| **Campus drives** | Structured drive lifecycle replacing ad-hoc Gmail threads |
| **Bulk onboarding** | Excel/CSV ingestion so TPOs onboard entire batches in one shot |
| **Real-time layer** | Socket.IO push notifications on deadlines and status changes |
| **Matching** | Skill-vector job recommendations against the extracted resume profile |
| **Analytics** | Drive metrics, funnel tracking, application-state dashboards |
| **Performance** | Redis caching on hot read paths, indexed Mongo queries |

**Stack** — `Node.js` `Express` `MongoDB` `Redis` `Socket.IO` `JWT` `Cloudinary` `Nodemailer` `Multer`

</details>

<a href="https://github.com/PriyankSaxenaa/Hiresync-backend"><img src="https://img.shields.io/badge/Read_the_code-3fb950?style=for-the-badge&logo=github&logoColor=0d1117&labelColor=0d1117"/></a>

<br clear="right"/>

<br/>

<img align="left" width="300" src="https://user-images.githubusercontent.com/74038190/216655410-f0ea5f22-2c8c-4b1a-b778-34b0b2e94fe8.gif"/>

### 🎵 SoundWave — Music Streaming Backend

> A Spotify-inspired API built to prove one thing: clean, secure, scalable REST design under real constraints.

<details>
<summary><b>▸ Engineering breakdown</b> — click to expand</summary>

<br/>

| Subsystem | Implementation |
|---|---|
| **Auth** | Stateless JWT sessions, hashed credentials |
| **Roles** | Artist vs User — separate permission surfaces on shared resources |
| **APIs** | Full CRUD for Songs & Albums with pagination and filtering |
| **Media** | ImageKit-backed uploads with Multer streaming and optimization |
| **Design** | Strict MVC separation, RESTful contracts, predictable error shapes |

**Stack** — `Node.js` `Express` `MongoDB` `JWT` `ImageKit` `Multer`

</details>

<a href="https://github.com/PriyankSaxenaa/SoundWave"><img src="https://img.shields.io/badge/Read_the_code-1f6feb?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117"/></a>

<br clear="left"/>

---

## `GET /v1/benchmarks` — problem solving

<img align="right" width="320" src="https://user-images.githubusercontent.com/74038190/238200428-67f477ed-6624-42da-99f0-1a7b1a16eecb.gif"/>

```
┌───────────────────────────────────────────────────┐
│  BENCHMARK RESULTS                    700+ RUNS   │
├───────────────────────────────────────────────────┤
│  LeetCode      priyanksaxenaa01        1700+  ⭐  │
│  Codeforces    priyank___saxena     1214 Pupil 🏁 │
│  Total solved  all platforms             700+  🧩 │
├───────────────────────────────────────────────────┤
│  Strongest:   Graphs · DP · Binary Search         │
│  Drilling:    DP optimization · Advanced graphs   │
│  Language:    C++  (fallback: JavaScript)         │
└───────────────────────────────────────────────────┘
```

🥈 **2nd Place** — Intercollege Ideathon

<br clear="right"/>

---

## `GET /v1/changelog`

```
v3.0  ▸  HireSync — 4-role platform, real-time layer, Redis caching
v2.5  ▸  Crossed 700 DSA problems · LeetCode 1700+
v2.0  ▸  SoundWave — first production-grade API backend
v1.5  ▸  Codeforces Pupil · 2nd place, Intercollege Ideathon
v1.0  ▸  First line of C++. Never stopped.
```

<details>
<summary><b>▸ /v1/incidents</b> — things that broke, and what I learned</summary>

<br/>

| Incident | Root cause | Fix | Takeaway |
|---|---|---|---|
| Slow job feed | Unindexed Mongo queries on every request | Compound indexes + Redis cache layer | Measure before optimizing — the DB tells you where it hurts |
| Notification storms | Socket events emitted per-write, unbatched | Batched emits + room-scoped broadcasts | Real-time ≠ every-time |
| Resume parse failures | Assumed uniform PDF structure | Defensive parsing + graceful fallbacks | User input is always weirder than your test file |

*Real engineering is mostly debugging. I'd rather show that than hide it.*

</details>

---

## `GET /v1/roadmap`

```mermaid
gantt
    title Now → Next
    dateFormat YYYY-MM
    axisFormat %b
    section Ship
    HireSync production deploy      :active, 2026-08, 2m
    section Depth
    System design · distributed sys :active, 2026-08, 4m
    Advanced graphs · DP optimization :2026-09, 3m
    section Goal
    Full-time SDE                   :crit, 2026-11, 3m
```

---

<div align="center">

## `GET /v1/metrics`

<img width="49%" src="https://github-readme-stats.vercel.app/api?username=PriyankSaxenaa&show_icons=true&hide_border=true&bg_color=0d1117&title_color=3fb950&text_color=c9d1d9&icon_color=1f6feb&include_all_commits=true&count_private=true"/>
<img width="49%" src="https://streak-stats.demolab.com?user=PriyankSaxenaa&hide_border=true&background=0d1117&stroke=161b22&ring=3fb950&fire=3fb950&currStreakLabel=3fb950&sideLabels=c9d1d9&dates=8b949e"/>

<img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PriyankSaxenaa&layout=compact&hide_border=true&bg_color=0d1117&title_color=3fb950&text_color=c9d1d9&langs_count=8"/>

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=PriyankSaxenaa&bg_color=0d1117&color=3fb950&line=1f6feb&point=ffffff&area=true&hide_border=true"/>

<img width="98%" src="https://github-profile-trophy.vercel.app/?username=PriyankSaxenaa&theme=onestar&no-frame=true&no-bg=true&column=7&margin-w=8"/>

<img width="98%" src="https://raw.githubusercontent.com/PriyankSaxenaa/PriyankSaxenaa/output/snake.svg" alt="contribution snake"/>

</div>

---

<div align="center">

## `POST /v1/hire`

</div>

```js
const evaluate = (role) => {
  const wantsBackend = role.stack.some(t =>
    ["node", "express", "mongodb", "redis", "system-design"].includes(t)
  );

  if (wantsBackend && role.type === "SDE") {
    return {
      status: 200,
      response: "Let's talk. I ship, I debug, and I don't need hand-holding.",
      responseTime: "< 6 hours",
      contact: "priyank0saxena@gmail.com"
    };
  }

  return { status: 200, response: "Still interested — I learn fast." };
};
```

<div align="center">

| Endpoint | SLA | Status |
|---|---|---|
| Recruiter email | `< 6h` | 🟢 |
| Take-home assignment | `< 48h` | 🟢 |
| Notice period | `0 days` | 🟢 |

<br/>

<a href="https://www.linkedin.com/in/priyank---saxena/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0d1117"/></a>
<a href="mailto:priyank0saxena@gmail.com"><img src="https://img.shields.io/badge/priyank0saxena@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0d1117"/></a>

<br/><br/>

<img src="https://user-images.githubusercontent.com/74038190/212284087-bbe7e430-757e-4901-90bf-4cd2ce3e1852.gif" width="70"/>

> ### *"Build skills so strong that opportunities chase you."*

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:3fb950,50:1f6feb,100:0d1117&height=140&section=footer&text=connection%20closed%20%C2%B7%20200%20OK&fontSize=18&fontColor=ffffff&fontAlignY=72&animation=fadeIn" width="100%"/>

</div>
