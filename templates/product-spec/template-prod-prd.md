---
id:
  PRD-001:
name:
  name of this prd:
version:
  X.Y.Z - update whenever there is a change:
task_link:
  referential URL in $TASK_MANAGER. If it doesn't exist:
  remove this line:
created:
  YYYY-MM-DD:
updated:
  YYYY-MM-DD:
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

## Context

{Provide 2-3 paragraphs (maximum total of 200 words) covering:
1. Current situation and pain points
2. Business impact of not solving
3. User perspective and needs
4. Strategic importance}

### Problem or Opportunity Statement
{Write 2-3 paragraphs summarizing the problem or opportunity we are addressing, from a product point of view. Then, list the 3-6 main specific problems this PRD addresses. Focus on user pains and business impact.}

- {Specific and measurable issue: Clearly describe the problem or opportunity that directly impacts the user}
- {Another specific issue: Describe a second problem or opportunity that affects the user experience}
- {Third key problem: Describe a third problem or opportunity that represents a significant blocker}

## Solution
{Write a short, impactful sentence, without jargon and other exaggerations, of a maximum of 280 characters, that summarizes the solution. Ex.: We will build a solution that [describe the main solution in a clear and direct sentence] for [describe the target audience].}

{2-3 paragraph overview with a maximum of 200 words total, answering: What are we building? Why? For whom? Expected impact? Describe what the solution is and why it's the best solution. What is the opportunity cost of not doing this? The description of our solution and how it will help the user solve the problem and the company explore this opportunity.} 

*Listing of functionalities that make up the solution scope:*
{If there are no FRDs created or it's a new project, don't create this block. This block should be created if there are FRDs created or if the user explicitly states the functionalities.}

- **[FRD-{id}](<path/to/frd/file.md>) ({current FRD status - if it doesn't exist, don't include}):** [medium/high level specific capability, for example, "allow users to upload medical files and analyze this extracted data"]
- **[FRD-{id}](<path/to/frd/file.md>) ({current FRD status - if it doesn't exist, don't include}):** [medium/high level specific capability, for example, "identify patterns through data correlation"]  
- **[FRD-{id}](<path/to/frd/file.md>) ({current FRD status - if it doesn't exist, don't include}):** [key interaction, for example, "register with email/password, social networks and two-factor authentication"]
- **[FRD-{id}](<path/to/frd/file.md>) ({current FRD status - if it doesn't exist, don't include}):** [data requirement, for example, "persist user preferences"]

{
Avoid:
These two points could be unified, being part of a single functionality:
- [FRD-001]: The system MUST allow users to upload medical documents (PDFs, images) simply and securely
- [FRD-002]: The system MUST automatically extract structured data from medical documents (exam names, values, dates, laboratories)

Better would be:
- [FRD-001]: Allow upload of medical files and documents, allowing automatic extraction of structured data
}

### What this Initiative is Not

{Describe in a maximum of 150 words, what this initiative is not, what we don't solve because this is part of another scope of segments or services that we don't propose to work on. This statement is important to avoid misunderstandings and clearly delimit the scope. Validate with the user.

Example:
This solution is not a health information addition system like Apple Health, Google Fit, Fitbit, Garmin and others. It is a personal health data management system, which aggregates information from different sources and allows the user to manage and view their health data in a centralized way. It is not a medical diagnosis system, nor a medical prescription system.}

### Technical Solution Summary

{If there are already technical specifications in the project based on related ARDs, read and create a 2-3 paragraph summary, with a maximum of 100 words total. And list the main technical and architectural decisions in the format below. If there aren't any, this block should not be included.}

- **[ARD-{id}](<path/to/file.md>)**: Clearly describe the technical decision
- **[ARD-{id}](<path/to/file.md>)**: Describe a second technical decision
- **[ARD-{id}](<path/to/file.md>)**: Describe a third technical decision

## Success Indicators
These are indicators that can be used to measure the success of this solution.

{If not provided, suggest which business and/or product indicators and metrics should be monitored to understand success, and validate with the user. Follow the format below:}

- {Indicator 1: Clearly describe the success indicator}
- {Indicator 2: Describe a second success indicator}
- {Indicator 3: Describe a third success indicator}


## Scope

### Future Evolutions
{Put a list following the format below, of possible future evolutions. If the user provides, insert, if not suggest and ask for their confirmation. If they don't send nor accept your suggestions, say you will ignore this block.}

- **[FRD-{id}](<path/to/frd/file.md>) - {FRD name}** - ({default status for future evolutions is ICEBOX - Change status if user requests or FRD changes status}): {Relevant future considerations}  
- **[FRD-{id}](<path/to/frd/file.md>) - {FRD name}** - ({default status for future evolutions is ICEBOX - Change status if user requests or FRD changes status}): {Possible improvements and expansions}

### Out of Scope of this Initiative's Concept
{Make this list based on the WHAT THIS INITIATIVE IS NOT block}

- {Specific exclusion}  
- {Another exclusion}  
- {Additional exclusion}

## Artifacts and Documentation
- {Document 1: Link or reference to supporting document}
- {Document 2: Additional reference material}

