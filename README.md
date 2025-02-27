# Python Requirements and Constraints Syntax Highlighting for Zed

## Overview

This extension provides syntax highlighting for `requirements.txt` and `constraints.txt` files in the [Zed](https://zed.dev/) code editor.

It leverages the [tree-sitter-requirements](https://github.com/tree-sitter-grammars/tree-sitter-requirements) grammar to ensure accurate and visually appealing syntax highlighting.

## Configuration

Zed does not (yet ?) support registering globs from extensions, so you will need to put these lines in your `settings.json` :

```json
{
  "file_types": {
    "Python constraints": [
      "constraints.txt",
      "constraints-*.txt",
      "constraints_*.txt",
      "*-constraints.txt",
      "*_constraints.txt"
    ],
    "Python requirements": [
      "requirements.txt",
      "requirements-*.txt",
      "requirements_*.txt",
      "*-requirements.txt",
      "*_requirements.txt"
    ]
  }
}
```

This should cover the most common cases.

## Contributing

If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This extension is licensed under the [MIT License](LICENSE).
