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
| `/complete-plan-and-merge` | Move plan to completed, merge to develop, cleanup branch |
| `/do-phase` | Implement a phase and commit |
| `/execute-full-plan` | Implement all phases in a plan |
| `/initial-prompt` | First prompt for exploration (no code editing) |
| `/list-ideas` | List all ideas in the ideas folder |
| `/next-phase` | Reply with next phase steps |
| `/review-plan` | Review plan against codebase |
| `/write-plan` | Write a new plan in plans folder |

## Usage

After installation, invoke skills in Claude Code using the slash command syntax:

```
/write-plan Add user authentication
/do-phase Phase 1
/list-ideas
```

## Project Structure Assumptions

These skills assume a project workflow with:

- `plans/` - Directory for implementation plans
- `plans/completed/` - Directory for completed plans
- `ideas/` - Directory for idea markdown files
- `develop` - Main development branch

## License

MIT
