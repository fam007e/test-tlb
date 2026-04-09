# Security Policy

## Supported Versions

This is a personal fork of [`torvalds/test-tlb`](https://github.com/torvalds/test-tlb), a local Linux benchmark tool. Only the latest commit on `master` is actively maintained.

| Version | Supported |
|---------|-----------|
| `master` (latest) | ✅ Yes |
| Older commits | ❌ No |

## Scope

`test-tlb` is a **local, single-user diagnostic tool** — it is not a daemon, network service, or multi-user application. Its attack surface is minimal by design.

Known intentional patterns (not vulnerabilities):
- Use of `random()`, `mmap`, `madvise` — standard for a benchmark tool.
- `// flawfinder: ignore` annotations are present where false positives have been reviewed.

## Reporting a Vulnerability

If you discover a genuine security issue (e.g., a memory safety bug that could be exploited when run as root or in a privileged context):

1. **Do not open a public GitHub issue.**
2. Report it privately by [emailing](mailto:faisalmoshiur+testtlb@gmail.com) the maintainer or via [GitHub private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability) if enabled.
3. Include:
   - A description of the vulnerability
   - Steps to reproduce
   - Potential impact

You can expect an acknowledgment within **7 days** and a resolution or response within **30 days**.

> For vulnerabilities in the upstream codebase, please also report to [torvalds/test-tlb](https://github.com/torvalds/test-tlb).
