# ECMA-262 Formal Specifications & Architecture Documentation Index

## 📚 Quick Navigation

This repository contains the ECMAScript Language Specification along with comprehensive formal specifications and architecture documentation.

### 🎯 Start Here

**New to this repository?** → Read [`README.md`](README.md)  
**Want formal specifications?** → Read [`README-ZPP.md`](README-ZPP.md)  
**Need build system docs?** → Read [`architecture_overview.md`](architecture_overview.md)  
**Integration guide?** → Read [`FORMAL-SPECS-INTEGRATION.md`](FORMAL-SPECS-INTEGRATION.md)

---

## 📖 Documentation Catalog

### Primary Specification

| Document | Description | Lines/Size | Audience |
|----------|-------------|------------|----------|
| [`spec.html`](spec.html) | **ECMAScript Language Specification** (main source) | 53,434 lines | Language implementers, standards bodies |

### Architecture Documentation

| Document | Description | Size | Key Features |
|----------|-------------|------|--------------|
| [`architecture_overview.md`](architecture_overview.md) | **Complete technical architecture** with Mermaid diagrams | 18.5 KB | 6 detailed diagrams: build pipeline, CI/CD, validation, component architecture |
| [`FORMAL-SPECS-INTEGRATION.md`](FORMAL-SPECS-INTEGRATION.md) | **Integration guide** for all formal specifications | 15.4 KB | Three-layer model, usage scenarios, best practices |

### Formal Specifications (Z++)

| Specification | Purpose | Size | Key Schemas |
|---------------|---------|------|-------------|
| [`ecmascript-zpp-specification.zpp`](ecmascript-zpp-specification.zpp) | **ECMAScript language semantics** | 597 lines | Lexical grammar, AST, values, objects, types, execution |
| [`build_system.zpp`](build_system.zpp) | **Build pipeline formalization** | 15.5 KB | Build state, operations, validation, theorems |
| [`spec_structure.zpp`](spec_structure.zpp) | **Document structure formalization** | 14.4 KB | Sections, grammar, algorithms, built-ins, validation |
| [`zpp-usage-examples.zpp`](zpp-usage-examples.zpp) | **Z++ usage examples** | 285 lines | Practical demonstrations |

### Analysis & Guides

| Document | Description | Focus |
|----------|-------------|-------|
| [`ZPP-SPECIFICATION-ANALYSIS.md`](ZPP-SPECIFICATION-ANALYSIS.md) | **Deep architectural analysis** by Deep Tree Echo | Language specification philosophy, verification theorems |
| [`README-ZPP.md`](README-ZPP.md) | **Z++ specifications user guide** | Introduction, features, usage |

### Contributing & Process

| Document | Purpose |
|----------|---------|
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Contribution guidelines, TC39 process |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Community code of conduct |
| [`FAQ.md`](FAQ.md) | Frequently asked questions |
| [`SECURITY.md`](SECURITY.md) | Security policy |

---

## 🗺️ Specification Architecture Map

```
ECMA-262 Repository
├── Language Specification Layer
│   ├── spec.html (source)
│   └── ecmascript-zpp-specification.zpp (formal semantics)
│
├── Meta-Specification Layer
│   ├── spec_structure.zpp (document structure)
│   └── build_system.zpp (build pipeline)
│
├── Documentation Layer
│   ├── architecture_overview.md (build architecture + diagrams)
│   ├── FORMAL-SPECS-INTEGRATION.md (integration guide)
│   ├── ZPP-SPECIFICATION-ANALYSIS.md (language analysis)
│   └── README-ZPP.md (user guide)
│
└── Supporting Materials
    ├── zpp-usage-examples.zpp (examples)
    ├── scripts/ (build automation)
    └── .github/workflows/ (CI/CD)
```

---

## 🎓 Learning Paths

### Path 1: Understanding ECMAScript Language

