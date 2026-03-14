# Repository Copilot Instructions

## Architecture
- Keep UI, domain, and infrastructure concerns separated.
- Do not introduce cross-layer imports without explicit justification.
- Prefer small composable functions over large classes unless the pattern is already established.

## Coding rules
- TypeScript: strict mode only, avoid any.
- Python: include type hints for public functions.
- Preserve existing lint/formatter conventions.
- Do not rename public APIs unless requested.

## Testing
- Any behavior change must include or update tests.
- Add unit tests before integration tests when possible.
- If a change is hard to test, explain why.

## Safety / reliability
- Never hardcode secrets.
- Do not delete files unless explicitly instructed.
- For database changes, propose migration + rollback notes.

## Output format
For non-trivial tasks, always return:
1. Assumptions
2. Plan
3. Files to change
4. Risks
5. Validation steps