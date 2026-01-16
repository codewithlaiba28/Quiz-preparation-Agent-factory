Yeh image **Agent Factory ke "Skills are progressively disclosed"** concept ko dikha raha hai, jo **Panaversity ke Agent Native book/docs** mein detail se bayan kiya gaya hai. Main ne book ke preface aur related sections ko research kiya (jaise SKILL.md structure, sub-skills, aur progressive disclosure), aur ab Roman Urdu mein step-by-step samjhaata hoon.

### Pehla, Image ka Breakdown:
Image mein **Anthropic ke brand styling skill** ka example hai, jo yeh bata raha hai ke skills **progressively disclose hoti hain** — yani step-by-step khulti hain, jaise zarurat pade.

1. **Left side: anthropic/brand_styling/SKILL.md**  
   Yeh **main SKILL.md file** hai, jo skill ka overall specification deta hai. Isme:  
   - **Name/Description**: Anthropic Brand Style Guidelines — colors aur typography ke rules.  
   - **Overview**: Yeh bataata hai ke yeh skill Anthropic ke official brand resources ko PowerPoint presentations mein apply karne ke liye hai.  
   - **Colors**: Specific hex codes diye gaye, jaise Dark (#141413), Light (#fa9f5), Black Gray (#e6e6dc).  
   - **Usage Tip**: Jab presentations ya documents banate ho, to specific sub-files read karo, jaise /slide-decks.md ya /docs.md.  

   Yani yeh **top-level skill file** hai jo overview deta hai, lekin poora detail nahi — detail sub-files mein hai.

2. **Right side: Sub-skills (slide-decks.md aur docs.md)**  
   - **slide-decks.md**: Yeh sub-skill hai jo **slide decks (PowerPoint)** ke liye rules batata hai. Misal:  
     - Intro/Outro slides ka background color #141413.  
     - Section slides ka foreground color oat.  
     - Aur mazeed details.  
   - **docs.md**: Yeh **documents** ke liye rules, jaise har document title se shuru ho, authors ki list, creation date, etc. Aur GDocs mein tabs use karne ke tips.  

   Arrow se connect hai, jo bata raha hai ke main SKILL.md se sub-skills tak jaao.

3. **Title: Skills are progressively disclosed**  
   Yeh core idea hai — skills ek baar mein sab kuch nahi batati; balki **layer by layer disclose hoti hain** jaise agent ko zarurat pade.

### Ab, Yeh Book (Agent Native Docs) ke Mutabiq Kya Matlab Hai?
Book mein (preface-agent-native section) skills ko **portable, monetizable assets** kaha gaya hai jo AI agents ko domain expertise sikhate hain. Research se yeh points nikle:

- **Skills ki Structure**:  
  Har skill ek **folder** hoti hai, jisme:  
  - **SKILL.md**: Core file jo specification deta hai (jaise image mein overview aur colors). Yeh markdown format mein hota hai, jo AI agent ke liye "executable" hota hai — yani agent isko read karke action leta hai.  
  - **Sub-skills**: Jaise slide-decks.md ya docs.md — yeh specific parts cover karte hain. Book kehte hai ke skills **composable aur vertical** hote hain, yani chhote pieces mein banaye jaate hain jo combine ho sakte hain.  
  - **Scripts**: Jaise pehle image mein apply_template.py — yeh real code hota hai jo agent run karta hai.  

  Quote from book: "You must teach AI your domain expertise through the Teacher/Student/Co-Worker dynamic—encoding it into SKILL.md files that become portable, monetizable assets."

- **Progressively Disclosed Ka Matlab**:  
  Skills **step-by-step reveal hoti hain** — agent pehle main SKILL.md padhta hai (observation), phir samajhta hai (orientation), decide karta hai ke kon sa sub-skill use kare (decision), aur phir action leta hai (jaise script run kare). Yeh **iteration** ke through hota hai, taake errors correct ho sakein.  
  Book mein yeh **spec-driven development** pillar se linked hai: "Intent before implementation" — pehle overall spec do, phir progressively implement.  

  Misal book se: Jaise Digital SDR skill mein, agent pehle founder's brand voice padhta hai (SKILL.md), phir qualify leads (sub-skill), aur response draft karta hai. Same yahan: Brand styling mein pehle overview (SKILL.md), phir slide-decks.md se colors apply.

- **Agents Kaam Kaise Karte Hain?**  
  Book ke **Three-Role Partnership** mein:  
  1. **Teacher**: Human skill encode karta hai (SKILL.md banata hai).  
  2. **Student**: Agent seekhta hai progressively.  
  3. **Co-Worker**: Agent execute karta hai, jaise brand styling apply karke presentation update.  

  Yeh **Nine Pillars of AI-Native Development** pe based hai, jisme markdown ko "programming language" mana gaya hai, aur skills folders mein organize hote hain.

### Chhoti Summary Table (Book ke Concepts se):

| Concept                  | Book ke Mutabiq Matlab                  | Image mein Example                     |
|--------------------------|-----------------------------------------|----------------------------------------|
| SKILL.md                | Core spec file, expertise encode karta hai | Overview aur colors ke rules           |
| Sub-skills (e.g., slide-decks.md) | Specific details, progressively access  | Slide colors aur sections              |
| Progressive Disclosure  | Step-by-step reveal, iteration ke saath | Main file se sub-files tak jaana       |
| Folder Structure        | Markdown + scripts in folders           | anthropic/brand_styling/ folder        |

**Yeh idea revolutionary hai** kyunkay ab AI agents sirf instructions follow nahi karte — woh **progressively learn aur execute** karte hain, jaise real expert insaan. Book kehte hai ke yeh tareeqa se "Digital FTEs" banaye ja sakte hain, jo companies ke liye bohot useful hai. Agar mazeed detail chahiye, to pooch lo! 🚀