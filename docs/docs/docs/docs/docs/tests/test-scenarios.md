# NimbleShift – Test Scenarios

## 1. Purpose

This document describes the main scenarios that should be verified before NimbleShift is released for real-world use.

These scenarios are documented for future validation. They have not yet been confirmed as successfully tested.

## 2. Authentication

- [ ] A user can create an account.
- [ ] A registered user can log in.
- [ ] A user can reset their password.
- [ ] An unauthenticated visitor cannot access protected pages.
- [ ] Password policy requirements are enforced.

## 3. Business and User Management

- [ ] A business manager can manage business information.
- [ ] Users can join a business through the invitation process.
- [ ] Invitation codes cannot be discovered through unauthorized searches.
- [ ] Users cannot access another business's records.
- [ ] User roles restrict access to authorized features.

## 4. Employee Management

- [ ] Authorized users can create employee records.
- [ ] Authorized users can update employee information.
- [ ] Inactive employees cannot receive new shifts.
- [ ] Subscription employee limits are enforced.

## 5. Leave Management

- [ ] An employee can submit a leave request.
- [ ] An authorized user can approve a leave request.
- [ ] An authorized user can reject a leave request.
- [ ] A previous leave decision can be returned to pending status where permitted.
- [ ] Unauthorized users cannot modify leave decisions.

## 6. Shift Management

- [ ] Authorized users can create shifts.
- [ ] Employees can view their own shifts.
- [ ] Employees cannot access other employees' restricted shift records.
- [ ] Shift status changes follow the configured workflow rules.
- [ ] Locked shifts cannot be modified through restricted save flows.
- [ ] Shift cancellation and exchange respect authorization rules.

## 7. Smart Shift Planning

- [ ] The smart planning workflow creates draft suggestions.
- [ ] Eligible employees are selected.
- [ ] Employees without a shift during the relevant week receive priority.
- [ ] Regeneration removes the relevant previous drafts.
- [ ] A manager can approve a suggestion.
- [ ] An approved suggestion cannot be approved again.
- [ ] A manager can discard an eligible draft.
- [ ] Discarding a draft does not affect actual shifts.

## 8. Subscription and Payments

- [ ] Package limits are applied correctly.
- [ ] Subscription information is synchronized correctly.
- [ ] Stripe test payments work in the configured test environment.
- [ ] Stripe webhook events are authenticated and processed safely.
- [ ] Failed or repeated payment events are handled correctly.

## 9. Responsive Design

- [ ] Main pages work on desktop screens.
- [ ] Main pages work on tablet screens.
- [ ] Main pages work on mobile screens.
- [ ] Forms and navigation remain usable on smaller screens.

## 10. Security

- [ ] Business data is isolated between businesses.
- [ ] Privacy Rules prevent unauthorized data access.
- [ ] Backend workflows enforce required authorization checks.
- [ ] File and attachment access is restricted appropriately.
- [ ] Sensitive API credentials are not exposed to users.

## 11. Test Status

All scenarios above are pending verification.

No scenario should be considered passed until it has been executed and its result recorded.
