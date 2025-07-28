# Content Organization Template for Future Content

## Overview

This template provides guidelines and templates for organizing content within the new information architecture for contribute.cncf.io. It ensures consistency, discoverability, and alignment with the service design mindset.

## Information Architecture Principles

### 1. Service Design Mindset
**"We provide projects a service"**

Every piece of content should clearly answer:
- **What service** does this content provide?
- **Who** is the primary audience?
- **What outcome** will users achieve?
- **How** does this connect to other services?

### 2. User Journey Orientation
Content should be organized around **what users want to achieve**, not organizational structure:
- **Individual Contributors:** "How do I start contributing?"
- **Project Maintainers:** "How do I maintain a healthy project?"
- **Community Leaders:** "How do I coordinate across projects?"
- **CNCF Staff:** "How do I support the community?"

### 3. Progressive Disclosure
Content should follow a **simple → detailed → expert** progression:
- **Overview:** High-level concept and value proposition
- **Getting Started:** Basic implementation steps
- **Advanced:** Complex scenarios and optimization
- **Reference:** Comprehensive technical details

## Content Templates by Category

### Template 1: Individual Contributor Content

#### File Structure Template
```
docs/contributors/
├── _index.md (overview and entry points)
├── getting-started.md (comprehensive onboarding)
├── [skill-area].md (e.g., code, documentation, design)
├── mentorship.md (mentorship programs and guidance)
└── career-paths.md (progression and recognition)
```

#### Content Template
```markdown
---
title: "[Topic Title]"
description: "One sentence describing the value this provides to individual contributors"
sidebar_position: [number]
tags: ["contributor", "individual", "[topic-specific-tags]"]
---

# [Topic Title]

## What You'll Learn
- [Specific outcome 1]
- [Specific outcome 2]
- [Specific outcome 3]

## Who This Is For
**Primary Audience:** [e.g., New contributors to CNCF projects]
**Prerequisites:** [e.g., Basic Git knowledge, GitHub account]
**Time Investment:** [e.g., 30 minutes to complete]

## Quick Start
[2-3 sentence summary with immediate next action]

## [Section 1: Core Content]
[Detailed guidance organized in logical steps]

## [Section 2: Advanced Topics]
[More complex scenarios and considerations]

## What's Next?
After completing this guide, you might want to:
- **Level Up:** [Link to more advanced content in same category]
- **Branch Out:** [Link to related content in other categories]
- **Get Help:** [Link to community resources]

## Related Resources
- [Link to complementary content]
- [Link to templates or tools]
- [Link to community discussions]

## Feedback
Was this helpful? [Link to feedback mechanism]
```

### Template 2: Project-Level Content

#### File Structure Template
```
docs/projects/
├── _index.md (project services overview)
├── lifecycle/
│   ├── _index.md
│   ├── sandbox.md
│   ├── incubating.md
│   ├── graduated.md
│   └── donation.md
├── governance/
│   ├── _index.md
│   ├── [governance-topic].md
├── health/
│   ├── _index.md
│   ├── metrics.md
│   └── assessment.md
├── community/
│   ├── _index.md
│   ├── [community-topic].md
└── templates/
    ├── _index.md
    └── [template-files].md
```

#### Content Template
```markdown
---
title: "[Project Service Title]"
description: "How this service helps CNCF projects succeed"
sidebar_position: [number]
tags: ["project", "maintainer", "[service-specific-tags]"]
---

# [Project Service Title]

## Service Overview
**What We Provide:** [Clear description of the service]
**Who It's For:** [Target projects - sandbox, incubating, graduated]
**When to Use:** [Timing and circumstances for using this service]

## Quick Access
- **Templates:** [Link to ready-to-use templates]
- **Tools:** [Link to assessment or implementation tools]
- **Support:** [Link to getting help with this service]

## Implementation Guide

### Step 1: [First Major Step]
[Clear instructions with success criteria]

### Step 2: [Second Major Step]
[Clear instructions with success criteria]

### Step 3: [Third Major Step]
[Clear instructions with success criteria]

## Common Scenarios

### For Sandbox Projects
[Specific guidance for early-stage projects]

### For Incubating Projects
[Specific guidance for growing projects]

### For Graduated Projects
[Specific guidance for mature projects]

## Troubleshooting
**Common Issue 1:** [Problem description]
- **Solution:** [How to resolve]
- **Prevention:** [How to avoid in future]

## Success Stories
[Brief examples of projects that have succeeded with this service]

## Support & Community
- **Questions:** [Where to get help]
- **Discussion:** [Community forums or channels]
- **Office Hours:** [Regular support sessions if available]

## Related Services
- **Before This:** [Prerequisites or foundational services]
- **After This:** [Next logical services to consider]
- **Complementary:** [Services that work well together]
```

### Template 3: Community Coordination Content

#### File Structure Template
```
docs/community/
├── _index.md (community services overview)
├── working-groups/
│   ├── _index.md
│   └── [group-name].md
├── accessibility/
│   ├── _index.md
│   └── [accessibility-topic].md
├── initiatives/
│   ├── _index.md
│   └── [initiative-name].md
├── staff/
│   ├── _index.md
│   ├── onboarding.md
│   └── [staff-topic].md
└── tag-leads/
    ├── _index.md
    └── [leadership-topic].md
```

#### Content Template
```markdown
---
title: "[Community Service/Initiative Title]"
description: "How this serves the broader CNCF community"
sidebar_position: [number]
tags: ["community", "coordination", "[initiative-specific-tags]"]
---

# [Community Service/Initiative Title]

## Mission & Scope
**Purpose:** [Why this initiative exists]
**Scope:** [What it covers and what it doesn't]
**Impact:** [How it benefits the broader community]

## Who's Involved
- **Leadership:** [Who leads this initiative]
- **Participants:** [Who can participate and how]
- **Stakeholders:** [Who benefits from this initiative]

## How to Participate

### For Individuals
[How individual contributors can get involved]

### For Projects
[How projects can participate or benefit]

### For Organizations
[How companies or organizations can contribute]

## Current Initiatives
[List of active work streams or projects]

## Resources & Tools
- **Documentation:** [Key resources and references]
- **Communication:** [Slack channels, mailing lists, meetings]
- **Collaboration:** [GitHub repos, project boards, tools]

## Success Metrics
[How the initiative measures success and impact]

## Governance
[How decisions are made and conflicts resolved]

## Getting Started
**New to this area?** [Entry point for newcomers]
**Ready to contribute?** [Next steps for those ready to engage]
**Want to lead?** [Path to taking on leadership roles]

## Related Community Efforts
[Links to complementary initiatives and working groups]
```

### Template 4: Resources & Services Content

#### File Structure Template
```
docs/resources/
├── _index.md (all CNCF services overview)
├── services/
│   ├── _index.md
│   └── [service-name].md
├── tools/
│   ├── _index.md
│   └── [tool-category].md
├── how-to/
│   ├── _index.md
│   └── [how-to-topic].md
├── templates/
│   ├── _index.md
│   └── [template-category]/
└── external/
    ├── _index.md
    └── [external-resource].md
```

#### Content Template
```markdown
---
title: "[Resource/Service Title]"
description: "What this resource provides and how to use it"
sidebar_position: [number]
tags: ["resource", "service", "[category-tags]"]
---

# [Resource/Service Title]

## What This Provides
[Clear description of the resource or service value]

## Who Can Use This
- **Eligibility:** [Who can access this resource]
- **Prerequisites:** [What's needed before using this]
- **Cost:** [Any costs or resource requirements]

## Quick Start
[Immediate next action to access or use this resource]

## Detailed Usage

### How to Access
[Step-by-step instructions for getting started]

### How to Use
[Guidance on effective usage]

### Best Practices
[Tips for getting the most value]

## Examples
[Real-world examples of successful usage]

## Limitations & Scope
[What this resource doesn't cover or provide]

## Support
- **Documentation:** [Additional technical documentation]
- **Community:** [Where to discuss or get help]
- **Issues:** [How to report problems or request enhancements]

## Related Resources
[Links to complementary tools and services]

## Updates & Changes
[How users stay informed about changes to this resource]
```

