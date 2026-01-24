## 🧠 **Perfect Agent Spec — Part 2 (Book ke Mutabiq)**

Book kehti hai ke **spec sirf role, context, aur logic tak nahi rukta**.
Ek **high-value agent** tab banta hai jab **success trigger, output standard, aur error handling** clear likhe gaye hon.

---

## 4️⃣ **The Success Trigger (SKILL.md ka “Trigger”)**

Ye step define karta hai **kab agent apni skill ko activate kare**.

### 🔹 **Keywords**

* Specific phrases ya signals define karo
* Example:

  * “Audit this transaction” → Claude bolta hai: *“I have a skill for this”*

📌 Book ke mutabiq:

> “Trigger ke bina agent randomly ya galat kaam karega.”

---

### 🔹 **File Types**

* Agent ko batao **kaunse files par kaam kare**
* Example: `.pdf`, `.csv`, `.json`

📌 Book ka logic:

> “Agent sirf relevant data pe kaam kare, baki ignore kare”

* Efficiency barh jati hai
* Errors kam hoti hain

---

## 5️⃣ **The Output Standard (Standardization)**

Agent ko sirf kaam complete karna nahi, **consistent aur useful output** dena hai.

### 🔹 **Template**

* Final result ka structure define karo:

  * Markdown
  * JSON schema
* Example:

  ```json
  {
    "lead_name": "",
    "score": "",
    "next_action": ""
  }
  ```

### 🔹 **Reporting**

* User ko notify kaise kare
* Example:

  * “Post a summary to #finance-alerts in Slack”
  * Ya email / dashboard

📌 Book ke mutabiq:

> “Agent ka kaam tabhi valuable hai jab output **predictable aur standardized** ho.”

---

## 6️⃣ **The Error Protocol**

Book kehti hai: **Reliable agent wo hai jo problem solve kar sake**.

### 🔹 **Fallback**

* Agar MCP tool down ho ya data missing ho
* Agent ko define karo kya karna hai
* Example:

  * Retry 3 times
  * Notify human
  * Skip aur continue

📌 Book ka lesson:

> “Errors aur downtime ka plan Spec mein hona chahiye,
> warna agent chaos create karega.”

---

## 🎯 **Book ka Core Message (Part 2 Blueprint)**

* **Success Trigger** = kab agent skill use kare
* **Output Standard** = kaise kaam ka result present kare
* **Error Protocol** = failure ke time kya kare

Agar ye teen cheezein clear ho →

* Agent **predictable**,
* **reliable**,
* **senior-level skill** wala ban jata hai

---

## 🧩 **One-Line Book Style Conclusion**

**Spec ka final section decide karta hai:
Agent kab active ho,
kaise output de,
aur error par kya kare —
ye teen cheezein hi agent ko professional banati hain.**
