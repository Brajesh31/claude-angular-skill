# claude-angular-skill

A development skill for building, modernizing, reviewing, and optimizing applications with modern Angular.

## Overview

This skill focuses on current Angular application architecture and practical implementation patterns. It covers reactive state with Signals, standalone components, dependency injection, routing, forms, server-side rendering, hydration, and performance.

It is intended for developers working on new Angular applications as well as teams modernizing existing codebases.

## Key Areas

### Signals and Reactive State

- Model local and shared state with Angular Signals.
- Derive values with computed signals.
- Respond to state changes with appropriate reactive effects.
- Keep state ownership clear and avoid unnecessary subscriptions.
- Use signal-based component inputs and outputs where appropriate.

### Standalone Components

- Build components without requiring NgModule declarations.
- Organize imports at the component or feature boundary.
- Keep components focused and reusable.
- Lazy-load routes and feature areas to control application startup cost.

### Dependency Injection

- Use Angular's dependency injection system consistently.
- Apply the `inject()` function where it improves clarity.
- Scope providers deliberately.
- Keep services focused on cohesive responsibilities.

### Routing and Forms

- Configure routes with modern functional patterns.
- Use guards and resolvers for route-level behavior.
- Build reactive forms with clear validation rules.
- Prefer type-safe form models and explicit error states.

### Rendering and Performance

- Evaluate server-side rendering and prerendering requirements.
- Configure hydration carefully.
- Understand zoneless application patterns.
- Reduce unnecessary change detection and rendering work.
- Measure performance before introducing optimizations.

## When to Use This Skill

Use this skill when:

- Creating or extending an Angular application.
- Implementing Signals-based state management.
- Building standalone components and feature routes.
- Modernizing older Angular architecture.
- Configuring SSR, prerendering, or hydration.
- Improving application performance.
- Reviewing Angular code for maintainability and current framework conventions.

It is not intended as a general TypeScript reference or as a guide for AngularJS 1.x applications.

## Installation

Clone the repository into your Claude Code skills directory:

```bash
git clone https://github.com/Brajesh31/claude-angular-skill.git ~/.claude/skills/angular
```

On Windows, use the corresponding user-level skills directory:

```text
%USERPROFILE%\.claude\skills\angular
```

## Usage

Open an Angular project and describe the implementation or review task. The skill can be invoked directly:

```text
/angular
```

For best results, include the Angular version, relevant component or service, expected behavior, and any project constraints.

## Suggested Development Workflow

1. Inspect the project configuration and installed Angular version.
2. Read the existing architecture and local conventions.
3. Identify the smallest feature boundary that should change.
4. Choose the appropriate Angular primitive for state, routing, forms, or rendering.
5. Implement the change using the patterns already established in the project.
6. Add or update focused tests.
7. Run linting, type checks, tests, and production builds where available.
8. Review accessibility, loading states, and error handling.

## Example Project Structure

A feature-oriented Angular project may be organized as follows:

```text
src/
├── app/
│   ├── core/
│   │   ├── services/
│   │   └── guards/
│   ├── shared/
│   │   └── components/
│   ├── features/
│   │   └── example/
│   │       ├── pages/
│   │       ├── components/
│   │       └── data-access/
│   ├── app.config.ts
│   └── app.routes.ts
└── main.ts
```

Adapt this structure to the size and needs of the application rather than creating folders without a clear purpose.

## Quality Checklist

- Components have clear responsibilities.
- State is modeled with the simplest suitable reactive primitive.
- Services do not become catch-all containers.
- Routes are lazy-loaded when it benefits the application.
- Forms provide useful validation feedback.
- SSR and hydration behavior is tested in the target environment.
- Accessibility and keyboard behavior are considered.
- Tests cover important user-visible behavior.

## Repository Contents

- `SKILL.md`: Detailed instructions and decision guidance for Angular tasks.
- `README.md`: Overview, installation, workflows, and practical checklist.

## Maintenance

Keep framework-specific recommendations aligned with the Angular version used by the target project. When a recommendation depends on a particular release, state that version boundary clearly rather than applying it to every Angular codebase.
