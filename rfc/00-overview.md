# 0. Overview

| | |
|---|---|
| Status | Draft |
| Version | 0.1 |
| Editors | One per group: name and group |

## Summary

The editors write it last: the farm in ten lines.

## The client's requirements

These come from the client and are not open to discussion. Every part of this RFC MUST satisfy them.

1. **One controller, many workers.** A worker starts knowing only the controller's address and who it belongs to: its group's name and its student's GitHub login.
2. **Any worker works for any controller.** Everything that goes between them follows this RFC.
3. **Only the controller is given the scene.** Workers learn everything else from it.
4. **Workers come and go.** A worker may start before the controller, join during a render, or disappear at any moment without warning: a crash, a freeze, a lost network.
5. **No tile is lost.** The work of a worker that disappears is given to another worker within 30 seconds. The render finishes, complete and correct, as long as one worker is left. A worker that comes back is used again.
6. **The controller shows what's happening.** During the render: who is connected, and the progress. At the end, a summary: who connected, how the work was shared out, how long each part took, what failed and what was done about it.
7. **The controller keeps a record.** For each render, it saves the final image as PNG, a report in the format of part 06, and every result as it was received, with who sent it.
8. **Every result is checked.** Each result is compared with a reference image, with the criteria of part 07.
9. **No shortcuts.** A worker renders every piece of work it accepts: no results kept from an earlier render.
10. **In C++**, in each group's project.

The client approves parts 06 and 07.

## Terms

Define here every word the other parts use: controller, worker, render, task, result, report.