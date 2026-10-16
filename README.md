# Build a Multi-Agent Book Writer

A Python project that demonstrates a **multi-agent system** for writing
books. Several LLM-powered crews collaborate on a single book:

- **Outline crew** — researches the topic and produces an outline
- **Writer crew** — expands the outline chapter by chapter
- **Review/consistency checks** — catch contradictions between chapters
- An LLM server runs the whole pipeline and exposes tools to the crews

The full flow is orchestrated by the commands in `book_flow/`.

## Tech stack

- Python 3.10+
- LLM APIs accessed through a central LLM server
- Async/await based orchestration
- YAML configuration for agents, crews, and tasks

## Running

```bash
python -m src.book_writing_flow.main
```

See `.env.example` for required environment variables.
