### Diagram ka Breakdown (Visual Explanation):
- **Center mein Agent** hai (beige box) — yeh **General Purpose Agent** hai (jaise Claude Code). Yeh reasoning karta hai, observe karta hai, decide karta hai, aur action leta hai (OODA loop: Observe → Orient → Decide → Act).
- Agent ke andar **red star** (✴️) aur **code icon** (</>) — yeh bata raha hai ke agent **code execute** karta hai aur **autonomous** hota hai.
- **Left side: Multiple MCP servers** (MCP server 1, 2, 3) — yeh green boxes hain jo agent se **double-headed arrows** se connected hain (↔). Yani **bidirectional communication** — agent inko call karta hai aur data/tools leta hai.
- **Right side: Filesystem** mein multiple **Skills** (purple boxes) — yeh agent ke file system mein stored hoti hain (jaise anthropic/brand_styling/SKILL.md waghera).
- **Curved arrows** (↺) agent ke andar — yeh **loop** dikha rahe hain: Agent continuously **MCP servers se data pull** karta hai, **Skills se expertise** use karta hai, aur phir **filesystem pe actions** perform karta hai (jaise files read/write, scripts run).

Yeh **closed loop system** hai jahan agent **real-time mein external world** (MCP via) aur **domain knowledge** (Skills via) se connect rehta hai.

### Book ke Mutabiq Yeh Complete Picture Kya Hai?

**General Purpose Agents** (jaise Claude Code) **universal reasoning machines** hote hain — woh kisi bhi domain mein kaam kar sakte hain, lekin **bina specialization ke generic** rehte hain.

Yeh do cheezon se **powerful domain-expert** ban jaate hain:

1. **MCP Servers** (Model Context Protocol):
   - Yeh **universal "USB for AI"** hain — open standard jo agent ko **real business data/tools** se connect karta hai.
   - Misal: CRM database, APIs, file systems, web browser, internal company data.
   - Agent MCP server ko call karta hai → live data fetch karta hai → uspe reasoning apply karta hai.
   - Book kehte hain: MCP bina agent sirf soch sakta hai, lekin **real world mein act nahi kar sakta**.

2. **Skills** (Composable Vertical Skills):
   - Yeh **domain expertise** ko encode karti hain — SKILL.md files mein (progressive disclosure ke saath).
   - Skills agent ko **sikhati hain ke kaise kaam karna hai** (procedures, best practices, style guides, workflows).
   - Misal: Brand styling skill colors batati hai, sales skill lead qualification criteria, legal skill contract review rules.
   - Agent filesystem se Skills read karta hai → unko **autonomously discover aur use** karta hai.

**Together ka Magic**:
- **MCP** → Agent ko **abilities deta hai** (data access, tools).
- **Skills** → Agent ko **intelligence deta hai** (kaise use karna hai un abilities ko professionally).
- Result: **General Purpose Agent → Specialized Digital FTE** (Full-Time Employee) ban jata hai jo 24/7 kaam karta hai, high accuracy ke saath (97%+ in tests).

### Key Book Concepts Jo Is Picture Mein Fit Hote Hain:
- **Spec-Driven Development**: Pehle intent/spec likho (Markdown mein), phir agent usko implement kare.
- **Three-Role Partnership**: Human (Teacher) Skills likhta hai → Agent (Student/Co-Worker) seekhta aur execute karta hai.
- **Nine Pillars** mein yeh teen important hain:
  - MCP Standard
  - Composable Vertical Skills
  - AI CLI & Coding Agents (General Purpose)

### Simple Summary Table:

| Component          | Kya Hai?                                   | Role in Picture                          | Book Quote/Insight                          |
|--------------------|--------------------------------------------|------------------------------------------|---------------------------------------------|
| General Purpose Agent | Reasoning engine (Claude Code etc.)       | Center, loop chalata hai                 | "General Agents BUILD Custom Agents"        |
| MCP Servers        | Data/tools connectors (universal protocol) | Left side, data provide karte hain       | "USB for AI tools" – real business data     |
| Skills             | Domain expertise files (SKILL.md)          | Right side, filesystem mein stored       | "Portable, monetizable assets"              |
| Loop (↺)           | Continuous interaction                     | Agent ko smart + connected banata hai    | Complementary: MCP + Skills = Domain power  |

**Yeh architecture revolutionary hai** kyunkay ab **non-developers** bhi Skills bana kar (apni expertise encode kar ke) General Purpose Agents ko **company-specific super-expert** bana sakte hain, aur MCP ke through real data se connect kar ke **real revenue-generating Digital FTEs** deploy kar sakte hain. Book ka yeh hi core message hai: "Your domain knowledge becomes an autonomous AI that never sleeps." 🚀
