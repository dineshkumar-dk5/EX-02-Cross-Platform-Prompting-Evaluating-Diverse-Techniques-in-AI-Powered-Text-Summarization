

# **EX-02 – Cross-Platform Prompting: Evaluating Diverse Techniques in AI-Powered Text Summarization**

---

### **AIM**

* To compare the **effectiveness of multiple prompting strategies** in improving AI-generated summaries.
* To identify which **AI platform** is most suitable for summarizing technical articles for undergraduate learners.
* To analyze trade-offs between **speed, accuracy, and simplicity** in real-world use cases.
* To build a **benchmark framework** for evaluating summarization tasks across AI tools.
* To understand how **prompt engineering impacts final output quality**.

---

### **SCENARIO**

* Task: Summarize a **500-word technical article** on *“The Basics of Blockchain Technology.”*

* Context: Part of an **educational platform** that provides short, student-friendly research summaries.

* **Evaluation Criteria**:

  1. **Accuracy** – Does the summary capture blockchain fundamentals (ledger, decentralization, immutability)?
  2. **Coherence** – Is the explanation logically ordered?
  3. **Simplicity** – Can undergraduates grasp it easily?
  4. **Speed** – How quickly is the summary produced?
  5. **User Experience** – How easy is it to design prompts?

* Platforms tested: **ChatGPT, Gemini, Claude, Copilot**.

* Prompting Techniques: **Zero-shot, Few-shot, Chain-of-thought, Role-based**.

---

### **ALGORITHM**

1. **Input Preparation**

   * Collect the blockchain article.
   * Preprocess text (remove noise, ensure clarity).

2. **Define Prompting Techniques**

   * **Zero-shot**: Direct request, no examples.
   * **Few-shot**: Provide 2–3 examples of summaries.
   * **Chain-of-thought**: Ask AI to reason stepwise before summarizing.
   * **Role-based**: Assign role (e.g., “Act as a teacher for undergraduates”).

3. **Platform Execution**

   * Run the same input text on **ChatGPT, Gemini, Claude, Copilot**.
   * Apply each prompting technique separately.

4. **Data Collection**

   * Save outputs in structured format.
   * Record **time taken per response**.

5. **Evaluation Metrics**

   * Assign **scores (0–5)** for Accuracy, Coherence, Simplicity, Speed, User Experience.
   * Example:

| Platform | Prompt Type      | Accuracy | Coherence | Simplicity | Speed | UX | Overall |
| -------- | ---------------- | -------- | --------- | ---------- | ----- | -- | ------- |
| ChatGPT  | Role-based       | 5        | 5         | 5          | 4     | 5  | 24/25   |
| Claude   | Chain-of-thought | 5        | 4         | 3          | 3     | 4  | 19/25   |
| Gemini   | Few-shot         | 4        | 4         | 4          | 3     | 4  | 19/25   |
| Copilot  | Zero-shot        | 3        | 3         | 3          | 5     | 3  | 17/25   |
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/60482444-2879-4de0-b92b-2ccd6d6dd44f" />
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/56e9297f-9ebb-48cd-a2d7-1187a5f80e70" />

6. **Analysis**

   * Compare results → Identify best combination.
   * Note advantages & weaknesses of each technique.

---

### **RESULT**

* **ChatGPT + Role-based prompting** produced the **best overall summaries** – clear, accurate, simple, and student-friendly.
* **Claude + Chain-of-thought** was highly **accurate and detailed**, but less simple for undergraduates.
* **Gemini + Few-shot** performed **moderately well** but was slower compared to others.
* **Copilot + Zero-shot** was **fastest** but lacked depth and coherence.
* **Key Insight:** Prompting style **directly influences summary quality** – structured prompts (role-based, few-shot) outperform plain zero-shot.
* **Conclusion:** For educational content creation, **ChatGPT (role-based)** is the most effective tool.

---

