# dotai / .ai

`dotai` is a self-improving AI system designed to track errors and learnings, creating better context-aware interactions in your project.

## Features

- **Codex (codex.md)**: Logs mistakes and learnings.
- **Learn Protocol (learn.md)**: Updates the Codex after corrections.
- **Split-Codex**: Categorizes Codex into manageable sections.
- **Session Management**: Keeps project context across sessions.
- **Blueprints**: Guides for setting up various tech stacks.
- **Snippets**: Code templates to streamline AI's code generation.

## Installation

1. **Clone this repository** or use it as a template.
2. **Create a `.ai` folder** in your existing project:
   ```bash
   mkdir .ai
   ```
3. **Move the contents of this repo into the `.ai` folder**.

## Usage Workflow

1. **Run Prompt**: Interact with the AI.
2. **Error Correction**: If AI makes a mistake, correct it by invoking Learn.
3. **Invoke Learn**: Enter `@learn.md @codex.md` to update Codex.
4. **Manage Codex**: Use `@split-codex` to categorize entries when needed.
5. **Persistent Memory Setup**: 
   - Create a Composer/Notepad project named 'Codex'.
   - Add `codex.md` to the project context for persistent project memory without needing explicit `learn.md` mentions.

### Important Note: Adding Codex to Chat Context

`codex.md` should be added to the context of every chat:

- For regular chats: Use the plus button at the top of the chat to add the file.
- For Composers: Add the file to a Project Composer so all Composers created in that project will automatically have the file.

This ensures that the AI has access to all logged errors and learnings for each interaction.

## Session Management

Session files create a "memory layer" for the AI across multiple interactions, enabling contextual awareness and adaptive assistance.

### Key Benefits:
- Maintains project context between sessions
- Reduces repetition of project details
- Provides consistent guidance aligned with project direction

### Usage:
1. **Start a session**: Use `@start-session` command
   - `start-session.md`: Initiates a new AI session

2. **End a session**: Use `@end-session` command
   - `end-session.md`: Concludes the current AI session

The AI will generate and read status files in the `status` directory to maintain project continuity.

## Codex Structure

The [Codex](codex/codex.md) is divided into two main sections:

1. Errors: Mistakes made and how to prevent them.
2. Learnings: Insights gained and their applications.

Each entry includes context, description, correction/application, and related entries.

## Snippets

Snippets include code templates that AI can use to generate or refactor code:

- Use [create-snippet.md](snippets/create-snippet.md) to create new snippets.

## Blueprints

Comprehensive guides for implementing specific technical architectures:

- [supabase-drizzle-actions.md](blueprints/supabase-drizzle-actions.md): Backend with Supabase, Drizzle ORM, and Server Actions
- [flux-with-replicate.md](blueprints/flux-with-replicate.md): Image generation using Flux and Replicate

## Additional Components

- **Libraries**: [lib](lib) contains documentation examples for library usage.
- **Plugins**: [v0](v0/v0.md) provides a guide for using v0.dev to generate component ideas and prompts.
- **Rules**: [Rules](rules) contains rules for default AI behavior and interaction.

## Contributing

This is an open-source template. Contributions are welcome! Please add a changelog entry with your contribution.

## License

[Include license information here]

