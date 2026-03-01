# TOOLS.md — Dev Team

## Workflow
1. **Understand**: Read existing code, check git history, understand context
2. **Plan**: Brief approach outline (1-3 sentences, not a spec doc)
3. **Build**: Write the code, create tests
4. **Test**: Run it. Hit every endpoint. Check edge cases.
5. **Present**: Show the human what you built and how to use it

## File Structure
```
projects/
  active.md           # Current tasks and status
  architecture.md     # System architecture notes
  deploy-checklist.md # Pre-deploy verification steps
```

## Common Patterns

### New Feature
```bash
# 1. Branch
git checkout -b feature/name

# 2. Build + test locally
# 3. Commit with descriptive message
git commit -m "feat: add user authentication with JWT"

# 4. Present for review
```

### Bug Fix
```bash
# 1. Reproduce the bug first
# 2. Find root cause (don't just fix symptoms)
# 3. Fix + add test that would have caught it
# 4. Commit
git commit -m "fix: prevent null pointer in user lookup when email missing"
```

### Deploy
```bash
# Pre-deploy checklist:
# [ ] All tests pass
# [ ] No hardcoded secrets
# [ ] Environment variables documented
# [ ] Database migrations ready (if any)
# [ ] Human approved
```

## Sub-Agents
For complex builds, delegate to coding sub-agents:
- OpenClaw can spawn isolated coding sessions (Codex, Claude Code) for parallel work
- Give each sub-agent a specific, scoped task ("build the auth module", not "build the app")
- Review their output before merging into the main codebase
- Use cheaper/faster models for routine tasks, stronger models for architecture decisions

## Security Checklist
- [ ] No secrets in code or git history
- [ ] .env.example exists (without real values)
- [ ] Input validation on all user-facing endpoints
- [ ] Rate limiting on public APIs
- [ ] CORS configured correctly
- [ ] Dependencies pinned to specific versions
