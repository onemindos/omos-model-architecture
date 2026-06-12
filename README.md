# OneMind Model Architecture

An interactive, educational visualization of how AI models flow from **cloud providers** through **model APIs** to **coding agents** and finally into **autonomous systems**.

> Teaches people how to leverage models — one model, many doors.

## Live

Open `index.html` in any browser. No build step, no dependencies.

## Structure

```
index.html                    ← Hub: force-directed graph + deep-dive links
providers/
├── aws-bedrock.html          ← AWS Bedrock: models, IAM, boto3
├── azure.html                ← Azure AI: OpenAI Service, AD, deployments
├── google.html               ← Google Cloud: Vertex AI, AI Studio
├── digitalocean.html         ← DigitalOcean: GPU Droplets, GenAI
└── alibaba.html              ← Alibaba Cloud: DashScope, Qwen
models/
├── anthropic-claude.html     ← KEY: one model, 4+ provider doors
├── openai.html               ← GPT family, reasoning, multimodal
└── gemini.html               ← Natively multimodal, 1M context
agents/
└── index.html                ← 5 coding agents + orchestration hierarchy
```

## The 4 Layers

| Layer | What | Examples |
|-------|------|----------|
| **Providers** | Cloud infrastructure hosting models | AWS Bedrock, Azure, Google, DigitalOcean, Alibaba |
| **Models** | The intelligence | Claude, GPT, Gemini, Qwen, Ollama |
| **Coding Agents** | Tools that use models to write code | Claude Code, Codex, Copilot, OpenCode, Pi Agent |
| **Autonomous Systems** | Orchestrators that command everything | Hermes, OpenClaw |

## Key Insight

**One model can be accessed through many doors.**

Claude (for example) is available via:
- Anthropic Direct API (simplest, API key)
- AWS Bedrock (IAM auth, enterprise, no keys floating)
- Google Vertex AI (service account, GCP native)
- Azure AI Foundry (AD integration)
- GitHub Copilot (zero cost with subscription)

Same model, different billing, different auth, different trade-offs. Zero vendor lock-in.

## Tech

- Pure HTML/CSS/JS — single files, no framework, no build
- Canvas-based force-directed graphs (custom engine, no d3)
- Each page: interactive graph + code examples + comparison tables
- AgentTap HUD theme: Chakra Petch + IBM Plex Mono, dark slate

## Roadmap

- [ ] GitHub Pages deployment
- [ ] Video walkthrough for community
- [ ] Add Ollama/local inference detail page
- [ ] Add model comparison benchmarks
- [ ] Connect to capability tree (cross-link)
- [ ] Pricing calculator tool
- [ ] Keep model versions current as new releases ship

---

*OneMind Model Architecture — The Fabric Connects Us All*
