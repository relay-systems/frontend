# frontend

Web client of Relay: the user interface, whose user actions trigger HTTP and WebSocket requests to the backend services.

**Status:** not implemented yet. This repository only holds the project setup.

## Planned stack

Angular and TypeScript. No Angular project, `package.json`, dependencies or application code exist yet; they will be added as a separate task.

## Planned authentication

Sign-in via ZITADEL using OpenID Connect, Authorization Code flow with PKCE. The frontend will be a public client: it holds no client secret and stores no credentials. Redirect URIs and origins will be defined when the project is created.

## Related repositories

- `core-service`: application user profiles and core messaging logic
- `api-gateway`: single entry point for clients
- `realtime-gateway`: WebSocket gateway for real-time communication
- `ai-service`: AI-powered features
- `infrastructure`: local PostgreSQL and ZITADEL (Docker Compose)

## Branches

`TASK_<kebab-case>` -> `test` -> `main`, both through pull requests, enforced by the `branch-policy` workflow. Feature branches are created from `test`.
