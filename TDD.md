# TDD.md

## Meta
Last updated: -
Owner: —  
Status: active

---

## 1. Testing Approach

Primary method:
Test-Driven Development (write test → make it pass → improve code)

Test distribution:
- Unit tests: majority
- Integration tests: moderate
- End-to-end tests: minimal

Coverage target:
Focus on critical logic, not 100% coverage

---

## 2. Test Environments

Local:
Developer runs tests before committing changes

CI:
Automated tests run on each push (optional)

Staging:
Used only if project grows (optional)

---

## 3. Test Categories

Unit:
Test small pieces of logic (functions, classes)

Integration:
Test how components work together

Contract:
Ensure APIs match expected inputs/outputs

E2E:
Test full user flow (minimal use)

Performance:
Basic checks for slow operations

---

## 4. Workflow (Red → Green → Refactor)

1. Write a failing test (define expected behavior)
2. Implement minimal code to pass the test
3. Refactor code while keeping tests passing
4. Update documentation and state

---

## 5. Feature Test Template

Feature name:

Requirement reference:
REQ.md#...

Context reference:
CONTEXT.md#...

Test cases:

- Happy path:
- Validation:
- Error handling:
- Edge cases:

Test data:
- Inputs
- Expected outputs

Exit criteria:
- All required tests pass
- No unstable tests
- No breaking changes

---

## 6. Regression Checklist

- Existing functionality still works
- No unexpected side effects
- Critical paths are tested

---

## 7. Quality Gates

Before completing any feature:

- Code passes all tests
- No major warnings or errors
- Core logic is covered by tests

---

## 8. Bug Tracking Template

| Bug ID | Found in | Test added | Root cause | Fix |
|--------|----------|------------|------------|-----|
| BUG-001|          | yes/no     |            |     |

---

## 9. Handling Flaky Tests

Rule:
Flaky tests must be fixed or removed

Process:
- Identify unstable test
- Fix root cause
- Avoid temporary ignores

Limit:
No long-term flaky tests allowed