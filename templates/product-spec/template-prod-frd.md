---
id:
  FRD-001:
name:
  name of this frd:
version:
  X.Y.Z - update whenever there is a change:
related_prd:
  related PRD path:
  example /master-docs/product/prd-001.md:
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

## TL;DR

- **What** to solve: 
  - {Problem statement 1: What is the core issue?}
  - {Problem statement 2: What are the existing pain points?}
  - {Problem statement 3: What opportunity are we addressing?}
- **Why** solve it: 
  - {Business impact 1: How does this benefit the business?}
  - {User benefit 1: How does this help users?}
  - {Strategic value: Why is this important now?}
- **How** to solve: 
  - {Solution approach 1: High-level solution concept}
  - {Solution approach 2: Key features/components}
  - {Differentiator: What makes this solution unique?}

## Introduction and Context
{This FRD describes the functional requirements specifications for the {Feature Name} functionality. It aims to guide development teams in the process of creating a feature that meets the planned standards for delivery and user expectations.}

{Provide 2-3 paragraphs (max 350 words) covering:
1. Current situation and pain points
2. User perspective and needs
3. Expected impact and success metrics related to this functionality

Remember that this FRD will be used by both humans and for training AI agents that will program or assist in code creation.}

## User Journey

{User interacts with the system through a sequence of actions leading to completion of the main task. Describe here the main steps of the user journey, including entry points, interactions, and decision points. Base this on the flow designed in design artifacts, using necessary files, or user inputs. If they don't provide it, don't assume, ask the user so we can create a complete and accurate journey.}

## Requirements and Criteria

{Remember that the criteria and requirements written in an FRD and PRD are different. In the FRD we should have much more detailed descriptions taking into account user behavior, with flow and action details. In the PRD, we should have more general and abstract requirements.

The requirements, acceptance criteria, and actions in an FRD define how the feature should work from the user's point of view and also the expected system behavior. They serve as a basis for validating whether the implementation is aligned with business and end-user expectations, in addition to serving as context for creating epics, stories, and tasks:

- Group criteria into clear, related blocks with titles and subtitles
- Include all possible scenarios and edge cases
- Be specific about UI elements and behavior, bringing flow and action details
- Include error states and validations
- Include technical criteria along with requirements, such as technologies, endpoints, tables, etc. If you don't have this information, ask the user:
  - Do you want to include technical criteria information now, or prefer to do it later?
  - If the user's answer is to do it later, continue inserting only requirements and acceptance criteria information, user behaviors and product flows.
  - If the user inserts technical criteria information, use it, placing them next to the requirement bullet point.

Follow the structure below to describe the requirements and acceptance criteria in the structure below:}

### RQT-1: Authentication Flow
- When the user clicks the "Login" button on the home page, the system displays the login modal
- When the user enters the email in the email field, the system validates the format in real-time
  - When the user enters an invalid email format, the system displays the error "Enter a valid email" below the field
- When the user enters the password and clicks "Sign In", the system attempts authentication
  - Information should be verified using the XYZ endpoint, which searches the ABC table in the Database Name database
- When authentication is successful, the system closes the modal and redirects to the dashboard
- When authentication fails, the system displays the error "Invalid credentials" above the form
- We must record in the XYZ audit database, the login failure or success information
- When the user clicks the "Forgot my password" link, the system displays the password reset mode

### RQT-2: Password Reset Flow
- When the user enters the email in the reset form and clicks "Send reset link", the system sends the reset email
- When the system sends an email, the system displays the confirmation "Check your email for the reset link"
- When the user doesn't receive the email within 1 minute, the system shows the "Resend email" button

## Dependencies

{Describe the dependencies this feature has to work correctly. Divide into blocks covering:
- Dependencies on other system features
- Data
- API services
- External tools, libraries or systems.

Examples:
- Integration with {GATEWAY NAME} payment API for payment processing
- [FRD-001 - FRD File Name](<link>)
- Chart library (version 3.0+)
- Email service (endpoint /api/email/send)
- Authentication feature (requires active login)
}

## Technical Requirements

{This block is dedicated to listing the technical decisions and architectures that were made for building the functionality. List all ARDs related to this FRD. If you don't know, ask the user.

If there aren't any or the user doesn't provide them, this block should not be included.}

```
- {[ARD-001](<path/to/file.md>): Clearly describe the technical decision}
- {[ARD-002](<path/to/file.md>): Describe a second technical decision}
- {[ARD-003](<path/to/file.md>): Describe a third technical decision}
```


## Epics and Issues Related to this FRD
{list all epics or issues related to this FRD}

- [EPIC-001 - Epic Name](<link>)
- [ISSUE-001 - Issue Name](<link>)

## History and Versioning

| Version | Date       | Description                  | Author        | 
|---------|------------|------------------------------|---------------|
| 1.0.0   | 2025-12-23 | Initial document version     | Health Team   |


---
