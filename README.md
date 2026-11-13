# claude-angular-skill

A development skill for building, modernizing, reviewing, and optimizing applications with modern Angular.

## Overview

This skill covers Angular application architecture and implementation patterns, including Signals, standalone components, dependency injection, routing, forms, server-side rendering, hydration, and performance.

## Key Areas

- **Signals and reactive state:** Model local and shared state, derive values, and keep state ownership clear.
- **Standalone components:** Build focused components and organize feature boundaries.
- **Dependency injection:** Scope providers deliberately and keep services cohesive.
- **Routing and forms:** Use clear route boundaries, validation rules, and type-safe form models.
- **Rendering and performance:** Evaluate SSR, prerendering, hydration, lazy loading, and performance measurement.
- **Accessibility and testing:** Validate keyboard behavior, focus, labels, forms, and important user journeys.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-angular-skill.git ~/.claude/skills/angular
```

## Usage

Invoke `/angular` in an Angular project. For best results, include the Angular version, relevant files, expected behavior, and project constraints.

## Suggested Workflow

1. Inspect project configuration and installed Angular version.
2. Read existing architecture and local conventions.
3. Identify the smallest feature boundary that should change.
4. Choose the appropriate Angular primitive for state, routing, forms, or rendering.
5. Implement using established project patterns.
6. Add or update focused tests.
7. Run linting, type checks, tests, and production builds where available.
8. Review accessibility, loading states, and error handling.

## Supporting Resources

| Resource | Purpose |
|---|---|
| `resources/angular-architecture-review-checklist.md` | Assess components, state, dependency injection, routing, rendering, security, and maintainability. |
| `resources/angular-migration-planning-template.md` | Plan framework upgrades, compatibility checks, migration waves, and rollback points. |
| `resources/angular-feature-release-checklist.md` | Validate accessibility, performance, reliability, tests, and release readiness. |

## Maintenance

Keep recommendations aligned with the target project's Angular version. Verify support for version-specific APIs and third-party package compatibility before applying changes.

## Creator and maintainer

Created and maintained by **Brajesh Kumar**.
