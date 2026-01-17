**Agent Skills Ecosystem - Industry Adoption (December 2025)**

**Left Side - Adoption Table:**

| **Agent** | **Vendor** | **Support Level** | **Directory Format** | **Status** |
|-----------|-----------|------------------|---------------------|------------|
| Claude Skills | Anthropic | ✅ Native | .claude/skills/SKILL.md | Production (Oct 2025) |
| Codex CLI | OpenAI | ✅ Beta | .codex/skills/SKILL.md | Beta (Dec 2025) |
| Goose | Block (Square) | ✅ Adopted | .claude/skills/ + .goose/skills/ | Production (2025) |
| Gemini CLI | Google | ⚠️ Under Review | — | Issue #7986 |
| Oven Code | Alibaba | 🔶 F1 Roadmap | — | Issue #365 |

**Key Points:**
- Claude Skills **production mein hai** - fully ready!
- OpenAI ka Codex CLI beta testing mein
- Goose ne adopt kar liya (Square/Block company ka)
- Google aur Alibaba abhi review/roadmap stage mein

**Right Side - SKILL.md Format Specification:**

```markdown
name: skill-name
description: One-line description for agent discovery

# Skill Title

## When to Use
Trigger conditions and use cases.        ~100 tokens

## Instructions  
Step-by-step guidance for the agent.    Progressive
                                        Disclosure
## Examples
Concrete examples of correct behavior.

## References
See REFERENCE.md/REFERENCE.md for detailed docs.
See EXAMPLES.md/EXAMPLES.md for more examples.
```

**File Structure:**
```
.claude/skills/my-skill/
├── SKILL.md          # Entry point (~100 tokens at start)
├── REFERENCE.md      # Loaded on-demand (0 tokens until needed)
├── EXAMPLES.md       # Loaded on-demand (0 tokens until needed)
└── scripts/
    └── helper.py     # EXCLUDED, never loaded (0 tokens always)
```

**Agent Factory Book ke Mutabiq:**

**Progressive Disclosure** - Book mein emphasize hai ke skills efficiently load honi chahiye:
- Pehle sirf SKILL.md ka summary load ho (~100 tokens)
- Jab zaroorat ho tab detailed docs load karein
- Helper scripts kabhi load nahi hote (0 tokens)
- Yeh **token efficiency** ke liye critical hai

**Industry Standard:**
Book kehti hai ke **agent-native development** ka matlab hai:
- Ek baar skill likho, har agent par chalaao
- Standard format sab samajhte hain
- Skills portable hain (vendor lock-in nahi)

**Bottom Line:**
"Claude Skills format industry standard ban raha hai. Skills ek baar likhi jaati hain aur multiple agents par kaam karti hain."

**Faida:**
Developers ko har platform ke liye alag se likhna nahi padega - ek skill sab jagah chalegi! Yeh exactly wohi vision hai jo Agent Factory book present karti hai.