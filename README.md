
# dotai / .ai

`dotai` is a self-improving AI system designed to track errors and learnings, creating better context-aware interactions in your project.

## Features
- **Codex (codex.md)**: Logs mistakes and learnings.
- **Learn Protocol (learn.md)**: Updates the Codex after corrections.
- **Split-Codex**: Categorizes Codex into manageable sections.
- **Session Management**: Keeps project context across sessions.

## Setup Instructions

1. **Clone this repo** or use as a template.
2. **Create a `.ai` folder** in a new or existing project:
   ```bash
   mkdir .ai
   ```
3. **Move all files** from the cloned repo into `.ai`.

## Usage Workflow

1. **Run Prompt**: Interact with the AI.
2. **Error**: If AI makes a mistake, correct it by invoking learn.md.
3. **Invoke Learn**: Enter `@learn.md @codex.md` to update Codex.
4. **Manage Codex**: Use `@split-codex` to categorize entries.

## Additional Steps

- Create a Composer/Notepad project named 'Codex' and add `codex.md` to the project context for persistent project memory without needing explicit learn.md mentions.


# dotai (improved readme)

`dotai` is a system for AI self-improvement designed to enhance project development by logging errors and learnings and providing contextual awareness across sessions.

## Features
- **Codex**: A repository that tracks AI errors and learnings (`codex.md`).
- **Session Management**: Maintains project memory across interactions (`start-session.md` and `end-session.md`).
- **Blueprints**: Guides for setting up various tech stacks. (by @mckaywrigley)
- **Snippets**: Code templates to streamline AI's code generation. They help in writing shorter prompts for better results.

## Installation (existing project)

1. **Clone this repository** or use it as a template.
2. **Create a `.ai` folder** in your existing project:
   ```bash
   mkdir .ai
   ```
3. **Move the contents of this repo into the `.ai` folder**.

## How to Use

1. **Start a session**: Add `start-session.md` to the `.ai` folder to maintain AI memory across interactions.
2. **Update Codex**: The AI will log errors and learnings automatically in `codex.md`.
3. **Use Snippets**: Add code snippets using `create-snippet.md` to enhance AI’s coding suggestions.
4. **Manage Codex Growth**: Use `split-codex.md` to categorize learnings for scalability.

## Example Workflow

1. **Test with a Prompt**: Ask the AI for help with a prompt.
2. **Error or Correction**: If the AI makes a mistake, correct it, and it will update `codex.md` to learn from it.
3. **Session Continuity**: Continue the project with improved AI context and fewer repeated mistakes.

### Important Note

[codex.md](codex/codex.md) should be added to the context of every chat:

- For regular chats: Use the plus button at the top of the chat to add the file.
- For Composers: Add the file to a Project Composer so all Composers created in that project will automatically have the file.

### Structure

The [Codex](codex/codex.md) is divided into two main sections:

1. Errors: Mistakes made and how to prevent them.
2. Learnings: Insights gained and their applications.

Each entry includes context, description, correction/application, and related entries.

## Snippets

Snippets include code templates that AI can use to generate or refactor code. They help in writing shorter prompts for better results.

- [create-snippet.md](snippets/create-snippet.md): Prompt for creating new snippets

## Session

- [start-session.md](session/start-session.md): Initiates a new AI session
- [end-session.md](session/end-session.md): Concludes the current AI session

Session files create a "memory layer" for the AI across multiple interactions, enabling contextual awareness and adaptive assistance.

Key benefits:

- Maintains project context between sessions
- Reduces repetition of project details
- Provides consistent guidance aligned with project direction

Usage:

1. End a session: Use [@end-session](session/end-session.md) command
2. Start a new session: Use [@start-session](session/start-session.md) command

The AI will generate and read status files in [status](status) to maintain project continuity.

## Blueprints

Blueprints are comprehensive guides for implementing specific technical architectures or project setups. They provide step-by-step instructions for installing, configuring, and integrating various technologies to create a functional foundation for your project.

- [supabase-drizzle-actions.md](blueprints/supabase-drizzle-actions.md): Backend architecture with Supabase, Drizzle ORM, and Server Actions
- [flux-with-replicate.md](blueprints/flux-with-replicate.md): Image generation using Flux and Replicate

## Libraries

- [lib](lib): Contains documentation examples for library usage

## Plugins

### v0

- [v0.dev](https://v0.dev/) is a tool for generating React components from screenshots and chat. Currently, they don't have a Cursor plugin, so you can use [v0](v0/v0.md) bridging prompt.
- [v0.md](v0/v0.md): Guide for using v0.dev to generate component ideas and prompts

## Rules of AI

[Rules](rules) contains rules for default AI behavior and interaction. These rules are meant to be added to the global "Rules of AI" setting.

## Contributing

This is an open-source template. Contributions are welcome! Please add a changelog entry with your contribution.

## Note

This system is designed for AI consumption. Entries should prioritize precision and relevance over human readability

