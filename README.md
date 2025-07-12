# 🤖 CogVerse: A Decentralized Cognitive Metasystem for Multi-Agent AI Collaboration

**Author:** Md Ayan

CogVerse is an experimental architecture that simulates a society of intelligent AI agents who collaborate asynchronously via shared memory and an event-driven messaging system. The goal is to move beyond linear, tool-chaining agent frameworks like AutoGPT or BabyAGI and create a digital collective brain — where agents behave like independent but cooperating minds.

---

## 💡 What is CogVerse?

CogVerse is inspired by:

- Human cognitive societies (research labs, communities, brains)
- The limitations of centralized AI orchestration
- A need for systems where AI agents can evolve, delegate, reason, and negotiate dynamically

The architecture includes:

- Thought Mesh: a shared, vector-based long-term memory layer (powered by FAISS + OpenAI embeddings)
- Agent Personas: each agent has personality traits (creativity, skepticism, verbosity, etc.)
- Event Bus: agents subscribe to and react to topic-specific events
- Social Graph: agents track trust scores for each other, adapting roles accordingly
- Emergent Planning: agents negotiate tasks instead of following hardcoded sequences

---

## 🧠 How It Works

You define a topic like:  
`"Write a research paper on decentralized cognitive architectures"`

This triggers:

- `PlannerBot` → sets milestones, structure
- `ResearchBot` → fetches relevant papers using OpenAI
- `CritiqueBot` → evaluates quality, detects bias
- `VisionBot` → proposes creative extensions
- `WriterBot` → synthesizes final content

Agents write to the **Thought Mesh**, listen to the **Event Bus**, and score each other in the **Social Graph**.
docs/architecture_diagram.png.png
---
⚙️ System Components
agent.py: Defines the base Agent class and specialized agents like ResearchBot

persona.py: Controls personality traits for each agent (creativity, curiosity, skepticism)

event_bus.py: Pub/Sub model — agents listen and respond to events

thought_mesh.py: Long-term vector memory with semantic search (OpenAI + FAISS)

social_graph.py: Agents track reliability of others over time (trust scores)

main.py: Bootstraps the system and publishes an initial topic event

🧪 Sample Output
After running main.py, sample logs might look like:

text
Copy
Edit
[*] Topic: decentralized cognitive metasystems
[ResearchBot] Summary node added to memory
[WriterBot] New memory received, updating related work
[CritiqueBot] Low novelty detected, requesting new citations
[VisionBot] Proposed speculative architecture update
Dummy metrics stored in experiments/dummy_results.csv:

csv
Copy
Edit
metric,value
originality_pct,87.2
revision_convergence,2
contradiction_count,1
📌 Why It Matters
This isn't just automation. This is cognition.

Most frameworks chain tools.

CogVerse chains minds.

We’re building a digital brain — distributed, dynamic, democratic — one agent at a time.

Use it as:

A base for multi-agent research tools

A launchpad for real-time cognitive systems

A foundation for human-AI collaboration platforms

📬 Contributions Welcome
Want to build DebateBot, ProofBot, MetaAgent, or a HumanInTheLoopBot? Go for it.

Open an issue, fork the repo, or suggest improvements!

📜 License
MIT License – use, fork, build, remix freely with attribution.

🤝 Acknowledgements
Inspired by:

AutoGPT, BabyAGI, LangChain

Marvin Minsky’s “Society of Mind”

Biological cognitive networks

The dream of building collective machine intelligence

Made with 💻 + ☕ by Md Ayan



## 🔧 How To Use

### 1. Install Requirements

```bash
pip install -r requirements.txt
2. Set OpenAI API Key
bash
Copy
Edit
export OPENAI_API_KEY="your_api_key_here"
3. Run It
bash
Copy
Edit
python src/main.py
You'll see logs from agents writing to memory, reacting to each other, and forming a collaborative result.

```
