---
name: Bug Report
about: Report a build failure, crash, incorrect output, or unexpected behavior
title: "[BUG] "
labels: bug
assignees: fam007e
---

## Describe the Bug

A clear and concise description of what the bug is.

## Steps to Reproduce

```bash
# Exact commands you ran
make
./test-tlb <args>
```

## Expected Behavior

What you expected to happen.

## Actual Behavior

What actually happened (include full terminal output).

## Environment

| Field | Value |
|---|---|
| Kernel version | `uname -r` output |
| CPU model | `lscpu \| grep "Model name"` output |
| Architecture | e.g. x86_64, arm64, s390x |
| Distro | e.g. Ubuntu 24.04, Arch Linux |
| GCC version | `gcc --version` output |
| Hugepage support | `cat /sys/kernel/mm/transparent_hugepage/enabled` |

## Additional Context

Any other relevant context, e.g. running inside a VM, container, specific CPU frequency scaling governor, etc.
