# Angular Architecture Review Checklist

Use this during implementation reviews, feature planning, and modernization work. Apply guidance that matches the Angular version and architecture used by the project.

## Project baseline

- [ ] Record Angular, TypeScript, Node.js, and package manager versions.
- [ ] Identify whether the application is standalone-first or still module-heavy.
- [ ] Review routing, lazy-loading, and feature boundaries.
- [ ] Identify rendering mode: client-side, server-side, prerendered, or hybrid.
- [ ] Record existing state-management and data-fetching patterns.

## Component design

- [ ] Components have clear, cohesive responsibilities.
- [ ] Presentation and data-access concerns are separated where useful.
- [ ] Inputs and outputs form a clear component contract.
- [ ] Shared UI is reusable without creating unnecessary abstraction.
- [ ] Templates avoid complex business logic.
- [ ] OnPush or signal-driven rendering patterns are used consistently where appropriate.

## State and reactivity

- [ ] State has an explicit owner and lifecycle.
- [ ] Signals and computed values are used for suitable local or derived state.
- [ ] Effects are not used where a computed value or direct event handler is clearer.
- [ ] RxJS streams are composed and cleaned up appropriately.
- [ ] State mutation patterns are predictable and testable.

## Dependency injection and services

- [ ] Services have focused responsibilities.
- [ ] Provider scopes match the required lifecycle.
- [ ] Injection patterns are consistent with the project.
- [ ] Circular dependencies and hidden global state are avoided.
- [ ] External services are isolated behind testable boundaries.

## Routing, forms, and data access

- [ ] Routes are lazy-loaded where it improves startup and feature isolation.
- [ ] Guards and resolvers are limited to their intended responsibilities.
- [ ] Forms have explicit validation and accessible error states.
- [ ] HTTP errors, loading states, and retry behavior are handled.
- [ ] Data access is not duplicated across unrelated components.

## Rendering, security, and quality

- [ ] SSR and hydration behavior is validated for the target environment.
- [ ] Browser-only APIs are guarded in server-rendered paths.
- [ ] Untrusted content is handled safely.
- [ ] Keyboard navigation and accessible names are verified.
- [ ] Unit, integration, and end-to-end tests cover critical behavior.
- [ ] Bundle size and runtime performance are measured for important routes.

## Review outcome

- Critical issues:
- Important improvements:
- Accepted trade-offs:
- Version-specific constraints:
- Owner and follow-up date:
