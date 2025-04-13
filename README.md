# Panel-of-AI-Minds

A simulated panel of AI minds that generates a roundtable discussion — including critique, consensus, and synthesis — from a single user prompt.

## 🧠 What is this?

**Panel-of-AI-Minds** is an experimental framework built using Google's Generative AI tools (Gemini), simulating a thoughtful conversation among diverse AI personas. Each AI agent represents a unique worldview (scientific, spiritual, ethical, etc.), responds to a complex question, critiques the others, and helps generate a cohesive, multi-perspective dialogue.

Inspired by recursive reasoning and pluralistic design, the project demonstrates how generative AI can go beyond content creation to simulate deliberation, ethical review, and dialogic intelligence.

## 💡 Core Features

- **Persona-driven prompting** — Agents like a scientist, ethicist, and visionary respond in-character.
- **Simulated RAG** — Context is added to each agent’s response for grounding.
- **LLM-based Peer Review** — Agents rate each other on clarity, accuracy, bias, ethics, and morality.
- **Top-agent selection** — The best-reviewed voices are chosen for synthesis.
- **Natural conversation synthesis** — Final dialogue is rewritten in human-style markdown.
- **Modular code** — Each stage can be extended or run independently.

## 🎯 Use Cases

- Ethical deliberation and AI alignment studies  
- Narrative generation and simulation  
- Educational demos in AI ethics or prompting techniques  
- Research into multi-agent systems and recursive evaluation

## 📂 Structure

- `agent_profiles`: Defines agent personas and the moderator
- `generate_agent_prompts()`: Creates persona-specific prompts
- `simulate_rag()`: Adds contextual knowledge per agent
- `call_gemini()`: Generates output using Gemini 2.0 Flash
- `llm_peer_review()`: Agents evaluate each other’s responses
- `summarize_reviews()`: Aggregates scores across review dimensions
- `select_top_agents()`: Picks the best 3 agents
- `synthesize_final_response()`: Combines top answers into a report
- `rewrite_transcript_as_conversation()`: Transforms output into a human-like panel transcript

## 🔧 Requirements

- Python 3.10+  
- Google Generative AI SDK (Google AI Studio) with generated API key 
- Anaconda Jupyter Notebook or Kaggle notebook environment
- Optional: Google Text-to-Speech API for audio synthesis

## 🚀 Quickstart

After running through the notebook with persona and function deifinitions, to run the full pipeline from your own single prompt use:

```python
topic = "Could AGI arrive sooner than we think?"
panel_discussion_transcript = run_full_panel_simulation(topic)
Markdown(panel_discussion_transcript)
```

