# Product Management Skill

A comprehensive Claude skill that transforms AI into a strategic and tactical product management partner.

Unlike simple template-filling tools, it creates high-quality PRDs, FRDs, and user stories by analyzing your context, providing intelligent suggestions based on domain understanding, and validating every assumption before creating final documents.
## Why I Built This

I'm building this skill because there are many skills and plugins focused on making development and coding work easier, but few well-crafted projects focusing on product managers and product leaders.

Therefore, I created this project so product managers and product leaders can use it in their daily work, connecting with the Spec Driven Development process used in their teams, or in a "standalone" way, to facilitate routine work and research.

Product managers deserve AI tooling as sophisticated as what developers have. This skill bridges that gap.
## Who is this for?

- **Product Managers** creating specifications and requirements documents
- **Product Leaders** needing strategic analysis and documentation
- **Startup Founders** building product foundations
- **Engineering Teams** requiring clear product direction
- **Anyone** managing product development and delivery
## Core Principles
1. **Intelligent, Not Robotic**
    - Analyzes context to provide smart suggestions
    - Shows understanding of product domain
    - Explains reasoning behind recommendations
2. **Validation First**
    - Never includes unconfirmed assumptions in final documents
    - Always presents suggestions for user approval
    - Maintains quality through validation gates
3. **Context-Adaptive**
    - Adjusts approach based on information provided
    - Rich context → intelligent completions
    - Minimal context → targeted questions

## Key Features

- **Intelligent Suggestions**
    - Analyzes your context to propose smart completions for missing information
    - Provides reasoning behind suggestions instead of asking empty questions
    - Adapts approach based on how much context you provide
- **Quality Validation**
    - Never creates final documents with unvalidated assumptions
    - Always confirms suggestions before including them
    - Prevents generic, low-quality outputs
- **Comprehensive Templates**
    - **PRD** (Product Requirements Document) - Full product specifications
    - **FRD** (Feature Requirements Document) - Detailed feature specs
    - **Epic** - Large initiatives broken down into stories
    - **Items** - User stories, tasks, and bugs with acceptance criteria
- **🧠 Context-Aware Workflows**
    - **Rich Context Mode**: When you provide detailed information, it suggests completions
    - **Minimal Context Mode**: When you have just an idea, it asks targeted questions
    - **Existing Project Mode**: Analyzes codebase and docs before suggesting
## Why This Skill is Different

**Most AI tools treat product management like form-filling.** They ask generic questions, produce templated outputs, and force you to do all the strategic thinking.

**This skill is a strategic partner, not a secretary.** Here's how:

- **Intelligence Over Templates**
    - ❌ **Traditional**: "What are your success metrics?" → You do all the work
    - ✅ **This Skill**: "Based on this being a B2B SaaS platform, I suggest: User Activation (60% in 7 days), Feature Adoption (40% in 30 days), Retention (75% at 90 days). These align with typical SaaS benchmarks. Use these?"
- Context Understanding
    - ❌ **Generic Skills**: Same suggestions for every product type
    - ✅ **This Skill**: Analyzes your specific domain (marketplace, SaaS, platform, etc.) and provides contextually relevant recommendations
- **Quality Gates**
    - ❌ **Auto-generation Tools**: Create documents filled with assumptions and placeholders
    - ✅ **This Skill**: Never includes unvalidated information in final outputs. Every suggestion is confirmed first.
- Adaptability
    - ❌ **Fixed Workflows**: One-size-fits-all questionnaires
    - ✅ **This Skill**: Adjusts approach based on what you provide - from detailed requirements to vague ideas

**The difference:** This skill makes you a better PM by augmenting your strategic and tactical thinking, not replacing it.
## How It Works

### Example: Creating a PRD

**You provide:**

```
I want to create a PRD for a Ghost-Obsidian sync plugin that lets users 
manage Ghost CMS posts directly from Obsidian markdown files.
```

**Traditional approach (bad):**

```
What problem does this solve?
What are the success metrics?
Who are the users?
What features will it have?
```

**This skill (good):**

```
Based on this being a sync plugin for content creators, I understand:

PROBLEM: Writers switching between Obsidian (writing) and Ghost (publishing) 
creates friction and manual sync errors.

SOLUTION: Bidirectional sync plugin letting users manage entire editorial 
workflow from Obsidian.

SUCCESS INDICATORS I suggest:
- Sync Reliability: 99.5% conflict-free syncs
- Time Saved: 15 min/post reduction
- Adoption: 70% weekly active users after 30 days

Should I proceed with this TL;DR, or adjust any part?
```
## Usage

### Creating a PRD
Simply say:
- "Create a PRD for [your product idea]"
- "New PRD about [topic]"
- "Help me spec out [feature]"
### Creating an FRD
Say:
- "Create an FRD for [feature name]"
- "Detail out the [specific feature]"
### Creating User Stories
Say:
- "Create a story for [user capability]"
- "Break down [feature] into stories"
## File Structure

```
product-management/
├── README.md                    # This file
├── SKILL.md                     # Skill configuration
├── commands/
│   ├── spec.prd.md             # PRD creation workflow
│   └── spec.frd.md             # FRD creation workflow
├── rules/
│   └── rules-prod.md           # Core principles and standards
└── templates/
    └── product-spec/
        ├── template-prod-prd.md      # PRD template
        ├── template-prod-frd.md      # FRD template
        ├── template-prod-epic.md     # Epic template
        └── template-prod-issue.md    # Story/Task/Bug template
```
## References & Inspiration

This skill incorporates best practices from:

- **Product Strategy**: Roger Martin, Michael Porter, Gibson Biddle
- **Product Management**: Martin Cagan, Teresa Torres, Shreyas Doshi
- **Product-Led Growth**: Elena Verna, Aakash Gupta
## Contributing

Improvements welcome! Key areas:

- Additional templates (roadmaps, one-pagers, strategy docs)
- Domain-specific workflows (SaaS, marketplace, platform)
- Integration with project management tools
## Support

For issues or questions:

- Create an issue in this repository
- Share feedback through Claude.ai

---

**Version**: 1.0.0  
**Last Updated**: February 2025  
**Maintained by**: Diego Eis