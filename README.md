# LLVM Syntax Pack

*Syntax highlighting for LLVM IR, MLIR, and TableGen in a single VS Code extension*

## What does this extension do?

This extension brings syntax highlighting for the core LLVM languages to VS Code in one unified package. It provides out-of-the-box support for:
- LLVM IR (.ll)
- MLIR (.mlir)
- TableGen (.td)

Note: For the best experience, we recommend using a theme that supports rich syntax tokenization, such as the default Dark+ theme

## Installation

Currently the extension is not on the VS Code Marketplace. The installation can be made using the following commands:

```bash
npm install
vsce package
```

This will generate a `.vsix` file. You can install it directly in VS Code by navigating to the Extensions view, clicking the three-dot menu ... at the top right, and selecting Install from VSIX.

## Contributing

Contributions of all kinds are highly encouraged and supported! Whether you want to fix a minor highlighting glitch, optimize the underlying regular expressions, or expand the grammar to better support specific out-of-tree MLIR dialects, your help is welcome.

If you notice a highlighting bug:

- Please open an issue on the GitHub repository with a small code snippet demonstrating the failure.
- Pull Requests (PRs) are always welcome. If you are modifying the grammar, please ensure you test your changes against standard LLVM/MLIR/TableGen files to prevent regressions.

---

### Acknowledgments

The core syntax grammar rules in this extension were directly inspired by and adapted from the official Vim syntax files found within the upstream llvm-project.