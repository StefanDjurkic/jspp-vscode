# JSPP for VS Code

Syntax highlighting, snippets, and language configuration for **[JSPP (JavaScript++)](https://github.com/StefanDjurkic/jspp)** — JavaScript syntax, C++ performance.

## Features

- Syntax highlighting for `.jspp` files
  - Keywords, control flow, declarations
  - Primitive types (`int`, `i32`, `u64`, `float`, `string`, `bool`, `ptr`, …)
  - String, template literal, and char literals with escapes
  - Integer, hex, binary, and float literals
  - Line (`//`) and block (`/* */`) comments
  - Embedded `cpp { ... }` blocks highlighted as C++
- Language configuration
  - Bracket matching, auto-closing pairs, surrounding pairs
  - Smart indentation
  - `// #region` / `// #endregion` folding markers
- Snippets for common constructs: `fn`, `af`, `class`, `classe`, `type`, `enum`, `for`, `forof`, `switch`, `try`, `imp`, `cpp`, and more.

## Installation

### From source

```bash
git clone https://github.com/StefanDjurkic/jspp-vscode.git
cd jspp-vscode
npm install -g @vscode/vsce
vsce package
code --install-extension jspp-0.1.0.vsix
```

### From the Marketplace

Once published: search for **JSPP (JavaScript++)** in the VS Code Extensions view.

## About JSPP

JSPP is a transpiler that takes JavaScript-like syntax with optional static types and emits idiomatic C++17. See the main project: <https://github.com/StefanDjurkic/jspp>.

## Contributing

Issues and PRs welcome. This is a side project and contributions (better grammars, more snippets, themes) are appreciated.

## License

MIT — see [LICENSE](LICENSE).
