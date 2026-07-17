# AI in Medical Education Consortium - Project Instructions

## Project Overview

This repository contains resources, policies, curricula, and frameworks for the AI in Medical Education Consortium—a collaborative effort among academic health systems to share AI governance and educational materials.

## Key Files

- `RESOURCES.md` - Main resource collection with links to curricula, frameworks, policies, and videos
- `resources/Composite-GenAI-Policy-Guide.md` - Synthesized "best of the best" policy framework from member institutions
- `resources/Faculty-Development-Workflows.md` - Faculty Development Repository: AI workflows for faculty clinical, administrative, teaching, and scholarly tasks
- `resources/penn/` - Penn-specific policy and curriculum documents

## Policy Review Workflow

### When New Policies Are Submitted

When users share new AI policy documents or links (e.g., from chat threads, emails, or direct URLs):

1. **Fetch and Review Content**: Retrieve the policy document and extract key elements:
   - Core principles and philosophy
   - Acceptable/prohibited use guidelines
   - Data protection requirements
   - Disclosure and citation standards
   - Clinical documentation rules
   - Academic integrity provisions
   - Faculty responsibilities
   - Unique or innovative approaches

2. **Evaluate for Composite Inclusion**: Check if the policy contains elements that would strengthen the [Composite-GenAI-Policy-Guide.md](resources/Composite-GenAI-Policy-Guide.md):
   - Novel best practices not already covered
   - Clearer articulations of existing principles
   - New use cases or scenarios
   - Updated guidance reflecting evolving technology
   - Unique frameworks or tools (e.g., detection red flags, syllabus templates)

3. **Update Composite if Warranted**: If valuable new content is identified:
   - Add new sections or bullet points as appropriate
   - Credit the source institution
   - Maintain the document's synthesized, generalizable tone
   - Update the "Source Policies" section at the bottom

4. **Add to RESOURCES.md**: Add the new policy to the Policies & Governance section with:
   - Descriptive title
   - Brief summary of what it covers
   - Link to the document
   - Source attribution

### Composite Document Principles

The Composite-GenAI-Policy-Guide.md should:
- Remain institution-agnostic (generalizable to any medical school)
- Synthesize best practices rather than duplicate specific policies
- Prioritize actionable guidance over aspirational statements
- Include practical tools (tables, checklists, sample language)
- Be updated when new policies offer meaningfully better approaches

## Faculty Workflow Submissions

Consortium members email workflow suggestions with **#workflow** in the subject line; the maintainer forwards them here for incorporation.

### When a Workflow Submission Is Forwarded

1. **Extract the workflow elements**: name, category (clinical / administrative / teaching / scholarly), tools used and their security tier, steps, prompts, guardrails, and estimated time saved. If elements are missing, draft them from the description using clinical and scholarly best judgment — flag anything invented for the maintainer to verify.

2. **Format as a workflow card** in `resources/Faculty-Development-Workflows.md`, matching the existing entries' structure: problem it solves, what the workflow does, numbered steps, prompt starter, guardrails, and why it's worth it.

3. **Enforce the security framing**: every workflow must state its required tool security tier (EHR-integrated PHI-secure / enterprise no-retention / local model / any). Clinical workflows involving patient data must specify PHI-secure tools only. Scholarly workflows on unpublished work must specify no-retention or local tools.

4. **Update the Workflow Index table** at the top of the file and, if the workflow represents a new category, add a category section.

5. **Credit the contributor** and their institution (or note anonymity if requested).

6. **Update the RESOURCES.md Faculty Development Repository section** if the new workflow changes the "Current workflows include" summary.

## Resource Contributions

When adding any resource to RESOURCES.md:
- Place in the appropriate section (Curricula, Frameworks, Policies, Videos, Partners)
- Include a clear description
- Provide working links
- Add source attribution with institution name
