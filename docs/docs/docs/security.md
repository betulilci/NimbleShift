# NimbleShift – Security

## 1. Overview

NimbleShift uses Bubble's built-in authentication, Privacy Rules, and workflow conditions to protect application data.

Security is designed around business ownership and user roles.

## 2. Authentication

The application uses Bubble User Authentication.

The configured password policy includes:

- Minimum 8 characters
- At least one number
- At least one uppercase letter
- At least one non-alphanumeric character

## 3. User Roles

NimbleShift has three main user roles:

- Yönetici
- Planlayıcı
- Personel

Access to application features is restricted according to user roles.

## 4. Business Data Isolation

Business-related records are designed to be accessible only to authorized users associated with the same business.

Privacy Rules use business ownership conditions to restrict access.

## 5. Workflow-Level Protection

Workflow conditions provide additional protection for important operations, including:

- Shift creation and approval
- Shift cancellation and exchange
- Leave approval and rejection
- Employee management
- Subscription package limits

## 6. Invitation Code Protection

Business invitation codes are treated as sensitive information.

Search access to invitation codes has been restricted to reduce the risk of unauthorized discovery.

## 7. Known Security Considerations

The following areas require further verification before public launch:

- Cross-business data isolation
- Field-level privacy and search permissions
- File and attachment access
- Invitation-code joining workflow
- Backend workflow authentication
- Stripe webhook security
- Role-based access across all pages and workflows

## 8. Payment Security

Stripe integration exists in the application, but payment processing and webhook behavior have not been fully validated.

Payments should not be considered production-ready until the integration is tested in an appropriate paid Bubble environment.

## 9. Security Status

Security improvements have been applied during development. However, this document does not represent a completed security audit or guarantee of production security.

A full security review is required before public launch.
