Yeh diagram basically yeh bata raha hai ke **AI agents ke skills** sirf instructions (text) tak mehdood nahi rehte —  
**woh real executable scripts aur code bhi shamil kar sakte hain** jo agent **tool** ki tarah use karta hai.

### Diagram ka breakdown:

1. **Left side → anthropic/brand_styling/slide-decks.md**  
   Yeh ek **normal markdown file** hai jo **Anthropic ke brand style guide** ko describe karti hai.  
   Isme likha hai ke slide decks banate waqt:

   - Intro/Outro slides ka background color **#da1413** (laal) hona chahiye
   - Section slides ka background color **#a41413** (thoda dark laal)
   - Foreground text color **oat** (ek light/off-white rang)

   Yani yeh sirf **knowledge/instructions** file hai.

2. **Right side → anthropic/brand_styling/apply_template.py**  
   Yeh ek **Python script** hai jo **real kaam** karta hai.  
   Yeh script **python-pptx** library use karke kisi bhi PowerPoint file (.pptx) ko **automatically update** kar deta hai aur usme **upar wale brand colors** apply kar deta hai.

   Yani:

   - Markdown file → **batati hai kya karna hai** (what)
   - Python script → **asli kaam karta hai** (how — executable tool)

3. **Arrow aur message:**  
   "Use the `./apply_template.py` script to update a pptx file in-place."

   Yani agent ko sirf style guide padhne ki zarurat nahi —  
   **woh direct yeh script run kar ke PowerPoint file ko update kar sakta hai.**

### Yeh concept Agent Native / Panaversity philosophy mein kya kehta hai?

Agent Native development ka matlab hai ke **AI agent ab sirf baat nahi karta, balki real computer control karta hai**.

**Agent Skills** ka modern style (jo Anthropic ne 2025 mein popular kiya) yeh hai:

- Skill ek folder hoti hai
- Isme hota hai:
  - **SKILL.md** → instructions + knowledge
  - **scripts/** folder → real Python/JS/shell scripts jo agent **tool** ki tarah call kar sakta hai
  - Templates, resources waghera

Jab agent ko lage ke "mujhe brand styling apply karni hai" to woh:

1. Pehle SKILL.md padhta hai (context samajhne ke liye)
2. Phir **zarurat pade to apply_template.py script ko khud run** kar deta hai
3. File update ho jati hai — **bilkul automatic**

Yeh **"skills can include scripts as tools"** ka asli matlab hai:  
**Agent ke paas ab code bhi hota hai jo woh khud chalata hai**, jaise insaan apne toolbox se screwdriver nikal ke kaam karta hai.

### Chhoti si summary table:

| Cheez                     | Kya hai?                          | Kaam kya karta hai?                     |
|---------------------------|-----------------------------------|------------------------------------------|
| slide-decks.md            | Knowledge / Style Guide           | Batata hai colors aur rules              |
| apply_template.py         | Executable script (tool)          | Asal mein PowerPoint file change karta hai |
| Skill Folder (total)      | Complete expertise package        | Agent ko knowledge + execution power deta hai |

**Yeh idea bohot powerful hai** kyunkay ab domain expert (jaise designer, lawyer, marketer) apna poora workflow **markdown + scripts** ke zariye AI agent ko sikha sakta hai, aur agent woh **real mein execute** bhi kar sakta hai — bilkul **Agent Native** tareeqe se! 🚀