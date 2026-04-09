# Contributing to test-tlb

Thank you for your interest in contributing to this fork of [Linus Torvalds' `test-tlb`](https://github.com/torvalds/test-tlb) — a simple memory latency and TLB benchmark tool for Linux.

## About This Fork

This is a personal fork maintained by [@fam007e](https://github.com/fam007e). Contributions that improve portability, correctness, usability, or documentation are welcome.

> **Note:** For changes that are broadly useful, consider also submitting them upstream to [torvalds/test-tlb](https://github.com/torvalds/test-tlb).

---

## How to Contribute

### Reporting Bugs

- Search [existing issues](../../issues) first to avoid duplicates.
- Use the **Bug Report** issue template and include:
  - Your Linux distro and kernel version (`uname -r`)
  - CPU architecture and model (`lscpu`)
  - Exact command used and observed vs. expected output

### Suggesting Enhancements

- Use the **Feature Request** issue template.
- Explain the use case clearly — why it's useful for a TLB/memory latency benchmark.

### Submitting Pull Requests

1. **Fork** the repo and create a branch:
   ```bash
   git checkout -b fix/your-description
   ```

2. **Make your changes** — keep them focused and minimal.

3. **Test your changes:**
   ```bash
   make
   ./test-tlb 64M 64
   make run
   ```

4. **Commit** with a clear message following [Conventional Commits](https://www.conventionalcommits.org/):
   ```
   fix: correct hugepage alignment on arm64
   feat: add -v flag for verbose output
   docs: update README with new stride examples
   ```

5. **Open a Pull Request** using the PR template and describe what changed and why.

---

## Code Style

- Match the existing **Linux kernel coding style** (tabs for indentation, K&R braces).
- Keep changes minimal — this is intentionally a small, self-contained tool.
- Avoid introducing external dependencies.
- Add `// flawfinder: ignore` comments only where false positives are well-understood (as already done in the codebase).

---

## License

By contributing, you agree that your contributions will be licensed under the **GNU General Public License v2.0** — the same license as this project. See [`LICENSE.txt`](LICENSE.txt) for details.
