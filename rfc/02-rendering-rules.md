# N. Title

Status: Draft

## Questions this part must answer

- Which ray goes through pixel (column, row)? Where is pixel (0, 0)?
- How does a polished surface mix its colour with what it reflects? What does `reflections` count, and what colour does a ray get when it runs out?
- Where does a reflected ray or a shadow ray start, so that it doesn't hit its own surface?
- When is a point in shadow: does a mirror block the sun too? What colour is a point in shadow, and what does `ambient` add where the sun shines?
- Is a triangle seen from both sides?
- What colour is a ray that hits nothing?
- From colour to byte: clamp, round, and in which order?

## Specification

The rules, with MUST, SHOULD and MAY.

## Examples

## Rationale

Why these choices, and what else was considered.