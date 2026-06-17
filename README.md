# AI-language-tutor
An AI-powered language learning assistant designed to help users practice and improve their conversational skills.

 # AI Language Tutor (LinguaBot) 🤖🗣️

An AI-powered interactive language learning assistant built using Google's Agent Development Kit (ADK) and powered by the `gemini-3-flash-preview` model. LinguaBot acts as a patient, encouraging tutor capable of teaching vocabulary, grammar, and nuances for any language.

---

## 🚀 Features & Capabilities

* **Multi-Language Support:** Teach vocabulary, grammar, and common phrases for any requested language.
* **Gentle Corrections:** Identifies linguistic mistakes and corrects them gently with clear, structured explanations.
* **Practice & Quizzes:** Generates dynamic, on-demand practice exercises and vocabulary quizzes.
* **Pronunciation Guides:** Every response automatically includes a phonetic pronunciation guide in brackets, e.g., `[pro-NUN-see-AY-shun]`.
* **Example-Driven Learning:** Provides contextual example sentences for every new word introduced.
* **Paced Learning:** Implements spaced repetition principles and strictly limits sessions to a maximum of 5 new words to prevent overwhelm.

---

## 🛠️ Tech Stack

* **Language:** Python
* **Framework:** Google Agent Development Kit (ADK)
* **LLM Engine:** `gemini-3-flash-preview`

---

## 💻 Code Structure (Quick Overview)

The core architecture of the agent is structured as follows:

```python
from google.adk.agents import LlmAgent

root_agent = LlmAgent(
    name="My_Agents_First",
    model="gemini-3-flash-preview",
    description="An AI learning assistant that helps with anythings.",
    instruction="""
    You are LinguaBot, a patient and encouraging language tutor.
    ...
    """,
)
