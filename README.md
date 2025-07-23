# Convergence Take-Home Test

This is a skeleton project for the Convergence take-home test. The project is set up with Docker to make development and testing consistent across different environments.

## 🚀 Your Task

Your goal is to build a deep research agent that can help users answer questions using the [Pokémon API](https://pokeapi.co/). The agent should be able to gather deep information, reason through the problem, and return a useful and rich response.

This task is designed to reflect the kind of work you'd be doing on our team: figuring out the shape of the problem, making technical decisions under ambiguity, and learning as you go. There’s no single correct answer—we’re interested in **how you approach the problem**, not just whether you “finish” it.

### 🧭 Scope and Expectations

At a minimum, your submission should include:
- A working application that allows some form of interaction with your agent.
- An agent that you implemented yourself (not just calling an agent library).
- The ability to gather information from the Pokémon API to help answer the user’s input.
- Basic code organization and a README with instructions on how to run your app.

These are the foundations—we recommend you **prioritize completing and polishing these before considering anything else**.

Once you’ve built the foundation, ask yourself:

- How can the agent reason more effectively before jumping to an answer?
- What is deep research, how to make an agent **deep** ?
- How does it decide when the task is “done” and ready to respond?
- Would a simple UI help demonstrate the agent’s functionality more clearly?
- Can your README help others understand your thought process?

### 🧠 Questions Worth Exploring (Optional, But Encouraged)

If you feel confident in your core implementation, you’re welcome to explore deeper challenges. Rather than prescribe tasks, here are some prompts to help guide your thinking:

- What if your agent forgets something important it previously discovered? How could you help it “remember” context across steps?
- Could a planning step help the agent approach problems more systematically?
- How can we speed up the deep research process?
- How would the agent handle vague or underspecified inputs? 
- How can we store the sessions and messages to allow users to revisit past interactions?
- Is there a way to evaluate whether your agent is doing a good job?

You don’t need to implement all—or even any—of these. But if you choose to explore one, we’d love to see your thinking reflected in the code or README.

---


## Getting Started with Docker

### Prerequisites

- Docker
- Docker Compose

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


## Project Structure

```
convergence-interview/
├── src/                    # Source code
│   └── main.py            # Main application entry point
├── tests/                 # Test files
├── requirements/          # Python dependencies
├── Dockerfile             # Docker image configuration
├── docker-compose.dev.yaml # Development Docker Compose
└── Makefile              # Common development commands
```

## Development

- All Python dependencies are managed through the `requirements/` directory
- The project uses Docker for consistent development environments
- If you want to add tests, put them in the `tests/` directory
- Implement your solution in the `src/` directory


We’re less concerned with what tools or architecture you pick, and more interested in how you make decisions, how you learn through the process, and how you communicate what you’ve built. If something doesn't work as planned, that’s fine—just tell us what you tried, what you learned, and where you'd take it next.

Good luck! We’re excited to see how you approach this.

Feel free to write your own README.md to explain your approach and any additional features you implemented.
```