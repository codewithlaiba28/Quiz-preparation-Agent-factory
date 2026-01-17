## **AGENTS.md Kya Hai?**

**Definition:**
- Ek **markdown file** jo KISI BHI AI agent ko batati hai ke aapka project kaise kaam karta hai
- **Created by OpenAI**
- **Adopted by 60,000+ open source projects**
- Ab **AAIF open standard** (Dec 2025)

**Works with:**
- Claude Code
- Codex (OpenAI)
- Goose
- Cursor
- Copilot
- Any Agent

*"One file → Works with ALL AI coding agents"*

---

## **Agent-Specific Files**

Agent-specific files (jaise `CLAUDE.md`) **universal instructions** include kar sakti hain by referencing `@AGENTS.md`:

```markdown
# CLAUDE.md
@AGENTS.md

## Claude-Specific Features
- Tool permissions
- Extended context
```

**Key Point:**
- Universal guidelines **ek baar** `AGENTS.md` mein likho
- Reference with `@AGENTS.md` in any agent-specific file
- Koi duplication nahi!

---

## **Best Practice - Project Structure:**

```
your-project/
├── AGENTS.md           # Universal foundation (all agents)
├── @AGENTS.md          # Alternative notation (optional)
├── .claude/skills/     # Reusable capabilities
└── src/
```

**Three Layers:**

1. **AGENTS.md** = Universal foundation (sab agents ke liye)
2. **@AGENTS.md** = Alternative notation (same thing, optional)
3. **.claude/skills/** = Reusable capabilities

---

## **Key Concepts:**

💎 **AGENTS.md** = Universal project context (ek baar likho)

📎 **@AGENTS.md** = Reference it from any agent-specific file

✨ **Works everywhere. No duplication. No hassle.**

---

## **Agent Factory Book ke Mutabiq:**

### **1. Universal Standards (Book ka Core Message):**

Agent Factory book emphasize karti hai ke **agent-native development** mein **portability** aur **standards** zaroori hain:

```
Traditional Approach:
- Copilot ke liye alag instructions
- Claude ke liye alag instructions  
- Cursor ke liye alag instructions
❌ Duplication, maintenance nightmare

Agent-Native Approach (AGENTS.md):
- Ek universal file
- Sab agents samajhte hain
✅ Write once, works everywhere
```

### **2. Separation of Concerns:**

Book mein **layered architecture** ka concept hai:

**Layer 1 - Universal (AGENTS.md):**
- Project structure
- Coding standards
- General guidelines
- Works with ALL agents

**Layer 2 - Agent-Specific (CLAUDE.md, etc.):**
- Tool permissions
- Extended context
- Agent-specific features
- References @AGENTS.md

**Layer 3 - Capabilities (Skills):**
- Reusable functions
- Procedural knowledge
- `.claude/skills/`

### **3. AAIF Standard:**

Book mention karti hai ke **AAIF (Agent-AI Interoperability Framework)** ek open standard hai jo agents ko standardize karta hai. AGENTS.md ab is standard ka official part hai!

**Benefits:**
- **Vendor lock-in nahi** - Kisi bhi agent ko switch kar sako
- **Community-driven** - 60,000+ projects already use kar rahe
- **Future-proof** - Naye agents bhi support karenge

---

## **Practical Example:**

### **Pehle (Without AGENTS.md):**

```
.copilot-instructions.md:
"Use TypeScript, follow ESLint rules, test with Jest..."

.cursor/rules:
"Use TypeScript, follow ESLint rules, test with Jest..."

CLAUDE.md:
"Use TypeScript, follow ESLint rules, test with Jest..."
```

❌ **Problem:** Same instructions 3 baar likhe! Agar change karna ho?

---

### **Ab (With AGENTS.md):**

```markdown
# AGENTS.md (Universal)
- Use TypeScript
- Follow ESLint rules  
- Test with Jest
- API docs at /docs/api

# CLAUDE.md (Claude-specific)
@AGENTS.md

## Claude Features
- Use extended context for large files
- Enable MCP tools

# .copilot/instructions (Copilot-specific)
@AGENTS.md

## Copilot Features
- Inline suggestions enabled
```

✅ **Faida:** Universal guidelines ek jagah. Agent-specific sirf unique features!

---

## **Real-World Use Case:**

### **Scenario:** Aap ek web app bana rahe ho

**AGENTS.md:**
```markdown
# Project: E-commerce Platform

## Tech Stack
- Next.js 14 with App Router
- TypeScript (strict mode)
- Tailwind CSS
- Prisma ORM

## Code Standards
- Use functional components
- Prefer server components
- API routes in /app/api/

## Testing
- Unit tests with Vitest
- E2E with Playwright

## Database
- Schema in /prisma/schema.prisma
- Migrations before deploy
```

**CLAUDE.md:**
```markdown
@AGENTS.md

## Claude-Specific
- Use web search for latest Next.js docs
- Create artifacts for new components
- Use .claude/skills/ for common patterns
```

**CURSOR.md:**
```markdown
@AGENTS.md

## Cursor-Specific
- Enable Copilot++ for autocomplete
- Use Cmd+K for AI edit
```

---

## **Agent Factory Vision:**

Book ka vision hai:

### **Before (Fragmented):**
```
Each tool has own format
├── .github/copilot-instructions.txt
├── .cursor/rules.json
├── .aider.conf.yml
└── CLAUDE.md
```
❌ Maintenance nightmare!

### **After (Unified):**
```
One universal standard
├── AGENTS.md  ← Universal truth
├── CLAUDE.md  ← References @AGENTS.md  
└── .cursor/rules ← References @AGENTS.md
```
✅ Single source of truth!

---

## **60,000+ Projects Already Using:**

AAIF standard report karta hai:
- GitHub par 60,000+ repositories
- Open source community rapidly adopting
- Industry momentum

**Why?**
- Simple (sirf ek markdown file)
- Universal (sab agents samajhte hain)
- Maintained easily

---

## **Book Quote (Paraphrased):**

> "Agent-native development mein **portability** key hai. AGENTS.md ensure karta hai ke aapka project documentation kisi bhi agent ke saath kaam kare - vendor lock-in nahi, maximum flexibility."

---

## **Comparison with Skills:**

| Feature | AGENTS.md | Skills |
|---------|-----------|--------|
| **Purpose** | Project-level instructions | Reusable capabilities |
| **Scope** | Entire codebase | Specific tasks |
| **Format** | Single markdown | Multiple files + scripts |
| **Usage** | One per project | Many per project |

**Both Together:**
```
AGENTS.md: "Yeh project kaise kaam karta hai"
Skills: "Yeh specific tasks kaise karte hain"
```

---

## **Tashbeeh (Analogy):**

**AGENTS.md = Company Handbook:**
- Universal rules sab employees ke liye
- Ek baar likho, sab follow karte hain
- New hire? Handbook do, samajh jayega

**Agent-Specific Files = Department Guidelines:**
- Marketing ka apna style guide
- Engineering ki apni practices
- But dono Company Handbook follow karte hain

**Skills = Standard Operating Procedures:**
- Specific tasks ke detailed steps
- Reusable across departments

---

## **Summary:**

🎯 **AGENTS.md = Universal project instructions**

📝 Write once, works with ALL AI coding agents

🔗 Reference with @AGENTS.md to avoid duplication

⚡ 60,000+ projects already using

🚀 AAIF open standard - future of agent-native development

**Agent Factory Book Message:** Standards like AGENTS.md enable true agent-native development where your project works seamlessly with any AI tool! 🌟