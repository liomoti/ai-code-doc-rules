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

Navigate to the folder corresponding to your AI assistant:

### 🖱️ Cursor
1. Go to the `Cursor/` folder in this repository.
2. Copy the `.cursorrules` file.
3. Paste it directly into the root directory of your project.

### 🧠 Claude Code
1. Go to the `Claude/` folder.
2. Copy the contents of the `CLAUDE.md` file.
3. Paste the rules into your project's `CLAUDE.md` file at the root directory.

### 🛠️ Amazon Q Developer (Kiro)
1. Go to the `Kiro/` folder.
2. Copy the `documentation-standards.md` file.
3. Place it in your project under the `.kiro/steering/` directory.

## Contributing
Contributions are welcome! If you want to add support for another programming language or refine existing rules:
1. Fork the project.
2. Create your feature branch.
3. Open a Pull Request (PR).
# Note: Keep in mind that core rule updates must be applied across all tool-specific folders.

## License
Distributed under the MIT License. See `LICENSE` for more information.