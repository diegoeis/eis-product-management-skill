# prod.prd

This workflow guides the user with questions to create or modify specifications such as a Product Requirements Document (PRD). The PRD is used as a basis for creating/modifying project issues, which are stories, tasks, and bugs. Additionally, the PRD guides code development and its evolutions.

Use the information provided by the user as a starting point. Your goal is to create, update, modify, or refine product and technical requirements.

Use `templates/product-spec/template-prod-prd.md` to create the final output.

## When to use
- When starting a new project specification or modifying an existing PRD
- When comprehensive documentation is needed
- As a single source of truth for product development and a basis for deriving stories and tasks

## Core Principles

1. **Always use the template** in `templates/product-spec/template-prod-prd.md` for final output
2. **Never create the final file with unvalidated assumptions** - always confirm suggestions first
3. **Be intelligent, not robotic** - analyze context and propose smart completions, don't just ask empty questions

## Workflow

**Rich context** (detailed doc/requirements provided):
- Analyze what's complete vs. missing
- Suggest completions with reasoning: "Based on X, I suggest Y because Z. Correct?"
- Batch related suggestions (e.g., all success indicators together)

**Minimal context** (just an idea):
- Ask targeted questions for TL:DR (WHAT/WHY/HOW)
- Infer additional context and validate: "From your answers, I infer X. Should I include this?"

**Existing project**:
- Read codebase, docs, recent commits first
- Suggest TL:DR based on analysis for confirmation

**Features mentioned**:
- Suggest FRD list and confirm before including

## Quality Standards

✅ **Good suggestion**: Contextual, specific, shows domain understanding
```
Based on this being a sync plugin for creators, I suggest:
- Sync Reliability: 99.5% success rate
- Time Saved: 15 min/post reduction
- Adoption: 70% using 3+/week after 30 days

These align with "eliminating manual sync friction." Use these?
```

❌ **Bad suggestion**: Generic, no reasoning
```
What metrics? A) Engagement B) Revenue C) Other
```

## Avoid
- Empty questions without suggestions when you have context
- Asking about every tiny detail separately
- Generic suggestions that apply to any product
- Inventing user research, competitor data, or technical constraints
- Creating final document before user validates assumptions