## Cross-Reference Patterns

### Standard Cross-Reference Sections

#### "What's Next?" Section Template
```markdown
## What's Next?

### Level Up
Ready for more advanced topics?
- [Advanced Topic 1](/docs/category/advanced-topic-1/) - [Brief description]
- [Advanced Topic 2](/docs/category/advanced-topic-2/) - [Brief description]

### Branch Out
Explore related areas:
- [Related Area 1](/docs/other-category/related-topic/) - [Brief description]
- [Related Area 2](/docs/other-category/related-topic/) - [Brief description]

### Get Support
Need help with implementation?
- [Community Discussion](/community/slack-channels/) - Ask questions and share experiences
- [Office Hours](/resources/office-hours/) - Get direct help from experts
- [Professional Services](/resources/services/consulting/) - Consider professional assistance
```

#### "Related Resources" Section Template
```markdown
## Related Resources

### Essential Tools
- [Tool 1](/docs/resources/tools/tool-1/) - [What it does]
- [Tool 2](/docs/resources/tools/tool-2/) - [What it does]

### Templates & Examples
- [Template 1](/docs/resources/templates/template-1/) - [What it provides]
- [Example Implementation](/docs/case-studies/example-1/) - [What you can learn]

### Community & Support
- [Working Group](/docs/community/working-groups/relevant-wg/) - [How they can help]
- [Special Interest Group](/docs/community/sigs/relevant-sig/) - [How they can help]
```

## Content Maintenance Guidelines

### Regular Review Process

#### Quarterly Review Checklist
- [ ] **Accuracy:** Are all facts and processes current?
- [ ] **Links:** Do all internal and external links work?
- [ ] **Relevance:** Is this content still serving its intended purpose?
- [ ] **Usage:** Is this content being used (analytics review)?
- [ ] **Feedback:** Has community feedback suggested improvements?

#### Annual Review Checklist
- [ ] **Alignment:** Does this content align with current strategy?
- [ ] **Gaps:** Are there new gaps this content should address?
- [ ] **Reorganization:** Would this content be better placed elsewhere?
- [ ] **Retirement:** Should this content be archived or removed?

### Content Ownership

#### Ownership Model
- **Primary Owner:** Subject matter expert responsible for accuracy
- **Secondary Owner:** Community representative who validates usefulness
- **Technical Owner:** Person responsible for maintenance and updates

#### Update Triggers
- **Immediate:** Factual errors, broken functionality
- **Weekly:** New resource availability, process changes
- **Monthly:** Community feedback integration
- **Quarterly:** Strategic alignment review

## Measurement & Optimization

### Content Performance Metrics

#### Quantitative Metrics
- **Usage:** Page views, time on page, user flows
- **Effectiveness:** Task completion rates, search success
- **Quality:** Link health, freshness, accuracy

#### Qualitative Metrics
- **User Feedback:** Comments, surveys, community discussions
- **Expert Validation:** Subject matter expert reviews
- **Community Adoption:** How widely content is referenced and used

### Continuous Improvement Process

1. **Monitor:** Regular review of analytics and feedback
2. **Identify:** Gaps, problems, and improvement opportunities
3. **Plan:** Prioritize improvements based on impact and effort
4. **Implement:** Make changes following templates and guidelines
5. **Validate:** Test with users and gather feedback
6. **Measure:** Assess impact and plan next improvements

## Implementation Checklist

### For New Content
- [ ] Content follows appropriate template
- [ ] Cross-references are comprehensive and bidirectional
- [ ] Content serves clear user journey and outcome
- [ ] All links are functional
- [ ] Content has been reviewed by subject matter expert
- [ ] Community feedback has been incorporated
- [ ] Analytics tracking is in place

### For Content Updates
- [ ] Changes align with template structure
- [ ] Cross-references are updated
- [ ] Related content is reviewed for consistency
- [ ] Breaking changes are communicated
- [ ] Redirects are in place if needed
- [ ] Update is tested with representative users

This template ensures that all content in the new information architecture serves users effectively, maintains consistency, and supports the overall goal of providing valuable services to the CNCF community.