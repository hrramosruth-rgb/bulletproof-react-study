# React feature architecture — source study

These notes were added in October 2026. The application is the work of the original upstream contributors. This fork does not claim the upstream code, dates, or experience as work by Ruth Ramos.

Source: [alan2207/bulletproof-react](https://github.com/alan2207/bulletproof-react). The exact imported revision is recorded in [SOURCE.json](SOURCE.json).

## Source map

| Entry point | What to trace |
| --- | --- |
| [apps/react-vite/src/features](../apps/react-vite/src/features) | Feature modules and their API/component boundaries |
| [apps/react-vite/src/lib/api-client.ts](../apps/react-vite/src/lib/api-client.ts) | Credentialed requests, error notification, and unauthorized redirects |
| [apps/react-vite/src/lib/react-query.ts](../apps/react-vite/src/lib/react-query.ts) | Shared server-state query configuration |
| [apps/react-vite/src/lib/authorization.tsx](../apps/react-vite/src/lib/authorization.tsx) | Client-side permission helpers |
| [AGENTS.md](../AGENTS.md) | Repository architecture and development conventions |

## Study exercise

Trace a discussion request from its page through a feature API hook and the shared client. Treat client permission helpers as interface behavior, not a replacement for server authorization.

## Setup and verification

Use the preserved [upstream README](../README.md) for setup and the repository package scripts for the exact commands. This addition changes documentation only. Dependencies were not installed and application tests were not run.

The added documentation was checked for valid local links, a matching upstream revision, unchanged application files, and preservation of the [MIT license](../LICENSE).

## Attribution

The original license and copyright notice remain unchanged. All imported commits retain their original authors. Only this fork's study documentation is a new contribution dated October 2026.
