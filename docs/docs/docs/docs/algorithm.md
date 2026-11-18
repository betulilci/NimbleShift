# NimbleShift – Smart Shift Planning Algorithm

## 1. Overview

NimbleShift includes a smart shift planning feature designed to help managers create shift suggestions based on staffing requirements and employee availability.

The planning logic is implemented using Bubble Workflows.

## 2. Planning Process

The current planning process follows these steps:

1. The manager defines staffing requirements.
2. The system starts the smart planning workflow.
3. The workflow evaluates eligible employees.
4. Employees are selected for shift suggestions.
5. Suggestions are saved as draft shifts.
6. The manager reviews the generated suggestions.
7. The manager can regenerate or discard suggestions.
8. Approved suggestions are converted into actual shifts.

## 3. Draft Shift Management

The application uses the `onerilen` field in the Vardiyalar data type to distinguish suggestions from actual shifts.

- `onerilen = yes`: The record is a draft suggestion.
- `onerilen = no`: The record is an actual shift.

This allows suggestions to be reviewed before becoming part of the real shift schedule.

## 4. Employee Selection

The current selection mechanism chooses randomly among eligible employees.

Employees who have no shift during the relevant week receive priority.

After employees without a shift have been prioritized, selection becomes random among the remaining eligible employees.

## 5. Regeneration

Managers can regenerate unapproved draft suggestions.

The regeneration process includes draft cleanup to prevent old suggestions from remaining alongside newly generated ones.

## 6. Approval

When a manager approves a suggestion, the application checks the approval conditions and converts the draft into a planned shift.

The approval workflow is designed to prevent the same suggestion from being approved more than once.

## 7. Current Limitations

The current algorithm is not a complete mathematical optimization system.

It does not guarantee globally optimal shift distribution or perfectly balanced working hours.

Advanced optimization, fairness scoring, and workload balancing may be considered in future development.

## 8. Implementation

The planning logic currently uses:

- Bubble Database
- Bubble Backend Workflows
- Bubble Workflow Conditions
- Employee eligibility checks
- Random employee selection

No external Python or SQL optimization service is currently used.
