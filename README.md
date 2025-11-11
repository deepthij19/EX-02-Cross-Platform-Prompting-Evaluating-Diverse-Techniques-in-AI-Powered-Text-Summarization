# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

# 1. Aim

To evaluate and compare the effectiveness of four prompting techniques — Zero-Shot, Few-Shot, Chain-of-Thought, and Role-Based prompting — in performing text summarization tasks across multiple AI platforms: ChatGPT, Claude, Gemini, and Copilot.
The goal is to determine which combination of prompting style and AI model produces the most coherent, concise, and contextually accurate summaries.

# 2. Scenario

A 300-word article about climate change impacts on agriculture is used as the input text. Each AI model is tasked with summarizing the same article using different prompting techniques. The results are evaluated using both quantitative (ROUGE, BLEU, BERTScore) and qualitative (coherence, fluency, factuality) metrics.

# 3. Algorithm / Methodology

| Step                   | Description                                                                       |
| ---------------------- | --------------------------------------------------------------------------------- |
| **1. Data Selection**  | A single standardized text (e.g., a news article or academic excerpt).            |
| **2. Prompt Design**   | Create four distinct prompts (Zero-Shot, Few-Shot, Chain-of-Thought, Role-Based). |
| **3. Model Selection** | ChatGPT, Claude, Gemini, Copilot.                                                 |
| **4. Execution**       | Run each prompt across each platform.                                             |
| **5. Evaluation**      | Compare outputs using human evaluation and automated NLP metrics.                 |
| **6. Analysis**        | Rank effectiveness and summarize findings.                                        |

# 4. Prompting Technique Examples

# A. Zero-Shot Prompt (ChatGPT Example)

Prompt:

“Summarize the following text in 100 words or fewer.”
[Insert article text]

Expected Output (ChatGPT):
ChatGPT produces a coherent and concise summary, capturing key ideas but occasionally missing nuanced details due to lack of context or examples.

# B. Few-Shot Prompt (Claude Example)

Prompt:

Example 1:
Text: “The iPhone launch drew huge crowds.”
Summary: “The iPhone launch attracted many people.”

Example 2:
Text: “Electric cars are reducing carbon emissions.”
Summary: “Electric vehicles help lower pollution.”

Now summarize the following text:
[Insert article text]

Expected Output (Claude):
Claude generates a fluent and contextually balanced summary, maintaining factual accuracy and style consistency. Few-shot improves alignment with desired summarization tone.

# C. Chain-of-Thought Prompt (Gemini Example)

Prompt:

“Let’s go step by step to summarize the key points of this text.

Identify the main topic.

Note supporting evidence.

Combine into a concise summary.”
[Insert article text]

Expected Output (Gemini):
Gemini provides a structured reasoning process, breaking down the passage and producing a logically sound summary. Occasionally slightly verbose but strong factual coverage.

# D. Role-Based Prompt (Copilot Example)

Prompt:

“You are a professional editor for a scientific journal. Your job is to produce a precise, well-structured summary of the following article for publication.”
[Insert article text]

Expected Output (Copilot):
Copilot produces a formal and polished summary with high linguistic fluency but may slightly underrepresent minor details due to style constraints.

# 5. Final Analysis:

| Technique            | Model   | Strengths                       | Weaknesses                        | Overall Effectiveness |
| -------------------- | ------- | ------------------------------- | --------------------------------- | --------------------- |
| **Zero-Shot**        | ChatGPT | Fast, generalizable             | Misses context, inconsistent tone | ★★★☆☆                 |
| **Few-Shot**         | Claude  | Balanced tone, accurate         | Requires examples                 | ★★★★☆                 |
| **Chain-of-Thought** | Gemini  | Logical, factual                | Sometimes verbose                 | ★★★★☆                 |
| **Role-Based**       | Copilot | Professional tone, high fluency | May omit nuances                  | ★★★☆☆                 |


# 6. Most Effective Combination:

Few-Shot prompting with Claude and Chain-of-Thought prompting with Gemini yield the most accurate and coherent summaries overall.

Claude (Few-Shot): Best balance of brevity, coherence, and fidelity.

Gemini (CoT): Best structured reasoning and fact retention.

# 7. Conclusion:

The evaluation demonstrates that prompt design significantly influences summarization quality across AI platforms.

Zero-Shot is efficient but less precise.

Few-Shot improves contextual alignment.

Chain-of-Thought enhances reasoning and factual accuracy.

Role-Based offers stylistic refinement.

The optimal strategy combines Few-Shot learning (for example-driven clarity) with Chain-of-Thought reasoning (for logical coherence) — forming a hybrid approach for advanced summarization performance.

# Result:

Few-Shot and Chain-of-Thought prompting give the best theoretical performance. Few-Shot ensures accuracy and coherence through examples, while Chain-of-Thought enhances logical flow and factual depth. Zero-Shot is basic but limited, and Role-Based adds polish but may miss details.
