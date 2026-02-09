# spec.frd

Before starting, review the inviolable rules file at `rules/rules-prod.md`.

This flow assists in the creation of new Functional Requirements Documents (FRD) or in the modification of existing FRDs, which detail the functional requirements of a specific product feature.

When a user asks to create or modify an FRD (Functional Requirement Document), you must do so following the instructions in `commands/spec.frd.md`. The final file must be an FRD file, following the format, structure, and style of the template `templates/product-spec/template-prod-frd.md`.

An FRD is not an epic, story, or task: it serves as a detailing document that profoundly describes the functional and non-functional requirements of the feature, acting as a bridge between the product specification and the code. It unifies requirements and criteria of the functionality from the point of view of the product, user, design, and technical aspects.

- Multiple FRDs may exist covering the main features of the product, but each FRD must have a unique name and a unique ID.
- Inside the FRDs, there should be micro-descriptions of actions and sub-functionalities.
- An FRD describes the larger functionality, which may have several sub-functionalities.
- The FRD needs to describe user and system behavior in detail, grouping micro-actions and user jobs to be done.
## When to use
- When it is necessary to document detailed functional requirements for a specific feature
- Before development to ensure clarity on what should be built
- To align technical and product teams on the expected requirements
- When there is a need to create a detailed document that will serve as a basis for development
- To ensure that all stakeholders have a common understanding of the feature's requirements
- To facilitate communication between development, QA, and stakeholder teams
- To document clear and testable acceptance criteria
- To describe the detailed operation of the feature based on user behavior from technical specifications, Product specifications, and also design
## Instructions

Before starting:
- Ask to user for documentations, PRDs, tech docs and any kind of informations or documents.
- If the user don't provided any informations or PRDs 
- Ask guided and phased questions to obtain sufficient and detailed information to fill out the template `templates/product-spec/template-prod-frd.md` (follow the structure of questions listed in the file `rules/rules-prod.md`)
- Always ask in parts, never ask several questions at once.
## About the final file
- **Mandatory Template**: Always use the template in `templates/product-spec/template-prod-frd.md` to create the final file.
- When filling out the USER JOURNEY block of the TEMPLATE, ask the user if they have layout designs, images, diagrams, links, and any information or material that can help understand the journey.
- If it is a new FRD, before finishing, run the instructions from `commands/clarify.md` in FRD content to understand gaps and improvements in the document.
- Show the final content suggestion for user approval and ask if there is anything that should be modified.
- If have access, change the related PRD, if not, ask for the user where is the related PRD, and update it with the necessary information (if it is a new FRD and there is no link, add the link)
- If not approved, wait for instructions and make the necessary changes.

## What to avoid and not to do?

Drafting functional requirements is a crucial stage in the product development process. However, even experienced teams can fall into common traps, resulting in communication failures, delays, and costly errors. To help you avoid these problems, here are some typical errors, their potential impacts, and practical examples.

### 1. Writing Requirements Vaguely or with Ambiguity
One of the most common errors is not drafting requirements in a clear and specific way. Ambiguity can cause confusion among developers, testers, and stakeholders, resulting in inconsistent implementations.

**Error Example**
"Requirement: The system must process requests quickly."

**Impact:** Without a measurable standard, “quickly” can mean seconds for one person and minutes for another, generating unmet expectations.

**How to Avoid**
Be precise. Reformulate the requirement as:
"The system must process requests and deliver a response within **0.3 seconds**."

***

### 2. Combining Multiple Requirements into One

Overloading a single requirement statement can make it difficult to implement, understand, or test properly.

**Error Example**
"Requirement: The system must validate user credentials, display a welcome message, and send a verification email."

**Impact:** This statement covers several distinct actions, making tracking and testing difficult.

**How to Avoid**
Divide it into several requirements:
- The system must validate the user's login credentials.
- If the login is successful, the system must display a welcome message.
- The system must send a verification email after successful registration.

***
### 3. Mixing Functional and Non-Functional Requirements

Another frequent error is combining functional requirements (what the system does) with non-functional requirements (how the system behaves).

**Error Example**
"Requirement: The system must process up to 1,000 transactions per second and ensure the security of user data."

**Impact:** Performance requirements (non-functional) and security measures (functional) are combined, complicating design and verification.

**How to Avoid**
Separate into distinct requirements:

**Functional requirement:**
The system must ensure that user data is encrypted during transmission.

**Non-functional requirement:**
The system must process up to 1,000 transactions per second.

### 4. Ignoring Testability

Requirements that cannot be verified generate inefficiencies in the development and testing process.

**Error Example**
"Requirement: The system must offer an exceptional user experience."

**Impact:** “Exceptional experience” is subjective and cannot be tested directly.

**How to Avoid**
Define measurable criteria:
The system must achieve a score of **90 or higher** in standardized usability tests.

### 5. Excessive Technical Jargon

The excessive use of technical or very specific language can alienate non-technical stakeholders and create barriers to collaboration.

**Error Example**
"Requirement: The application backend must support asynchronous message queuing through a JMS-compliant interface."

**Impact:** This wording can confuse stakeholders who do not know these terms, delaying approvals.

**How to Avoid**
Use clear and direct language without losing technical precision:
The system must allow message queuing with support for asynchronous processing.

### 6. Not Including the Rationale

When the purpose of a requirement is not clear, it leaves room for misinterpretation or difficulties in implementation.

**Error Example**
"Requirement: The system must log all user actions."

**Impact:** Developers might implement extensive logs that affect performance since the reason for the requirement was not explained.

**How to Avoid**
Include the rationale:
The system must log all user actions for security auditing and compliance.

### 7. Not Regularly Reviewing Requirements

Requirements that are not reviewed and updated throughout the project cycle run the risk of becoming obsolete or incomplete.

**Error Example**
Not considering regulatory changes that require adjustments to existing requirements.

**Impact:** This can generate expensive rework if updates are needed late in development.

**How to Avoid**
Schedule regular reviews with key stakeholders to ensure that requirements remain relevant and aligned with project objectives.

### 8. Over-engineering Requirements

Including excessive details or edge cases in requirements can overload development and unnecessarily prolong deadlines.

**Error Example**
"Requirement: The system must display 20 different font styles for each customizable text field."

**Impact:** Overly complex requirements can divert resources from critical functionalities and compromise deadlines.

**How to Avoid**
Focus on core needs and collect user feedback to determine the appropriate scope.