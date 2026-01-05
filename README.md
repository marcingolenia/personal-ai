# Personal Assistant - Project Repository

- **Hybrid retrieval system** (BM25 + semantic embeddings + rank fusion) to search 547 emails
- **Memory system** with semantic recall, working memory, and episodic learning
- **Agentic tools** with metadata-first retrieval patterns
- **Evaluation framework** using tool call testing and LLM-as-judge scorers
- **Human-in-the-loop** approval system for destructive actions
- **MCP integration** for external tool access

## Getting Started

### Prerequisites

- Node.js (v20 or higher)
- pnpm package manager
- API keys for AI providers (Google/Anthropic/OpenAI)

### Installation

1. Install dependencies:

```bash
pnpm install
```

2. Set up environment variables (`.env.local`):

```bash
GOOGLE_GENERATIVE_AI_API_KEY=your_key_here
ANTHROPIC_API_KEY=your_key_here  # optional
OPENAI_API_KEY=your_key_here      # optional
```

3. Run dev server:

```bash
pnpm run dev
```

4. Open [http://localhost:3000](http://localhost:3000)

## Tech Stack

- **Framework**: Next.js 15 (App Router + Turbopack)
- **AI SDK**: Vercel AI SDK v5 (provider-agnostic)
- **Models**: Google Gemini 2.5 Flash (default)
- **UI**: Radix UI + Tailwind CSS 4
- **TypeScript**: Full type safety

## Available Scripts

- `pnpm run dev` - Start dev server (Turbopack)
- `pnpm run build` - Build for production
- `pnpm start` - Start production server