1. Read [`README.md`](README.md) - Repository overview
2. Browse [`spec.html`](spec.html) - Official specification
3. Study [`ecmascript-zpp-specification.zpp`](ecmascript-zpp-specification.zpp) - Formal semantics
4. Review [`ZPP-SPECIFICATION-ANALYSIS.md`](ZPP-SPECIFICATION-ANALYSIS.md) - Deep analysis
5. Try [`zpp-usage-examples.zpp`](zpp-usage-examples.zpp) - Practical examples

### Path 2: Contributing to Specification

1. Read [`CONTRIBUTING.md`](CONTRIBUTING.md) - Contribution process
2. Study [`spec_structure.zpp`](spec_structure.zpp) - Document structure requirements
3. Review [`architecture_overview.md`](architecture_overview.md) - Build system understanding
4. Follow build instructions in [`README.md`](README.md)
5. Submit changes following TC39 process

### Path 3: Working with Build System

1. Read [`architecture_overview.md`](architecture_overview.md) - Complete architecture
2. Study [`build_system.zpp`](build_system.zpp) - Formal build model
3. Review [`package.json`](package.json) - NPM scripts and dependencies
4. Examine [`scripts/`](scripts/) - Build automation scripts
5. Check [`.github/workflows/`](.github/workflows/) - CI/CD configuration

### Path 4: Formal Methods Research

1. Start with [`README-ZPP.md`](README-ZPP.md) - Z++ introduction
2. Study [`zpp-usage-examples.zpp`](zpp-usage-examples.zpp) - Learn syntax
3. Analyze [`ecmascript-zpp-specification.zpp`](ecmascript-zpp-specification.zpp) - Language formalization
4. Explore [`spec_structure.zpp`](spec_structure.zpp) - Meta-specification
5. Review [`build_system.zpp`](build_system.zpp) - Build formalization
6. Read [`FORMAL-SPECS-INTEGRATION.md`](FORMAL-SPECS-INTEGRATION.md) - Integration patterns

---

## 🔍 Quick Reference

### Build Commands

```bash
# Clean build artifacts
npm run clean

# Build with strict validation (for PRs)
npm run build-head

# Standard development build
npm run build-only

# Watch mode for development
npm run watch

# Generate PDF
npm run pdf

# Snapshot build (with warning)
npm run build-snapshot
```

### Key Diagrams (in architecture_overview.md)

1. **High-Level Component Architecture** - Overall system structure
2. **Build System Data Flow** - Source → Build → Output pipeline
3. **CI/CD Pipeline Architecture** - GitHub Actions workflows
4. **Specification Validation** - Multi-level quality control
5. **Ecmarkup Processing** - Document transformation
6. **Module & Script Organization** - Code organization

### Important Theorems (in Z++ specs)

From `ecmascript-zpp-specification.zpp`:
- **ParseCompleteness**: All valid source code can be parsed
- **EvaluationDeterminism**: Programs evaluate consistently
- **TypeSafety**: Well-typed programs don't have type errors

From `build_system.zpp`:
- **BuildCompleteness**: Valid sources always build successfully
- **BuildDeterminism**: Same input produces same output

From `spec_structure.zpp`:
- **SpecificationCompleteness**: All grammar has semantics
- **SpecificationEvolution**: Backward compatibility preserved

---

## 📊 Repository Metrics

| Category | Count | Total Size |
|----------|-------|------------|
| **Specification Documents** | 1 | 53,434 lines |
| **Z++ Formal Specs** | 4 | ~2,000 lines |
| **Architecture Docs** | 4 | ~50 KB |
| **Mermaid Diagrams** | 6 | in architecture_overview.md |
| **Build Scripts** | 6 | ~50 lines total |
| **CI/CD Workflows** | 8 | ~500 lines total |
| **Supporting Files** | 15+ | Various |

---

## 🔗 External Links

### TC39 Ecosystem

