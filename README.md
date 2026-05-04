# AI Code Documentation Standards 🚀

A strict, language-agnostic set of standards designed to stop AI coding assistants (like Cursor, Kiro, and Claude Code) from generating noisy, obvious, and redundant code comments.

## The Problem
By default, LLMs tend to over-explain code, leaving behind meta-comments like `# Added validation` or narrating obvious operations like `# Increment the counter`. This pollutes the codebase and reduces readability.

## The Solution
This repository provides a set of core principles that forces the AI to:
1. Write **English-only** comments.
2. Focus on the **"Why, not the What"** (intent and business logic).
3. Use strict, language-specific formatting (e.g., Sphinx for Python, XML for C#).
4. Eliminate dead code instead of commenting it out.

## How to Use

### For Cursor Users
1. Copy the `.cursorrules` file from this repository.
2. Paste it into the root directory of your project.
3. Cursor will automatically apply these standards in your next prompt.

### For Kiro / Claude Code Users
1. Copy the contents of `CLAUDE_GUIDELINES.md`.
2. Add it to your project's custom instructions or system prompt settings.

## Contributing
Contributions are welcome! If you want to add support for another programming language or refine existing rules:
1. Fork the project.
2. Create your feature branch.
3. Open a Pull Request (PR).

> **Note:** All PRs require review and approval before merging.

## License
Distributed under the MIT License. See `LICENSE` for more information.
