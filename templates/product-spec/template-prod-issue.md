---
id:
  issue_type-001:
name:
  name of this issue:
type:
  Story:
  Task:
  Bug:
related_prd:
  related PRD path:
  example /master-docs/product/prd-001.md:
related_epic:
  related Epic name:
  example /master-docs/product/epics/epic-001.md. If it doesn't exist:
  ignore this line:
related_frd:
  related FRD path:
  example /master-docs/product/frds/frd-001.md:
created:
  YYYY-MM-DD:
updated:
  YYYY-MM-DD:
task_link:
  referential URL in $TASK_MANAGER - if it exists. If not:
  ignore this line:
status:
  icebox|in_review|in_progress|in_production|deprecated:
created_by:
  name of who created this doc:
last_editor:
  name of last editor:
---

# {id}: {name}

## Context
{Background: why this story is important, how it fits into the epic, what the problem is and how it solves it, related resources}

**As** {user type}
**I want** {capability}  
**So that** {benefit/value delivered}

## Acceptance Criteria
{Remember the difference in level of acceptance criteria from a PRD/Epic and Stories/Tasks mentioned in `SKILL.md`. Below is the example.}

```
#### Authentication Flow
- When the user clicks the "Login" button on the home page, the system displays the login modal
- When the user enters the email in the email field, the system validates the format in real-time
- When the user enters an invalid email format, the system displays the error "Enter a valid email" below the field
- When the user enters the password and clicks "Submit", the system attempts authentication
- When authentication is successful, the system closes the modal and redirects to the dashboard
- When authentication fails, the system displays the error "Invalid credentials" above the form
- When the user clicks the "Forgot my password" link, the system displays the password reset mode

#### Password Reset Flow
- When the user enters the email in the reset form and clicks "Send reset link", the system sends the reset email
- When the system sends an email, the system displays the confirmation "Check your email for the reset link"
- When the user doesn't receive the email within 1 minute, the system shows the "Resend email" button
```

## Technical Requirements

- **Implementation guidance**: {Suggestions, not requirements}
- **Performance requirements**: {If applicable}
- **Security considerations**: {If applicable}
- **Data requirements**: {If applicable}


## Edge Cases and Error Handling

1. **{Edge case 1}**: {How the system should handle}
2. **{Edge case 2}**: {How the system should handle}
3. **{Error scenario}**: {User-friendly error message and recovery}

## Out of Scope

- {What this story explicitly does NOT include}
- {Features deferred to future stories}


### Design Assets

- {Link to mockups/wireframes}
- {Link to prototypes}
- {Link to design specifications}

---
