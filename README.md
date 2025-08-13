# Convergence Take-Home Test

## 🚀 Your Task

Your goal is to build a Deep Research agent that can answer questions about Pokemon. The agent should be able to use tools to gather information, reason through the problem, and return a useful response.

### 🧭 Expectations

Your submission should include:
1. A working application or cli that allows interaction with your agent.
2. An agent you implemented yourself (not just calling an agent library).
3. Well-organised code.
4. A README with instructions on how to set up and run your agent.

### Agent Design

The agent should:
1. Reason and plan how it will solve the user's query.
2. Gather information from the Pokémon API, multiple times as needed.
3. Conduct multiple iterations of research and problem solving as needed.

Your README should outline the main agent design and your thought process.

### Evaluation

Prioritize completing all of the above. Then begin to iterate on your agent to improve its outputs, perhaps by tweaking the tools or prompts or overall agent design.

Make sure to play around with your agent and inspect its outputs. Find out what's actually working well or not. If you don't know much about Pokemon, you can ask ChatGPT to evaluate the response for quality and it can point out recommendations or issues.

---

## Getting Started on this Template Repo

### Prerequisites

- Docker
- Docker Compose

### Development Setup

Feel free to use your own setup. The below explains how this template repository works.

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

Feel free to make your own structure.

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

There is no expectation to write tests.
