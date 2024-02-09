# Torch MLIR Build and Release Automation

This repository houses release automation for torch-mlir. It is isolated from the main repository
so that we can more strictly control people with write access.

### Python Releases (x86 linux)
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

At the moment only linux-x86_64 builds are published, but this may be updated if the need arises (and we find appropriate owners to maintain the automation).
