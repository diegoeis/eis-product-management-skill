---
name: [Name from PRD]  
team: [Team Name]
created_at: [YYYY-MM-DD]
last_updated: [YYYY-MM-DD]  
---

# template-prod-breakdown

## Detailed Plan Summary (breakdown)

{3-4 sentences: What we're building, Why we're building it, how we'll solve it, and expected impact}

---

## Relationship with Deliverables

```
Version 1 {Period when provided. Otherwise, ignore this field}
  ├── Epic 1.1 {Date when provided. Otherwise, ignore this field}
  │ ├── Story/Task 1.1.1
  │ └── Story/Task 1.1.2
  └── Epic 1.2 {Date when provided. Otherwise, ignore this field}
      ├── Story/Task 1.2.1
      └── Story/Task 1.2.2

Version 2 {Period when provided. Otherwise, ignore this field}
  ├── Epic 2.1 {Date when provided. Otherwise, ignore this field}
  │ └── Story/Task 2.1.1
  └── Epic 2.2 {Date when provided. Otherwise, ignore this field}
      └── Story/Task 2.2.1
```

{After creating this relationship, ask to validate if the relationship is correct. This is important to avoid errors in the detailed plan.}

---

## Releases

### Version 1: {Name}

**Goal**: {What this version achieves. User's point of view, without technical details.}  
**Epics, stories and tasks included in this version**:
- {Epic name 1.1}
   - {Story 1.1.1}
   - {Story 1.1.2}
- {Epic name 1.2}
   - {Story 1.2.1}
   - {Story 1.2.2}

**Dependencies**:
- {write a list of dependencies based on the product design and technical gaps identified or not provided by the user}

**Risks and concerns**:
- {write a list of risks based on the product design and technical gaps identified or not provided by the user}

---

#### Epic 1.1: {Name}

**Outcome delivered**: {What this deliverable accomplishes}

**User expectations**: {As a user, what value does this epic offer?}

**Stories that make up this epic**:
1. {Story title 1.1.1}
2. {Story title 1.1.2}
3. {Story title 1.1.3}

**Acceptance criteria (epic level)**:
- [ ] {List of high-level criteria. This criterion is used to validate the epic and create detailed stories}

**Working days**: {sum of useful working days based on velocity or delivery deadline - if provided. Otherwise, ignore this field}

---

##### Epic 1.1.2: {Epic Name}

{Same structure as Epic 1.1.1}

---

### Version 2: {Name}

{Same structure as version 1}

---

## Dependencies and Sequencing

### Critical Path

```
Epic 1.1.1
   ↓
Epic 1.1.2 ──→ Epic 1.2.1
                   ↓
                Epic 2.1.1
```

### Dependency Matrix
{if asked to create the dependency matrix, create it. Otherwise, ignore this section}

| Epic | Depends on | Blocks | Status |
|------|------------|--------|--------|
| Epic 1.1.1 | - | Epic 1.1.2 | Not started |
| Epic 1.1.2 | Epic 1.1.1 | Epic 1.2.1 | Not started |
| Epic 1.2.1 | Epic 1.1.2 | Epic 2.1.1 | Not started |

### External Dependencies
{if asked to create external dependencies, create them. Otherwise, ignore this section}

- **{Dependency 1}**: {Description}
- **{Dependency 2}**: {Description}

---

## Risk Management
{if asked to create risk management, create it. Otherwise, ignore this section}

### High-level Risks

| Risk | Impact | Probability | Mitigation | Owner | Status |
|------|----|------------|------------|-------|--------|
| [Risk 1] | H/M/L | H/M/L | [Strategy] | [Name] | [Status] |
| [Risk 2] | H/M/L | H/M/L | [Strategy] | [Name] | [Status] |

### Contingency Plans

**If [Risk 1] occurs**:
1. [Action 1]
2. [Action 2]
3. [Fallback option]

**If [Risk 2] occurs**:
1. [Action 1]
2. [Action 2]
3. [Fallback option]

---
