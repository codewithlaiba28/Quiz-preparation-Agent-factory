### Core Definition (left side of the slide)
> "Skills are **organized collections of files** that package **composable procedural knowledge** for agents"

This is the cleanest, most concise official explanation of what Agent Skills really are:

- They are **not** just long prompts
- They are **not** traditional tools/functions
- They are **structured folders** containing multiple files
- Their main purpose = packaging **procedural knowledge** (step-by-step know-how, workflows, best practices, style guides, templates etc.) in a way that is:
  - **composable** → can be combined/stacked with other skills
  - **reusable** → across projects, teams, even shared/sold
  - **on-demand** → Claude only loads the parts it actually needs (progressive disclosure)

This makes Claude behave much more like a **trained specialist coworker** instead of a general-purpose chatbot that needs to be reminded of procedures every single conversation.

### Typical Folder Structure (right side of the slide)
The slide shows a very common real-world pattern used in Anthropic's own skills (and recommended for custom ones):

```
anthropic_brand/           ← folder name = skill name (usually kebab-case or snake_case)
├── SKILL.md               ← **mandatory** main file — this is the entry point
│                            contains YAML frontmatter (name, description, when to trigger)
│                            + the core procedural instructions
├── docs.md                ← additional documentation / reference material
│                            (Claude reads this only when really needed)
├── slide-decks.md         ← specialized instructions just for creating/editing slide decks
│                            (again — only loaded on demand when making presentations)
└── apply_template.py      ← optional helper script
                             Claude can execute this when it needs to apply templates
                             (very common pattern for pptx/word/excel/pdf skills)
```

### How it actually works in Claude (very elegant design)
1. Claude gets the **skill name + short description** pre-loaded in system prompt (very cheap)
2. When the task matches → skill gets **activated**
3. Claude reads **SKILL.md** first (core instructions)
4. If the procedure says "when creating slides, also follow rules in slide-decks.md" → Claude dynamically reads that file too
5. Same for docs.md, templates, brand guides, etc.
→ This is called **progressive disclosure** — extremely token-efficient compared to dumping 20,000 tokens of instructions every time

### Connection with the Agent Factory book/course (panaversity)
The book https://agentfactory.panaversity.org/docs/preface-agent-native teaches almost exactly the **same philosophy**, but uses a slightly more general/educational framing:

- "Composable Vertical Skills — Reusable domain expertise"
- Skills encode procedural knowledge into **SKILL.md** files
- They become portable, monetizable assets
- Goal = turn human domain expertise into reliable, repeatable Digital FTEs (Full-Time Equivalents)

The Anthropic slide is basically showing the **concrete implementation detail** of that same idea in the Claude ecosystem (as of late 2025).

In short:  
The slide is teaching developers the **"how"** (real folder structure used by Anthropic)  
The Agent Factory book is teaching the **"why + bigger picture"** (agent-native development, composable skills as the future of building specialized AI workers).