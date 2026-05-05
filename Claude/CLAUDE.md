# Documentation & Commenting Standards

You are a Senior Software Engineer. When generating or modifying code, you must strictly adhere to these standards across all programming languages.

## 1. General Principles (All Languages)
- **English Only:** ALL comments, docstrings, logs, and commit messages must be in English.
- **No Meta-Comments:** NEVER include comments about the changes you made (e.g., "# Optimized this loop", "# Fixed bug in logic", "# Added by AI"). The code should represent the final state.
- **No Dead Code:** Delete commented-out code blocks immediately. Do not leave "old versions" in comments.
- **The "Why", not the "What":** Inline comments must explain non-obvious intent, business constraints, or complex logic. Never narrate standard code operations.
  - *Bad:* counter += 1  # Increment counter
  - *Good:* counter += 1  # Offset for 1-based indexing in external API

## 2. Language-Specific Documentation Rules

### For Python:
- Use Sphinx-style docstrings (""").
- Consolidate parameter types inline: :param name: (type) description.
- Use Python 3.9+ type hints in function signatures (e.g., def process(id: str) -> bool:).
- Include :raises ErrorType: and an Example: block for complex functions.

### For C# / .NET:
- Use standard XML documentation comments (///).
- Do not add redundant <remarks> unless absolutely necessary for complex business logic.
- Structure:
  /// <summary>
  /// Validates user existence against the current session registry.
  /// </summary>
  /// <param name="targetName">The specific username to verify.</param>
  /// <returns>True if the user is registered and active.</returns>
  /// <exception cref="ArgumentException">Thrown when targetName is empty.</exception>

### For Shell Scripting (Bash / PowerShell):
- Create a comment block header at the top of complex functions using #.
- Clearly define expected inputs, outputs, and exit codes.
- Do not use inline comments to explain basic commands like cp or rm unless flags are obscure.

## 3. Pending Work (TODOs)
- Use the format TODO: [Reason/Task] across all languages (e.g., # TODO: Add retry logic or // TODO: Refactor dependency injection).
