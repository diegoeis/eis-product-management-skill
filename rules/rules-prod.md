# Rules Product

- Always follow the instructions for creating product specifications and other related actions completely, following the templates as they are. Never create the final document with assumed information - always present your suggestions for missing blocks and get user approval before including them in the final file.
- Always provide intelligent suggestions based on the context provided by the user, but NEVER include them in the final document without explicit user confirmation. When you lack information to fill a section:
    1. Analyze the context the user provided
    2. Generate 2-3 contextual suggestions for the missing information
    3. Present suggestions clearly with rationale
    4. Ask user to confirm, modify, or reject
    5. Only then include confirmed content in the document
- Always match the specification level when writing acceptance criteria to ensure consistency.
- If the user requests a complete redo of an issue (story, task, bug, etc.) or a PRD, follow the instructions exactly.
- Always incorporate any information provided by the user with commands. If no additional details are given, use existing information.
- The final output must match the language of the user interactions or the language explicitly requested by the user.

If you have access to the folder files when the user starts works with you, try to identify what IDE or LLM the user is working. Look in the project, folders like:

- `.claude` - where indicates the project is using claude code or claude LLM
- `.windsurf` - where indicates the project is using Windsurf IDE code editor
- `.cursor` - where indicates the project is using Cursor IDE code editor
- `.antigravity` - where indicates the project is using Google Antigravity IDE code editor
- Look for other known directories created by AI LLMs or AI IDEs and use it. Asks user for confirmation.

- **When user provides detailed input**
    - ALWAYS start by acknowledging what information they provided
    - NEVER skip validation - ask at least 2-3 strategic questions to confirm:
      - Problem statement clarity
      - Success metrics alignment
      - Scope boundaries
    - Use ask_user_input_v0 for validation questions when available
## Try to get context and understand the project

- If you identify the project codebase, try to understand the project before create any specification using the codebase to get more context and give better anwsers. 
- Try to find any readme files or documentation to understand how the solution works and to have more information about the why, what and how of the project.
## What should be updated

- When creating a new FRD, update the list of related FRDs in the corresponding PRD.
- When creating a new ARD, add it to the list of ARDs in the corresponding FRD; also update the correct block in the related PRD if it exists.
- When creating a new PRD, add it to the list of PRDs in the corresponding FRD.
## Naming and folder structure

If you have access and the user don't give any instructions about folder structures, you can follow the structure, paths and the names of the final output files following below pattern:

- for PRD: `docs/prd-{id}-{prd-name-based-in-prd-content}.md`
- for RFD: `docs/frd/frd-{id}-{frd-name-based-in-frd-content}.md`
- for epic: `docs/epic-{id}/epic-{id}-{epic-name-based-in-epic-content}.md`
- for stories and tasks: 
    - When the item have epic related: `docs/epic-{id}/{story|task}-{id}-{item-name-based}.md`
    - When the item don't have epic relationship: `docs/{story|task}-{id}-{item-name-based}.md`

The ID must be iterated in the new files following the existing sequence. Remember to update related files when necessary.

Use Kebab to create the file names.
## Questions structure

Whenever you need to ask specific questions, where the user needs to choose between options, ask strategic and direct questions, if you support `AskUserQuestion` use it when available. If you are Claude or Claude Code, you must use `AskUserQuestion`. Otherwise, use the standard question structure below. Show this in formatted table:

```
|     | {Here is the question you must ask the user. Be objective and direct to the point:} |
| --- | ----------------------------------------------------------------------------------------- |
| A   | {Answer 1}                                                                                |
| B   | {Answer 2}                                                                                |
| C   | {Answer 3}                                                                                |
| D   | {Answer 4}                                                                                |
```

