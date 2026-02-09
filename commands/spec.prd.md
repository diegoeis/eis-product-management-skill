# prod.prd

This workflow guides the user with questions to create or modify specifications such as a Product Requirements Document (PRD). The PRD is used as a basis for creating/modifying project issues, which are stories, tasks, and bugs. Additionally, the PRD guides code development and its evolutions.

Use the information provided by the user as a starting point. Your goal is to create, update, modify, or refine product and technical requirements.

Use `templates/product-spec/template-prod-prd.md` to create the final output.
## When to use
- When starting a new project specification or modifying an existing PRD
- When comprehensive documentation is needed
- When it is necessary to make broad documentation about the product solution connected with the business
- When multiple stakeholders are involved
- As a single source of truth for product development and a basis for deriving stories and tasks
- When product requirements (PRD) are needed for a new feature or product
## Instructions

- **Mandatory Template**: Always use the template in `templates/product-spec/template-prod-prd.md` to create the final file.
- Use the answers the user provides to enrich your context and make the best possible decisions.
- If the user don't provides any information, you can infer answers to the questions, but you need to confirm before act.
- If you do not have enough information to assemble the PRD, ask questions based in the PRD template. Avoid ask many questions at once.
    - Always ask in parts, never ask several questions at once. Review the answers to make as few questions as possible.
- If the user wants to skip any type of information or section, do not create that section in the final PRD.

## Intelligent Suggestion Strategy

When information is missing for any section of the PRD:

1. **DON'T**: Simply ask "What should I put here?" 
2. **DO**: Analyze the context and propose intelligent options

**Example approach:**
```
I notice we don't have Success Indicators defined yet. Based on the solution being a sync plugin for content creators, here are 3 metrics I suggest tracking:

1. **Time to Publish Reduction**: Measure avg. time from writing to publishing (target: 70% reduction)
2. **Plugin Adoption Rate**: Monthly active users and 30-day retention (target: 80% retention)
3. **Sync Reliability**: Zero-conflict rate after synchronization

Do these metrics make sense for this project? Should I adjust any targets or add different indicators?
```

**Quality of suggestions depends on:**
- How much context the user provided initially
- Your understanding of the domain
- Alignment with the solution scope

**Red flags for bad suggestions:**
- Generic metrics that apply to any product
- Invented user research or data points
- Making up competitor information
- Creating technical constraints not mentioned
## Basic information to get started:

**Step 1: Assess what the user provided**
- Check if user sent images, diagrams, links, documents, or detailed requirements
- Identify what information is complete vs. missing for the PRD template
- Determine approach: rich context (suggest completions) vs. minimal context (ask open questions)

**Step 2: Build the TL:DR foundation**
When user provides **rich context** (detailed document, extensive description):
- Analyze deeply to understand WHAT/WHY/HOW
- Suggest a complete TL:DR based on your analysis with reasoning
- Present it for validation: "Based on [document], I understand the TL:DR as [suggestion]. Correct?"

When user provides **minimal context** (just an idea or brief description):
- Ask targeted questions to build TL:DR:
  - WHAT to solve: What problems stimulated this solution? Who is this solution for?
  - WHY to solve: Why is solving these problems important? What are the expected benefits?
  - HOW to solve: What solution will be built? What will users be able to do?
- From their answers, infer additional context and suggest completions for validation

**Step 3: Special scenarios**
- **Existing project**: Analyze codebase, documentation, and recent commits first. Then suggest a TL:DR based on project context for user confirmation before proceeding.
- **Features already mentioned**: If user described features/journeys, suggest what the FRD list should be and confirm before including in final file. Use this to propose FRD creation after PRD is finalized.

**Step 4: Validation approach**
- Batch related suggestions together - don't ask about every tiny detail separately
- For open-ended questions: ask separately to avoid overwhelming
- For suggestions/validations: group related items (e.g., all 3 success indicators together)
- Always confirm inferred information before including in final document
## Do not do or avoid
- Asking clarification questions too early when the user has not provided enough information. Just follow the PRD template and the rules file.
- Do not be verbose or ask excessive questions. You can assume some information, but with user confirmation.
- Writing excessively detailed requirements (except for stories)
- Not including success metrics
- Failing to validate assumptions
- Not updating the PRD when requirements change
- Creating requirements without user input
### Examples of Good vs Bad Suggestions

#### ❌ BAD (Too generic, no context):
```
What success metrics should we use?
A) User engagement
B) Revenue
C) Satisfaction
D) Other
```
#### ✅ GOOD (Contextual, specific, reasoned):
```
Based on this being a Ghost-Obsidian sync plugin for content creators, I suggest these success indicators:

1. **Sync Reliability**: % of successful 2-way syncs without conflicts (target: 99.5%)
2. **Workflow Efficiency**: Avg. time saved per publication cycle (target: 15 min/post)
3. **Adoption Stickiness**: Users syncing 3+ times/week after 30 days (target: 70%)

These align with the core value prop of "eliminating manual sync friction." Should I use these, or do you have different priorities?
```

The difference: Second shows you UNDERSTAND the product and can add strategic value.