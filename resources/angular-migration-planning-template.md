# Angular Migration Planning Template

## Migration context

- Application:
- Current Angular version:
- Target Angular version:
- TypeScript version:
- Node.js version:
- Package manager and version:
- Current rendering mode:
- State-management approach:
- Repository and primary branch:
- Migration owner:

## Baseline inventory

| Area | Current state | Target state | Risk | Owner |
|---|---|---|---|---|
| Angular packages | | | | |
| TypeScript | | | | |
| Build configuration | | | | |
| Routing | | | | |
| Components and modules | | | | |
| Forms | | | | |
| State management | | | | |
| SSR and hydration | | | | |
| Tests and tooling | | | | |
| Third-party libraries | | | | |

## Compatibility review

- [ ] Check the official update path for each version boundary.
- [ ] Confirm Node.js and TypeScript compatibility.
- [ ] Identify deprecated or removed APIs used by the application.
- [ ] Check compatibility of UI libraries and Angular integrations.
- [ ] Review custom builders, schematics, and build scripts.
- [ ] Record required manual code changes.
- [ ] Identify behavior changes that need regression tests.

## Migration waves

| Wave | Scope | Dependencies | Test gate | Rollback point |
|---|---|---|---|---|
| 1 | Toolchain and dependency alignment | | | |
| 2 | Framework package updates | | | |
| 3 | Required code/API changes | | | |
| 4 | Build, routing, and rendering validation | | | |
| 5 | Optional modernization improvements | | | |

## Validation strategy

- Unit tests:
- Component tests:
- End-to-end tests:
- Accessibility checks:
- SSR and hydration tests:
- Performance and bundle checks:
- Browser/device coverage:

## Release plan

- Staging deployment:
- Smoke-test owner:
- Production release window:
- Monitoring signals:
- Rollback mechanism:
- Communication plan:

## Completion criteria

- [ ] Build and tests pass on the target toolchain.
- [ ] Critical user journeys work as expected.
- [ ] Accessibility and rendering regressions are checked.
- [ ] Deprecated API usage is reviewed.
- [ ] Dependencies are compatible and documented.
- [ ] Deployment and rollback procedures are verified.
