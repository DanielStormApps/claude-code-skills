# Claude Code Skills

A collection of reusable skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Installation

Copy the `skills/` folder to your project's `.claude/` directory:

```bash
cp -r skills/ /path/to/your/project/.claude/skills/
```

Or copy individual skills as needed.

## Available Skills

| Skill | Description |
|-------|-------------|
| `/list-ideas` | List all ideas in the ideas folder |
| `/initial-prompt` | First prompt for exploration (no code editing) |
| `/write-plan` | Write a new plan in plans folder |
| `/review-plan` | Review plan against codebase |
| `/next-phase` | Reply with next phase steps |
| `/do-phase` | Implement a phase and commit |
| `/execute-full-plan` | Implement all phases in a plan |
| `/complete-plan-and-merge` | Move plan to completed, merge to develop, cleanup branch |

## Usage

After installation, invoke skills in Claude Code using the slash command syntax:

```
/list-ideas
/write-plan Add user authentication
/do-phase Phase 1
```

## Project Structure Assumptions

These skills assume a project workflow with:

- `ideas/` - Directory for idea markdown files
- `plans/` - Directory for implementation plans
- `plans/completed/` - Directory for completed plans
- `develop` - Main development branch

## License

This project is released under the MIT License. See the [LICENSE](https://github.com/DanielStormApps/claude-code-skills/blob/main/LICENSE) file for more information.
