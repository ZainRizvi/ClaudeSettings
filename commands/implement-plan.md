---
allowed-tools: Task, Read, Glob, Grep, Bash(yarn test:*), Bash(yarn lint:*), Bash(yarn build:*), Bash(npx tsc:*), Write, Edit, MultiEdit
description: Implement a feature using comprehensive TDD workflow with iterative review cycles
---

Please implement the feature described in the plan document at: $ARGUMENTS

Use a comprehensive Test-Driven Development (TDD) workflow with multiple review cycles. I want you to follow this process:

## Phase 1: Planning & Architecture Review
1. **Initial Planning**: Read and understand the plan document, then create a detailed implementation strategy
2. **Senior Engineering Review**: Use the senior-code-reviewer agent to get comprehensive feedback on the approach
3. **Plan Iteration**: Refine the plan based on feedback and iterate until the senior-code-reviewer agent is satisfied with the approach

## Phase 2: Test Planning & Review
4. **Test Strategy Development**: Design comprehensive test coverage including unit tests, integration tests, and API tests as appropriate
5. **Test Review**: Use the test-reviewer agent to evaluate the test strategy for completeness and value
6. **Test Plan Refinement**: Iterate on test planning based on test-reviewer agent feedback until satisfied

## Phase 3: Test Implementation & Review
7. **Test Implementation**: Write all planned tests following TDD principles (tests should fail initially)
8. **Test Code Review**: Use the test-reviewer agent to get expert review of the actual test implementations for quality and effectiveness
9. **Test Iteration**: Refine tests based on test-reviewer agent feedback until the reviewer approves the test suite

## Phase 4: Feature Implementation & Debugging
10. **Implementation**: Implement the actual feature code to make tests pass
11. **Debugging Support**: Use the debugging-expert agent to resolve any unexpected test failures (expected initial failures are normal in TDD)
12. **Code Quality**: Ensure all tests pass and code meets quality standards

## Phase 5: Final Code Review
13. **Senior Code Review**: Use the senior-code-reviewer agent to get comprehensive review of the complete implementation
14. **Final Iteration**: Address any feedback and iterate until the senior-code-reviewer agent is satisfied with the final solution

Throughout this process:
- Follow strict TDD principles (red-green-refactor)
- Maintain high code quality and test coverage
- Ensure all implementations follow project conventions
- Run `yarn lint`, `yarn test`, and `yarn build` to validate changes
- Document any architectural decisions or trade-offs made
- **Use subagents to do most of the actual development work** (test writing, code implementation, debugging) to conserve your context window