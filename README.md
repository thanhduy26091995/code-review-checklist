# code-review-checklist

## 1. Code Quality
- [ ] Code is clean, readable, and well-formatted
- [ ] Follows the project's coding conventions or style guide
- [ ] Uses meaningful variable, method and class names
- [ ] Avoid deep nesting and long functions
- [ ] No commented-out or un-used code blocks

## 2. Funcionality
- [ ] Code meets all business/functional requirements
- [ ] Handle edge cases and input validation
- [ ] Implements error handling and fallbacks
- [ ] All logic is covered by approriate tests

## 3. Security
- [ ] Inputs are validated and sanitized
- [ ] No hardcoded secrets or credentials
- [ ] Sensitive data is encrypted or masked appropriately
- [ ] Access controls and permissions are enforced
- [ ] No sensitive data leakage in logs or error message

## 4. Performance
- [ ] Code is optimized for performance
- [ ] Expensive operations are minimized or cached
- [ ] Efficient use of loops, memory and resources
- [ ] Async logic is used where appropriate

## 5. Maintainability
- [ ] Code is modular and separated by concern
- [ ] Duplicated logic is refactored (DRY principle)
- [ ] Avoids magic numbers and uses contants/configs
- [ ] Easy to understand, extend and test

## 6. Testing
- [ ] Unit tests cover core logic
- [ ] Integration and/or E2E tests cover main flow
- [ ] Tests are reliable and do not randomly fail
- [ ] Good test coverage for edge cases
- [ ] No dependencies on external system (use mocks)

## 7. Documentation
- [ ] Public classes/method are documented
- [ ] Complex logic is explained with comments
- [ ] API contracts and usage examples are provided
- [ ] README or usage guides are updated
- [ ] Database or insfrastructure changes are documented

## 8. Version Control
- [ ] Commits are small, atomic and meaningful
- [ ] No debug logs or temporary files commited
- [ ] Branch is up-to-date with base branch
- [ ] Pull request has clear description and context
- [ ] Related issues or tickets are referenced

## 9. Framework/Tooling Specific
- [ ] **Frontend**: Follows accessibility (a11y) best practices
- [ ] **Frontend**: Works on all supported devices and browsers
- [ ] **Mobile**: Manages lifecycle (foreground/background) well
- [ ] **Backend**: APIs follow REST/GraphQL best practices
- [ ] **Database**: Schema changes are backward-compatible

## 10. Deployment Readiness
- [ ] No environmnet-specific code or hardcoded paths
- [ ] Uses feature toggles for incomplete features
- [ ] CI/CD pipeline or deployment scripts are updated
