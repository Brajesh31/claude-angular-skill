# Angular Feature Release Checklist

## Implementation quality

- [ ] Feature responsibilities and boundaries are clear.
- [ ] Components use a consistent standalone/module approach.
- [ ] State ownership and reactive dependencies are explicit.
- [ ] Loading, empty, success, and error states are implemented.
- [ ] Forms include validation and accessible error descriptions.
- [ ] Navigation, guards, and route data are tested.
- [ ] External API failures are handled deliberately.

## Accessibility

- [ ] All interactive controls are keyboard reachable.
- [ ] Focus order and focus restoration are predictable.
- [ ] Inputs have programmatic labels.
- [ ] Errors are associated with their controls.
- [ ] Dialogs and overlays manage focus correctly.
- [ ] Color is not the only indicator of state.
- [ ] Dynamic updates are announced where required.

## Rendering and performance

- [ ] Change detection behavior is understood and tested.
- [ ] Expensive lists and repeated views are optimized.
- [ ] Lazy loading or deferred loading is considered.
- [ ] Bundle size is checked for the affected route.
- [ ] Images and media are appropriately sized.
- [ ] SSR and hydration are validated when enabled.
- [ ] Browser-only APIs do not break server rendering.

## Security and reliability

- [ ] Untrusted HTML and URLs are handled safely.
- [ ] Authorization is enforced by the backend, not only the UI.
- [ ] Secrets are not embedded in client bundles.
- [ ] Error messages do not expose sensitive implementation details.
- [ ] Critical paths have automated regression coverage.

## Release verification

- [ ] Build succeeds using the documented toolchain.
- [ ] Unit and integration tests pass.
- [ ] Critical end-to-end journeys pass.
- [ ] Accessibility checks are complete.
- [ ] Browser and device coverage is appropriate.
- [ ] Monitoring and rollback owners are identified.
