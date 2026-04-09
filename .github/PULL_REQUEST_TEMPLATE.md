## Description

Brief description of what this PR does and why.

Fixes # (issue number, if applicable)

## Type of Change

- [ ] Bug fix
- [ ] New feature / enhancement
- [ ] Documentation update
- [ ] Refactor (no functional change)
- [ ] Other (describe):

## Testing Done

```bash
# Commands run to verify the change
make
./test-tlb 64M 64
make run
```

**Test environment:**
- Kernel: 
- CPU: 
- Architecture: 

## Checklist

- [ ] Code follows the existing Linux kernel style (tabs, K&R braces)
- [ ] No new external dependencies introduced
- [ ] Tested with both regular pages and hugepages (`-H` flag) where relevant
- [ ] `README` updated if behavior or usage changed
- [ ] Commit message follows [Conventional Commits](https://www.conventionalcommits.org/)

## Notes for Reviewer

Any additional context, edge cases, or things to pay attention to during review.
