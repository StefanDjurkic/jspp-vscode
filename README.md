# JSPP for VS Code

[![CI](https://github.com/StefanDjurkic/jspp-vscode/actions/workflows/ci.yml/badge.svg)](https://github.com/StefanDjurkic/jspp-vscode/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

Syntax highlighting, snippets, and language configuration for **[JSPP (JavaScript++)](https://github.com/StefanDjurkic/jspp)** — JavaScript syntax, C++ performance.

## Features

- **Syntax highlighting** for `.jspp` files
  - Keywords, control flow, declarations (`class`, `function`, `type`, `enum`, `constructor`, `operator`, `extends`, `new`, `shared_new`, `ref`, …)
  - Primitive types (`int`, `i8`/`i16`/`i32`/`i64`, `u8`/`u16`/`u32`/`u64`, `float`, `double`, `bool`, `string`, `char`, `void`, `auto`, `size`, `ptr`)
  - Class / type / enum / function declaration names picked up as entities
  - Type annotations after `:` highlighted as types
  - String, char, and template literals (with `${expr}` interpolation)
  - Integer, hex, binary, and float literals
  - Line (`//`) and block (`/* */`) comments
  - `cpp { ... }` blocks highlighted as embedded **C++**
  - `cpp_include "<header>"` treated as an import
- **Language configuration**
  - Bracket matching, auto-closing pairs, surrounding pairs
  - Smart indentation
  - JSDoc-style `/** */` continuation on Enter
  - `// #region` / `// #endregion` folding markers
- **Snippets** for common constructs: `fn`, `af`, `class`, `classe`, `type`, `enum`, `for`, `forof`, `switch`, `try`, `imp`, `expfn`, `cpp`, and more.

## Installation

### From the Marketplace

Search for **JSPP (JavaScript++)** in the VS Code Extensions view, or install via command line:

```
code --install-extension StefanDjurkic.jspp
```

### From a `.vsix` release

Download the latest `jspp-<version>.vsix` from [Releases](https://github.com/StefanDjurkic/jspp-vscode/releases) and run:

```
code --install-extension jspp-<version>.vsix
```

### From source

```bash
git clone https://github.com/StefanDjurkic/jspp-vscode.git
cd jspp-vscode
npm install -g @vscode/vsce
vsce package
code --install-extension jspp-0.1.0.vsix
```

## About JSPP

JSPP is a transpiler that takes JavaScript-like syntax with optional static types and emits idiomatic C++17. See the main project: <https://github.com/StefanDjurkic/jspp>.

## Contributing

Issues and PRs welcome. This is a side project and contributions (grammar refinements, more snippets, theme tweaks) are appreciated.

## License

MIT — see [LICENSE](LICENSE).
