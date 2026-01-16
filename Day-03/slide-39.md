## 📌 1. **Manual Prompting** — *Purani/Basic Approach*

**Manual Prompting** ka matlab hai:

* Aap bar-bar har turn mein manually instructions likhtay ho.
* Har baar prompt mein sari rules, context aur logic likhna padta hai.
* Yeh adhoc (best-effort) hota hai — kabhi accurate, kabhi nahin.
* Jab AI ko instructions dene hote hain, token cost har turn badhti hai kyunki sari rules har baar prompt mein repeat hotay hain.

**Summary (Roman Urdu):**
Manual Prompting ek **ad-hoc aur baar baar manual kaam** hai. Aap har baar prompt paste karte ho aur AI ko bataate ho kya karna hai. Instructions waste tokens generate kartay hain aur reuse mushkil hota hai.

**Example:**

> “AI, yeh rules follow kro: step1, step2, ... ab yeh kaam karo.”
> Har baar repeat.

👉 Token cost zyada
👉 Reliable nahin
👉 Reusable nahin

---

## 📌 2. **Agent Skills (`SKILL.md`)** — *Nayi/Structured Approach*

**Agent Skills** ka concept agent-native development ka core hai. Yeh ek structured file format hota hai (`SKILL.md`), jisme aap apni expertise ko define karte ho — jab use karna hai, kaise execute karna hai, aur output kaisa chahiye.

Book ke hisaab se skills **Intellectual Property (IP)** ban jati hain aur reusable assets hoti hain.  

**Key Points (Roman Urdu):**

* **Deterministic aur script-backed:** Agent Skills ek *script* ki tarah hoti hain jo AI agent ko batati hai *exactly* kya karna hai.
* **Reusable & Scalable:** Ek skill bar likh dene ke baad, woh har project mein reuse hoti hai.
* **Token Cost Efficient:** Skill sirf tab load hoti hai jab agent decide karta hai ke use karni hai — is se overall token cost bohat kam hoti hai.
* **Integration Ready:** Skills easily AI Agent SDKs (OpenAI, Claude etc.) mein integrate hoti hain.

**Example SKILL.md Structure:**

```
---
name: financial-analysis
description: Analyze financial statements ...
---
## When to Use
- User asks for analysis

## How to Execute
1. Gather docs
2. Extract metrics
3. Compare
4. Generate report

## Output Format
Summary + Table + Analysis
```

Yeh ek reusable expertise definition hai jo agent “activate” karega jab relevant kaam aaye.  

---

## 🆚 **Manual Prompting vs Agent Skills (Side-by-Side)**

| Feature            | **Manual Prompting**        | **Agent Skills (`SKILL.md`)**       |
| ------------------ | --------------------------- | ----------------------------------- |
| **Reliability**    | Ad-hoc / Best-effort        | Deterministic / Script-backed       |
| **Token Cost**     | Har turn instructions cost  | Only load when triggered (low cost) |
| **Asset Type**     | Disposable conversation     | Reusable, scalable IP               |
| **Integration**    | Needs human to paste prompt | API-ready via agents SDKs           |
| **Reuse**          | Nahi                        | Haan (bar-bar use)                  |
| **Productization** | Difficult                   | Easy (digital products)             |

📌 **Roman Urdu Explanation:**
Manual prompting shehzada prompt copy-paste karke AI ko bolta hai “yeh kaam kro.” Har baar sari instructions likhnay se cost zyada hoti hai aur repeat karna mushkil hota hai.
Agent Skills mein aap ne apni expertise ek file ke taur pe likh di — jasay ek *recipe* — jise agent kabhi bhi use kar sakta hai bina repeat likhay. Yeh scalable aur *product ready* approach hai.  

---

## 🧠 Summary (Roman Urdu)

**Manual Prompting:** simple par inefficient, baar baar instructions likhni padti hain aur AI reliable response nahi deta.

**Agent Skills:** structured, reusable, aur efficient. Aap apni expertise ko ek file (SKILL.md) mein define karte ho jo agent ko batati hai *jab aur kaise kaam karna hai*. Yeh modern AI development ka future hai, jahaan AI agents deterministic workflows follow karte hain aur business logic reusable hota hai.  
