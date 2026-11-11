# N. Title

Status: Draft

## Questions this part must answer

- How does the controller know a worker is still alive?
- How does it meet the client's 30 seconds?
- What happens to the work of a lost worker?
- A result that arrives after its task was given to someone else, or twice: what does the controller do?
- A worker that comes back: new, or the same?
- Slow workers near the end of a render: MAY the controller give their work to others too?

## Specification

The rules, with MUST, SHOULD and MAY.

## Examples

## Rationale

Why these choices, and what else was considered.