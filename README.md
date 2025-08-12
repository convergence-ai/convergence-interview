# Convergence Take-Home Test

## 🚀 Your Task

Your goal is to build a deep research agent that can help users answer questions using the [Pokémon API](https://pokeapi.co/). The agent should be able to gather deep information, reason through the problem, and return a useful and rich response.

This task is designed to reflect the kind of work you'd be doing on our team: figuring out the shape of the problem, making technical decisions under ambiguity, and learning as you go. There’s no single correct answer—we’re interested in **how you approach the problem**, not just whether you “finish” it.

### 🧭 Expectations

Your submission should include:
1. A working application or cli that allows interaction with your agent.
2. An agent you implemented yourself (not just calling an agent library).
3. Well-organised code.
4. A README with instructions on how to set up and run your app.

### Agent Design

The agent should:
1. Reason and plan how it will solve the user's query.
2. Gather information from the Pokémon API, multiple times as needed.
3. Conduct multiple iterations of research and problem solving as needed.

Your README should outline the main agent design and your thought process.

### Evaluation

Prioritize completing all of the above before you move on to "improving" your agent and making its outputs better.

Once you have a working agent, make sure to play around with your agent and inspect its outputs. Find out what's actually working well or not and iterate. If you don't know much about Pokemon, you can ask ChatGPT to evaluate the response for quality and it can point out recommendations or issues.

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
```
