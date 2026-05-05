# Jakarta Language

**Bahasa pemrograman berbasis Bahasa Indonesia dengan sintaks yang mudah dipahami.**

A programming language based on Indonesian with intuitive, easy-to-understand syntax. Jakarta Language (`.jkt`) is designed to lower the barrier to entry for Indonesian-speaking developers by providing keywords, constructs, and built-in functions in Bahasa Indonesia.

---

## About

Jakarta Language is an open-source programming language project that aims to make coding more accessible for Indonesian speakers. Instead of using English-based keywords, Jakarta Language uses Indonesian words such as `jika` (if), `selama` (while), `fungsi` (function), and `cetak` (print), allowing developers to write programs in a syntax that feels natural in their native language.

The project includes multiple interpreter implementations across different programming languages, a VS Code extension for syntax highlighting and code snippets, and a browser-based playground for running Jakarta code directly on the web.

---

## Key Features

- **Indonesian-based syntax** -- All keywords, built-in functions, and error messages use Bahasa Indonesia
- **Multi-language interpreters** -- Reference implementations in Python, Go, Ruby, Rust, C, Java, Node.js/TypeScript, and Shell
- **Web Playground** -- Browser-based editor with real-time execution and error reporting
- **VS Code Extension** -- Syntax highlighting, code snippets, bracket matching, and comment toggling for `.jkt` files
- **Closures and Recursion** -- Full support for functional programming patterns
- **Rich built-in library** -- String manipulation, math functions, list operations, and type conversion

---

## Language Overview

### Keywords

| Jakarta | English | Purpose |
|---------|---------|---------|
| `cetak` | print | Print to screen |
| `var` | var | Variable declaration |
| `konstan` | const | Constant declaration |
| `fungsi` | function | Function definition |
| `kembali` | return | Return value |
| `jika` | if | Conditional |
| `lain` | else | Else branch |
| `selama` | while | While loop |
| `untuk` | for | For loop |
| `dalam` | in | Iteration |
| `benar` | true | Boolean true |
| `salah` | false | Boolean false |
| `kosong` | null | Null value |
| `dan` | and | Logical AND |
| `atau` | or | Logical OR |
| `bukan` | not | Logical NOT |
| `putus` | break | Break loop |
| `lanjut` | continue | Continue loop |

### Data Types

| Jakarta | English | Example |
|---------|---------|---------|
| `angka` | number | `42`, `3.14` |
| `teks` | string | `"Halo"`, `'Jakarta'` |
| `boolean` | boolean | `benar`, `salah` |
| `daftar` | list | `[1, 2, 3]` |
| `kosong` | null | `kosong` |

### Code Example

```
fungsi faktorial(n) {
    jika (n <= 1) {
        kembali 1
    }
    kembali n * faktorial(n - 1)
}

cetak("5! = " + teks(faktorial(5)))
```

---

## Interpreter Implementations

Jakarta Language provides interpreter implementations in the following languages:

| Language | Status | REPL Support |
|----------|--------|--------------|
| Python | Full | Yes |
| Go | Full | No |
| Ruby | Full | Yes |
| Rust | Full | No |
| C | Full | No |
| Java | Full | No |
| Node.js / TypeScript | Full | No |
| Shell | Basic | No |
| Web (Browser) | Full | Yes |

---

## Quick Start

### Running with Python (Reference Implementation)

```bash
python src/interpreter.py example/main.jkt
python src/interpreter.py              # REPL mode
```

### Running with Go

```bash
cd src/go
go run main.go ../../example/main.jkt
```

### Running with Rust

```bash
cd src/rust
cargo run -- ../../example/main.jkt
```

### Web Playground

Open `web/index.html` in any modern browser. The playground provides a code editor with line numbers, example programs, real-time execution, and keyboard shortcuts (`Ctrl+Enter` to run, `Tab` for indentation).

---

## VS Code Extension

The Jakarta Language extension for VS Code provides:

- Syntax highlighting for `.jkt` files
- Code snippets for all keywords and constructs
- Bracket matching and auto-closing
- Comment toggling (`//` and `/* */`)
- Custom file icon

### Installation via VSIX

```bash
npm install -g @vscode/vsce
cd jakarta-lang
vsce package
code --install-extension jakarta-lang-0.1.0.vsix
```

---

## Project Structure

```
jakarta-lang/
├── package.json                    # VS Code extension manifest
├── language-configuration.json     # Language configuration
├── syntaxes/
│   └── jakarta.tmLanguage.json     # Syntax highlighting grammar
├── snippets/
│   └── jakarta.json                # Code snippets
├── images/
│   └── jakarta-icon.svg            # File icon for .jkt
├── src/
│   ├── interpreter.py              # Python interpreter (reference)
│   ├── go/                         # Go interpreter
│   ├── ruby/                       # Ruby interpreter
│   ├── rust/                       # Rust interpreter
│   ├── c/                          # C interpreter
│   ├── java/                       # Java interpreter
│   ├── node/                       # Node.js/TypeScript interpreter
│   └── shell/                      # Shell interpreter
├── web/
│   ├── index.html                  # Web playground UI
│   ├── style.css                   # Playground styles
│   ├── interpreter.js              # Browser interpreter
│   └── app.js                      # Playground controller
├── example/
│   ├── main.jkt                    # Basic example
│   └── advanced.jkt                # Advanced example
└── README.md
```

---

## Contributing

Contributions are welcome. Whether you want to add a new interpreter implementation, improve existing features, fix bugs, or enhance documentation, your help is appreciated.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add your feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## License

This project is licensed under the GPL-3.0 License. See the [LICENSE](https://github.com/Jakarta-Language/jakarta-lang/blob/main/LICENSE) file for details.

---

## Links

- **Repository**: [github.com/Jakarta-Language/jakarta-lang](https://github.com/Jakarta-Language/jakarta-lang)
- **Issues**: [github.com/Jakarta-Language/jakarta-lang/issues](https://github.com/Jakarta-Language/jakarta-lang/issues)
- **Contributors**: [SOBING4413](https://github.com/SOBING4413)
