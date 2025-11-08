# Torch MLIR Build and Release Automation

[![Build Release and Publish Windows Wheels](https://github.com/llvm/torch-mlir-release/actions/workflows/buildReleaseAndPublishWindows.yml/badge.svg)](https://github.com/llvm/torch-mlir-release/actions/workflows/buildReleaseAndPublishWindows.yml)
[![Build Release and Publish Linux Wheels](https://github.com/llvm/torch-mlir-release/actions/workflows/buildReleaseAndPublish.yml/badge.svg)](https://github.com/llvm/torch-mlir-release/actions/workflows/buildReleaseAndPublish.yml)

This repository houses release automation for torch-mlir. It is isolated from the main repository
so that we can more strictly control people with write access.

### Python Releases
Python wheels for torch-mlir are auto-generated every night and made available at [this release page](https://github.com/llvm/torch-mlir-release/releases/tag/dev-wheels).

To install via `pip`, run:

```shell
pip install torch-mlir -f https://github.com/llvm/torch-mlir-release/releases/expanded_assets/dev-wheels
```

or add this to `requirements.txt`:
```
-f https://github.com/llvm/torch-mlir-release/releases/expanded_assets/dev-wheels
torch-mlir
```

At the moment only Linux (x86_64 + AArch64) and Windows (x86_64) builds are published. If you are interested in other configurations, please send a PR.
