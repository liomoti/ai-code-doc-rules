# AI Code Documentation Standards 🚀

A strict, language-agnostic set of standards designed to stop AI coding assistants from generating noisy, obvious, and redundant code comments.

## The Problem
By default, LLMs tend to over-explain code, leaving behind meta-comments like `# Added validation` or narrating obvious operations like `# Increment the counter`. This pollutes the codebase and reduces readability.

## The Solution
This repository provides a set of core principles that forces the AI to:
1. Write **English-only** comments.
2. Focus on the **"Why, not the What"** (intent and business logic).
3. Use strict, language-specific formatting (e.g., Sphinx for Python, XML for C#).
4. Eliminate dead code instead of commenting it out.

## How to Install & Use

### For AWS Kiro
1. Copy the `kiro-steering.md` file from this repository.
2. Place it in your project under the `.kiro/steering/` directory.
3. The file automatically includes the `--- inclusion: always ---` frontmatter so Kiro will always enforce it.

### For Visual Studio (GitHub Copilot)
1. Copy the `copilot-instructions.md` file.
2. Place it in a `.github/` directory at the root of your workspace (i.e., `.github/copilot-instructions.md`).

### For Claude Code
1. Copy the `CLAUDE.md` file.
2. Place it in the root directory of your project. Claude Code will read it automatically at the start of every session.

### For Cursor
1. Copy the `.cursorrules` file.
2. Paste it into the root directory of your project.

## Contributing
Contributions are welcome! If you want to add support for another programming language or refine existing rules:
1. Fork the project.
2. Create your feature branch.
3. Open a Pull Request (PR).
