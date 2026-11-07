<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b1e3d,50:1F8ACB,100:FFA116&height=200&section=header&text=Priyank%20Saxena&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=Backend%20Engineer%20%C2%B7%20Competitive%20Programmer%20%C2%B7%20ICPC%20Regionalist&descSize=17&descAlignY=60" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=19&duration=3000&pause=900&color=1F8ACB&center=true&vCenter=true&width=760&height=40&lines=Microservices+%C2%B7+Multi-Agent+AI+%C2%B7+AWS+CI%2FCD;900%2B+DSA+problems+solved;Final-year+CS+student.+Open+to+SDE+roles." />

<br/>

<img src="https://img.shields.io/badge/ICPC-Asia%20West%20Regionalist%202026-C8102E?style=for-the-badge"/>
<img src="https://img.shields.io/badge/LeetCode-1788-FFA116?style=for-the-badge&logo=leetcode&logoColor=white"/>
<img src="https://img.shields.io/badge/Codeforces-Pupil%201312-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white"/>
<img src="https://img.shields.io/badge/DSA-900%2B-3fb950?style=for-the-badge"/>

</div>

<br/>

> **B.Tech CSE (Data Science), GLBITM · Batch 2027.** I design and ship backend systems end to end: microservices, real-time features, caching, payments, AI agent pipelines and cloud deployment. I also compete in algorithmic contests.

---

<div align="center">

## 🏆 Contest Record

</div>

<table>
<tr>
<td align="center" width="25%">
<h1>🌏</h1>
<b>ICPC Regionalist</b><br/>
<sub>Asia West Amritapuri Regional<br/>Jan 1–2, 2027 · Bengaluru</sub>
</td>
<td align="center" width="25%">
<h1>⭐ 1788</h1>
<b>LeetCode</b><br/>
<sub>Peak rating in<br/>live contests</sub>
</td>
<td align="center" width="25%">
<h1>🏁 1312</h1>
<b>Codeforces</b><br/>
<sub>Pupil · actively<br/>competing</sub>
</td>
<td align="center" width="25%">
<h1>🧩 900+</h1>
<b>Problems Solved</b><br/>
<sub>LeetCode · GFG ·<br/>Codeforces</sub>
</td>
</tr>
</table>

<div align="center">
<sub>🥇 Top 2 in my institute on the CP-31 sheet &nbsp;·&nbsp; 🥈 Runner-Up, Intercollege Ideathon (team lead of 5)</sub>
</div>

---

<div align="center">

## 🛠️ Tech Stack

</div>

<table>
<tr>
<td width="18%"><b>Languages</b></td>
<td><img src="https://skillicons.dev/icons?i=cpp,c,js,mysql&theme=light" /></td>
</tr>
<tr>
<td><b>Backend</b></td>
<td><img src="https://skillicons.dev/icons?i=nodejs,express&theme=light" /> &nbsp;<sub>REST · Microservices · MVC · JWT · RBAC · Socket.IO</sub></td>
</tr>
<tr>
<td><b>Databases</b></td>
<td><img src="https://skillicons.dev/icons?i=mongodb,redis&theme=light" /> &nbsp;<img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square"/></td>
</tr>
<tr>
<td><b>AI Engineering</b></td>
<td><img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/> <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge"/> <img src="https://img.shields.io/badge/RAG-6f42c1?style=for-the-badge"/></td>
</tr>
<tr>
<td><b>Cloud & DevOps</b></td>
<td><img src="https://skillicons.dev/icons?i=docker,aws,githubactions&theme=light" /> &nbsp;<sub>ECS · ECR · S3 · CloudFront</sub></td>
</tr>
<tr>
<td><b>Tools</b></td>
<td><img src="https://skillicons.dev/icons?i=git,github,postman,firebase,vscode&theme=light" /></td>
</tr>
</table>

---

<div align="center">

## 💼 Projects

</div>