- **Published Spec**: https://tc39.es/ecma262/
- **GitHub Repository**: https://github.com/tc39/ecma262
- **Proposals**: https://github.com/tc39/proposals
- **Test Suite**: https://github.com/tc39/test262
- **Discussion Forum**: https://es.discourse.group/
- **Matrix Chat**: See [TC39 Matrix Guide](https://github.com/tc39/how-we-work/blob/HEAD/matrix-guide.md)

### Related Specifications

- **ECMA-402 (Intl API)**: https://tc39.es/ecma402/
- **HTML Standard**: https://html.spec.whatwg.org/
- **Web IDL**: https://heycam.github.io/webidl/
- **WebAssembly**: https://webassembly.github.io/spec/

### Tools

- **Ecmarkup**: https://github.com/tc39/ecmarkup
- **Node.js**: https://nodejs.org/
- **Prince PDF**: https://www.princexml.com/

---

## 🎯 Use Cases

### "I want to implement ECMAScript in my language runtime"

**Resources:**
1. [`spec.html`](spec.html) - Normative specification
2. [`ecmascript-zpp-specification.zpp`](ecmascript-zpp-specification.zpp) - Formal semantics
3. [Test262](https://github.com/tc39/test262) - Conformance tests
4. [`ZPP-SPECIFICATION-ANALYSIS.md`](ZPP-SPECIFICATION-ANALYSIS.md) - Semantic analysis

### "I want to propose a new ECMAScript feature"

**Resources:**
1. [`CONTRIBUTING.md`](CONTRIBUTING.md) - Contribution process
2. [TC39 Process](https://tc39.es/process-document/) - Proposal stages
3. [`spec_structure.zpp`](spec_structure.zpp) - Structure requirements
4. [ES Discourse](https://es.discourse.group/) - Community discussion

### "I want to modify the specification build system"

**Resources:**
1. [`architecture_overview.md`](architecture_overview.md) - Build architecture
2. [`build_system.zpp`](build_system.zpp) - Formal build model
3. [`package.json`](package.json) - Build scripts
4. [`.github/workflows/build.yml`](.github/workflows/build.yml) - CI configuration

### "I want to research formal methods in language specification"

**Resources:**
1. [`FORMAL-SPECS-INTEGRATION.md`](FORMAL-SPECS-INTEGRATION.md) - Integration guide
2. All `.zpp` files - Complete formal specifications
3. [`ZPP-SPECIFICATION-ANALYSIS.md`](ZPP-SPECIFICATION-ANALYSIS.md) - Theoretical foundations
4. [`architecture_overview.md`](architecture_overview.md) - Meta-specification architecture

---

## 📝 Document Versions

| Document | Version | Last Updated | Status |
|----------|---------|--------------|--------|
| spec.html | Living Standard | Continuous | Official |
| architecture_overview.md | 1.0 | 2025-11-12 | New |
| build_system.zpp | 1.0 | 2025-11-12 | New |
| spec_structure.zpp | 1.0 | 2025-11-12 | New |
| FORMAL-SPECS-INTEGRATION.md | 1.0 | 2025-11-12 | New |
| ecmascript-zpp-specification.zpp | 1.0 | Prior | Existing |
| ZPP-SPECIFICATION-ANALYSIS.md | 1.0 | Prior | Existing |
| README-ZPP.md | 1.0 | Prior | Existing |

---

## 🤝 Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for detailed contribution guidelines.

**Quick Summary:**
1. Read contribution guidelines
2. Understand TC39 process for language changes
3. Use proper commit message format (Normative/Editorial/Meta: description (#PR))
4. Build and test locally before submitting
5. Follow existing patterns in specification structure

---

## 📧 Contact & Community

- **Editors**: See [`spec.html`](spec.html) metadata section
- **Discussion**: [ES Discourse](https://es.discourse.group/)
- **Chat**: [TC39 Matrix](https://github.com/tc39/how-we-work/blob/HEAD/matrix-guide.md)
- **Issues**: [GitHub Issues](https://github.com/tc39/ecma262/issues)
- **Pull Requests**: [GitHub PRs](https://github.com/tc39/ecma262/pulls)

---

**Index Version**: 1.0  
**Last Updated**: 2025-11-12  
**Maintained By**: Repository contributors  
**License**: See [LICENSE.md](LICENSE.md)
