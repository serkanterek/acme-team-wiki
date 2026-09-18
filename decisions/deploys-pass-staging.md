---
title: Deploys pass through staging first
summary: Since 2026-08-14 every gadget is tested in the staging canyon before it
  ships; decided after the rocket skates incident.
status: active
updated: 2026-08-14
tags:
  - key-decisions
  - how-we-work
sources:
  - sources/dev-thread-2026-08-14.md
---

## Context

Until August 2026 a finished gadget went straight from the workshop to the customer on the mesa. It was fast. It was also how the [canyon test of August 11](field-reports/2026-08-11-canyon-test.md) happened: the rocket skates were never run at full speed before the customer put them on.

## Decision

Every gadget goes through the staging canyon before it ships. No exceptions for a customer who is in a hurry. The procedure is in [How we deploy](runbooks/deploy.md).

## Options considered

- **Ship as before, add a warning label.** Rejected. The customer does not read labels; the customer reads the bird.
- **Test in the workshop only.** Rejected. The workshop has no cliff, and every failure so far has involved a cliff.
- **Test in the staging canyon under real conditions.** Chosen. It costs a day. The incident cost a customer.

## Rationale

The decision was made in the #dev thread on 2026-08-14, after Wiley E. presented the field report. The thread is the source cited above. The short version: we are not in the business of being fast. We are in the business of catching the bird.

## Consequences

The [rocket skates](products/rocket-skates.md) were the first product to go through the new process, and the first to be pulled from field use as a result. Every page in the catalogue now carries a "how it fails" section, written from staging results rather than from hope.
