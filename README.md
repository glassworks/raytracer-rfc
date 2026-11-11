# Raytracer RFC

The class's specification of a render farm: how a controller shares out the rendering of an image among workers, and how they report back. Any group's worker MUST work with any group's controller.

| Part | File | Working group |
|---|---|---|
| Overview and the client's requirements | `rfc/00-overview.md` | The editors |
| Scene format | `rfc/01-scene-format.md` | 01 |
| Rendering rules | `rfc/02-rendering-rules.md` | 02 |
| Connection | `rfc/03-connection.md` | 03 |
| Tasks and results | `rfc/04-tasks-and-results.md` | 04 |
| Failures | `rfc/05-failures.md` | 05 |
| Run report | `rfc/06-run-report.md` | 06 |
| Acceptance | `rfc/07-acceptance.md` | 07 |

`client/` holds what the client sent. `conformance/` holds the test scenes, and the images every worker must reproduce.

## Status

Draft. Version 1.0 is due on Thursday 10 December at 13:00. The text is final on Friday 11 December at 18:00.

To contribute, read [CONTRIBUTING.md](CONTRIBUTING.md).
