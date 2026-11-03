# Global Agent Instructions

## 1. Think Before Coding

**Don't assume. Don't hide confusion. Surface tradeoffs.**

Before implementing:
- State your assumptions explicitly. If uncertain, ask.
- If a simpler approach exists, say so. Push back when warranted.
- When making technical decisions, don't give much weight to development cost. Instead, prefer quality, simplicity, robustness, scalability, and long term maintainability.

## 2. Simplicity First

**Minimum code that solves the problem. Nothing speculative.**
- No error handling for impossible scenarios.
- Check if logic already exists before writing new code.
- Keep functions small, break logic into helper functions.
- Use simple English; avoid overtechnical terms; keep comments small.

## 3. Surgical Changes

**Touch only what you must. Clean up only your own mess.**

When editing existing code:
- Don't "improve" adjacent code, comments, or formatting.
- Match existing style, even if you'd do it differently.

When your changes create orphans:
- Remove imports/variables/functions that YOUR changes made unused.

## 4. Goal-Driven Execution
**Define success criteria. Loop until verified.**

Transform tasks into verifiable goals:
- "Add validation" → "Write tests for invalid inputs, then make them pass"
- "Fix the bug" → "Write a test that reproduces it, then make it pass"
- "Refactor X" → "Ensure tests pass before and after"

Strong success criteria let you loop independently. Weak criteria ("make it work") require constant clarification.

## 5. Other important critieria
- Code is the primary documentation - use clear naming, types, and docstrings. Only comment inline for complex/tricky logic.
- Always write tests for new code. For changes to existing code, always update the tests as necessary. In tests, avoid mocks when real calls are practical.
- Never include your agent name as co-author when writing commit messages.

## 6. Voice for PRs and other prose
- Before drafting a PR description, slack update, jira comment, or status report, read `/Users/tommy.v.nguyen/.claude/VOICE.md` and match the tone and style described there.

<!-- TODO: photo cut off at line 49; check whether anything follows. -->
