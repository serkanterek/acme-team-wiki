---
title: How we deploy
summary: The steps every gadget takes from the workshop to a customer, with the
  staging canyon in the middle.
status: active
updated: 2026-08-14
tags:
  - how-we-work
---

Since 2026-08-14 no gadget ships straight from the workshop to a customer. It goes through the staging canyon first. The reason is in [Deploys pass through staging first](decisions/deploys-pass-staging.md); this page is the procedure.

## Steps

1. Build the gadget in the workshop and label it with a batch number.
2. Take it to the staging canyon. Wiley E. owns this step (see [Who owns what](people/who-owns-what.md)).
3. Run the gadget under the same conditions the customer will run it: full speed, real cliff, real bird if one is available. Nobody has caught one, so usually a painted tunnel.
4. Write the field report the same day, even if the gadget worked. Especially if the gadget worked.
5. Only after the report is in the wiki does the gadget ship to production, meaning the mesa.

## When something goes wrong in staging

Stop. Write it up. Do not ship it anyway because the customer is waiting. The customer is always waiting; that is what the customer does. The [canyon test of August 11](field-reports/2026-08-11-canyon-test.md) is what happens when this step is skipped.

The words in this page that have a house meaning (staging canyon, the mesa, production) are defined in the [glossary](glossary/key-terms.md).
