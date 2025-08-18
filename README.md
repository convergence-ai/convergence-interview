# Convergence Take-Home Test

## 🚀 Your Task

Your goal is to build a Deep Research agent that can answer questions about Pokemon. The agent should be able to reason through the task, use tools to gather information, and return a useful response.

### 🧭 Expectations

Your submission should include:
1. A simple command line client or working application.
2. An agent you implemented yourself (not just calling an agent library).
3. Well-organised code that is easy to review.
4. A README with instructions on how to set up and run your agent.

### Agent Design

The agent should:
1. Reason and plan how it will solve the user's query.
2. Gather information from the Pokémon API, calling tools multiple times as needed.
3. Conduct multiple rounds of thinking and acting as needed.

We recommend you start simple and slowly expand your agent.

Your README should outline your final agent design, including the steps the agent takes and what sort of tools it has.

### Evaluation

Once things are working end-to-end (your agent can reason and call tools), begin to iterate on your agent.

Start out by trying a few simple tasks for your agent. If things don't work yet, try even simpler tasks (break the tasks down even more, or add extra information in your query: "Use the get_pokemon tool to return data about Pikachu").

It's important to see what your agent is able to do. Then try to figure out what's missing. You can try to improve its outputs, perhaps by adding new tools, fixing existing tools, or improving your system prompting.

Do make sure to play around with your agent and read its outputs. If you don't know much about Pokemon, you can ask ChatGPT to evaluate the response for quality and it can point out recommendations or issues.

---

## Getting Started on this Template Repo

Feel free to use your own setup. The below explains how this particular template repository works.

### Prerequisites

- Docker

### Development Setup

1. **Build and run the development environment:**

   ```bash
   make build
   ```
   then
   ```bash
   make start
   ```
2. **Add dependencies once in docker container:**
   Add new libraries in requirements/dev.in

   then

   ```bash
   make deps
   ```

## Default Project Structure

Feel free to adjust and design your own structure.

```
convergence-interview/
├── src/                    # Source code with agent code
│   └── main.py             # Main application entry point (CLI)
├── tests/                  # Test files
├── requirements/           # Python dependencies
├── Dockerfile              # Docker image configuration
├── docker-compose.dev.yaml # Development Docker Compose
└── Makefile                # Common development commands
```

There is no expectation to write tests. It might help to isolate API behaviour to ensure the tools work correctly.
