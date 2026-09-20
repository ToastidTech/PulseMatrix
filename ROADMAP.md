# PulseMatrix Production Roadmap

PulseMatrix is currently a functional marketing command-hub prototype. This roadmap tracks the work required to move it toward a production-ready Toastid Tech product without breaking the existing working flows.

## Phase 1: Harden the BYOK architecture

- [ ] Move Anthropic requests behind a controlled backend/API route.
- [ ] Keep customer BYOK support so Toastid Cloud can remain the long-term routing layer.
- [ ] Remove direct browser-side dependency on Anthropic's browser-access header.
- [ ] Add request validation, bounded inputs, error normalization, and rate limiting.
- [ ] Never persist provider secrets outside the customer's intended local/secure storage path.

## Phase 2: Replace mock dashboard behavior

- [ ] Define the PulseMatrix analytics data contract.
- [ ] Add a real dashboard data source.
- [ ] Replace the static "100% Operational" feed with live service state.
- [ ] Add explicit loading, empty, and error states.

## Phase 3: Production UX

- [ ] Audit every workflow on mobile first.
- [ ] Improve keyboard/focus/accessibility behavior.
- [ ] Add consistent Toastid Tech visual language and responsive spacing.
- [ ] Replace browser alerts with in-app status/toast components.
- [ ] Add copy/export states that work cleanly on mobile.

## Phase 4: Workflow completeness

- [ ] Give each of the six command cards a defined input/output contract.
- [ ] Add structured outputs for ad scripts, hooks, visual prompts, content calendars, and competitor analysis.
- [ ] Add reusable prompt templates and versioned system instructions.
- [ ] Add persistent project/session state where appropriate.

## Phase 5: Deployment and launch

- [ ] Add production deployment configuration.
- [ ] Add environment/configuration documentation.
- [ ] Add smoke tests for all six workflows.
- [ ] Add health/status checks.
- [ ] Run a final mobile and production QA pass.
- [ ] Promote PulseMatrix from prototype to launched product.

## Guardrails

Existing working behavior should remain intact while each phase is implemented. Changes should be incremental, reviewable, and easy to roll back.