### 🤖 Gyaani AI &nbsp;<img src="https://img.shields.io/badge/Microservices-1F8ACB?style=flat-square"/> <img src="https://img.shields.io/badge/Multi--Agent%20AI-6f42c1?style=flat-square"/> <img src="https://img.shields.io/badge/Demo-paused%20(low%20API%20credits)-orange?style=flat-square"/>

**The problem:** Different AI tasks need different tools. One model is good at chatting, another at reading PDFs, another at writing code. Switching between apps wastes time, and one overloaded service can slow everything down.

**What I built:** One AI assistant that understands what you're asking and hands it to the right specialist agent. Drop in a PDF and it answers strictly from that document. Ask for code, search, or a generated document and a different agent picks it up. Underneath, it's split into independent services for login, chat, billing, and the AI agents, with credits, payments, and fair-use limits built in. Every change I push is built, packaged, and deployed to the cloud automatically.

```mermaid
flowchart LR
    U([User]) --> CF[CloudFront + S3<br/>Frontend]
    CF --> GW[API Gateway]
    GW --> AU[Auth]
    GW --> CH[Chat]
    GW --> BL[Billing]
    CH --> AG[Agent Service<br/>LangGraph router]
    AG --> A1[Chat · Search · Code<br/>PDF Q&A · Vision · Docs]
    AG --> VDB[(Qdrant)]
    GW --> RD[(Redis)]
    CH --> DB[(MongoDB)]
```

<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square"/>
<img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/Razorpay-0C2451?style=flat-square&logo=razorpay&logoColor=white"/>
<img src="https://img.shields.io/badge/Firebase%20Auth-FFCA28?style=flat-square&logo=firebase&logoColor=black"/>

<a href="https://d2nd94qbszkbeq.cloudfront.net/"><img src="https://img.shields.io/badge/🌐%20Live%20Demo-1F8ACB?style=for-the-badge"/></a>

<br/>

### 🎓 HireSync &nbsp;<img src="https://img.shields.io/badge/LIVE-3fb950?style=flat-square"/> <img src="https://img.shields.io/badge/Real--time-FFA116?style=flat-square"/>

**The problem:** A final-year student hunting for a job has opportunities scattered across ten different websites, WhatsApp groups, and a flooded email inbox. Good chances get missed simply because nobody saw them.

**What I built:** One website that pulls every opportunity into a single place. Students, recruiters, and college placement officers each get their own view. Everyone gets alerted the moment something changes, so nothing gets missed.

<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white"/>
<img src="https://img.shields.io/badge/JWT%20%2B%20RBAC-000000?style=flat-square&logo=jsonwebtokens&logoColor=white"/>
<img src="https://img.shields.io/badge/REST%20APIs-1F8ACB?style=flat-square"/>
<img src="https://img.shields.io/badge/MVC-6f42c1?style=flat-square"/>
<img src="https://img.shields.io/badge/Cloudinary-3448C5?style=flat-square&logo=cloudinary&logoColor=white"/>

<a href="https://myhiresync.vercel.app/"><img src="https://img.shields.io/badge/🚀%20Live%20Demo-3fb950?style=for-the-badge"/></a>
<a href="https://github.com/PriyankSaxenaa/Hiresync-backend"><img src="https://img.shields.io/badge/View%20Code-181717?style=for-the-badge&logo=github&logoColor=white"/></a>

---

<div align="center">

## 📈 GitHub Activity

<img width="47%" src="https://github-readme-stats.vercel.app/api?username=PriyankSaxenaa&show_icons=true&hide_border=true&theme=nord&include_all_commits=true&count_private=true"/>
<img width="47%" src="https://streak-stats.demolab.com?user=PriyankSaxenaa&hide_border=true&theme=nord"/>

<br/><br/>

**Open to SDE internships and full-time roles** · 📧 priyank0saxena@gmail.com

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FFA116,50:1F8ACB,100:0b1e3d&height=110&section=footer" width="100%"/>

</div>
