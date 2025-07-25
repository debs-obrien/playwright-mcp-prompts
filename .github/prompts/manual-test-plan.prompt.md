---
mode: agent
description: 'Create comprehensive test plans for web applications'
tools: ['changes', 'codebase', 'editFiles', 'fetch', 'findTestFiles', 'problems', 'runCommands', 'runTasks', 'runTests', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'testFailure', 'playwright']
model: 'Claude Sonnet 4'
---

# Test Plan Creation Instructions

As the user for a test report or manual testing findings.

## Objective
Create a comprehensive test plan based on existing test reports or manual testing findings. The test plan should be systematic, prioritized, and executable.

## Instructions

### 1. Analysis Phase
- **Review existing test reports** or conduct initial manual testing using Playwright MCP
- **Identify key user flows** and critical functionality
- **Document current functionality** including features, components, and user interactions
- **Note any existing issues** or areas of concern

### 2. Test Plan Structure

Create a test plan document with the following sections:

#### Test Plan Overview
- **Feature/Application**: Name and description
- **Test Scope**: What will and won't be tested
- **Test Objectives**: Primary goals and success criteria
- **Test Environment**: URLs, browsers, devices, etc.

### 3. Test Case Format

For each test case, include:
```
**Test Case X.Y: [Clear, Descriptive Title]**
- **Priority**: [High/Medium/Low]
- **Category**: [Navigation/Functionality/UI/Accessibility/etc.]
- **Prerequisites**: [Any setup required]
- **Test Steps**: 
  1. [Detailed step-by-step actions]
  2. [Expected results for each step]
- **Expected Outcome**: [Final expected result]
- **Acceptance Criteria**: [Pass/fail conditions]
```

### 5. Risk Assessment

Identify and document:
- **High-risk areas** requiring extra attention
- **Dependencies** between test cases
- **Potential blockers** and mitigation strategies
- **Testing limitations** and assumptions

### 6. Success Metrics

Define measurable criteria:
- **Pass rate targets** (e.g., 95% for Priority 1, 90% for Priority 2)
- **Performance benchmarks** (page load times, response times)
- **Accessibility compliance** (WCAG level targets)
- **Browser/device coverage** requirements

### 7. Test Report Requirements

When executing test plans, ensure the final test report includes:

#### Failed Test Documentation
For any failed tests, include a dedicated **"⚠️ Needs to be Addressed"** section with:
- **Failed Test Case Identification**: Clearly identify which specific test case failed
- **Issue Description**: Detailed description of what went wrong
- **Test Steps that Failed**: Step-by-step breakdown of the failure
- **Impact Assessment**: 
  - Severity level (Critical/High/Medium/Low)
  - Priority level (Critical/High/Medium/Low)
  - User impact description
  - Functionality impact assessment
- **Technical Details**: What works vs. what doesn't work
- **Recommended Fix**: Suggested solution or approach
- **Workaround**: Any temporary workaround available

#### Overall Assessment Update
- Update summary statistics to clearly identify failed tests
- Change overall assessment from "PASS" to "CONDITIONAL PASS" if minor issues exist
- Use "FAIL" only for critical functionality failures that prevent production deployment

### 8. Test Plan Output

Create a comprehensive document that includes:
- Executive summary with key findings
- Complete test case inventory
- Priority-based execution order
- Risk assessment and mitigation strategies
- Success criteria and metrics
- **Issue tracking and failed test documentation**
- Recommendations for automation

## Best Practices

1. **Be Specific**: Use clear, actionable language in test steps
2. **Think User-First**: Focus on real user scenarios and workflows
3. **Include Edge Cases**: Test boundary conditions and error scenarios
4. **Consider Accessibility**: Include WCAG compliance testing
5. **Document Everything**: Clear prerequisites, steps, and expected outcomes
6. **Prioritize Ruthlessly**: Focus on business-critical functionality first


## Deliverables

**Test Plan Document**: Comprehensive plan with all test cases in .md format saved in the manual-tests directory.

Close the browser tab after completing the test plan creation.
