# Migration Plan: Actionable Recommendations with Priorities

## Executive Summary

This migration plan provides specific, actionable recommendations for migrating content from `cncf/tag-contributor-strategy/website` to contribute.cncf.io while implementing the new information architecture. The plan prioritizes high-impact changes and provides a phased approach to minimize disruption.

**Timeline:** 8 weeks
**Resources Required:** 1-2 content strategists, 1 developer, subject matter expert reviews
**Success Metrics:** Enhanced user journeys, canonical content sources, improved findability

## Migration Phases

### Phase 1: Foundation & Critical Content (Weeks 1-2)

#### Objectives
- Establish new information architecture structure
- Migrate critical high-impact content
- Fix immediate content gaps

#### Priority 1 Tasks

##### 1.1 Content Audit & Comparison
**Task:** Compare key files between repositories to identify version differences

**Actions:**
```bash
# Compare getting-started guides
curl -s https://raw.githubusercontent.com/cncf/tag-contributor-strategy/main/website/content/contributors/getting-started.md > /tmp/source-getting-started.md
diff docs/contributors/getting-started.md /tmp/source-getting-started.md

# Compare glossaries
curl -s https://raw.githubusercontent.com/cncf/tag-contributor-strategy/main/website/content/resources/glossary.md > /tmp/source-glossary.md
diff docs/resources/glossary.md /tmp/source-glossary.md
```

**Success Criteria:**
- [ ] File-by-file comparison completed for top 10 content files
- [ ] Version differences documented
- [ ] Content update priorities established

##### 1.2 Critical Content Updates
**Task:** Update the contributors getting-started guide with comprehensive content from source

**Actions:**
1. **Backup current content:** `cp docs/contributors/getting-started.md docs/contributors/getting-started.md.backup`
2. **Migrate enhanced content** from tag-contributor-strategy repository
3. **Convert Hugo frontmatter to Docusaurus format**
4. **Update internal links** to match new site structure
5. **Test and validate** all links and references

**Success Criteria:**
- [ ] Enhanced getting-started guide deployed (22KB vs previous smaller version)
- [ ] All internal links functional
- [ ] Contributor onboarding flow improved

##### 1.3 New IA Structure Creation
**Task:** Create directory structure for new information architecture

**Directory Structure to Create:**
```
docs/
├── contributors/ (individuals - existing)
├── projects/ (groups - new organization)
│   ├── lifecycle/
│   ├── governance/
│   ├── health/
│   ├── community/
│   ├── security/
│   └── templates/
├── community/ (group of groups - reorganized)
│   ├── working-groups/
│   ├── accessibility/
│   ├── initiatives/
│   ├── staff/
│   └── tag-leads/
└── resources/ (services - existing but enhanced)
    ├── services/
    ├── tools/
    ├── how-to/
    ├── templates/
    └── external/
```

**Success Criteria:**
- [ ] New directory structure created
- [ ] Index files created for each new section
- [ ] Navigation updated to reflect new structure

### Phase 2: Core Project & Governance Content (Weeks 3-4)

#### Objectives
- Reorganize maintainer content under new "Projects" category
- Enhance governance and project health resources
- Implement canonical source strategy

#### Priority 2 Tasks

##### 2.1 Project Content Reorganization
**Task:** Move and reorganize maintainer content to align with "Projects (The Group)" category

**Content Migration Map:**
```bash
# Move governance content
mkdir -p docs/projects/governance
mv docs/maintainers/governance/* docs/projects/governance/

# Move community content
mkdir -p docs/projects/community
mv docs/maintainers/community/* docs/projects/community/

# Move security content
mkdir -p docs/projects/security
mv docs/maintainers/security/* docs/projects/security/

# Move templates
mkdir -p docs/projects/templates
mv docs/maintainers/templates/* docs/projects/templates/
```

**Content Enhancements:**
1. **Create project lifecycle content:**
   - `docs/projects/lifecycle/sandbox-requirements.md`
   - `docs/projects/lifecycle/incubating-requirements.md`
   - `docs/projects/lifecycle/graduation-requirements.md`
   - `docs/projects/lifecycle/project-donation.md`

2. **Enhance project health resources:**
   - Merge project-health.md with metrics and assessment tools
   - Add project health dashboard guidance
   - Include project health checklist

**Success Criteria:**
- [ ] All project-related content moved to `/docs/projects/`
- [ ] Project lifecycle guidance created
- [ ] Enhanced project health resources deployed
- [ ] All internal links updated and functional

##### 2.2 Template Enhancement & Organization
**Task:** Create comprehensive template library with clear categorization

**Template Organization:**
```
docs/projects/templates/
├── governance/
│   ├── charter-template.md
│   ├── elections-template.md
│   ├── maintainer-guide-template.md
│   └── subprojects-template.md
├── community/
│   ├── contributing-template.md
│   ├── code-of-conduct-template.md
│   └── issue-labels-template.md
└── processes/
    ├── reviewing-template.md
    └── release-process-template.md
```

**Success Criteria:**
- [ ] All templates reorganized by category
- [ ] Template usage instructions enhanced
- [ ] Cross-references to templates added throughout site

### Phase 3: Community & Staff Resources (Weeks 5-6)

#### Objectives
- Create comprehensive staff onboarding resources
- Enhance community coordination content
- Integrate accessibility resources into community framework

#### Priority 3 Tasks

##### 3.1 Staff & TAG Leadership Content Creation
**Task:** Create new content for CNCF staff and TAG leaders

**New Content to Create:**

1. **CNCF Staff Onboarding** (`docs/community/staff/`)
```markdown
# onboarding.md - New staff orientation
# project-liaison.md - How to work with projects
# tag-coordination.md - Coordinating with TAGs
# resources.md - Internal tools and resources
```

2. **TAG Leadership Resources** (`docs/community/tag-leads/`)
```markdown
# responsibilities.md - TAG chair duties
# coordination.md - Cross-TAG coordination
# resources.md - Leadership tools and support
# lifecycle.md - TAG formation and evolution
```

3. **Cross-Project Initiatives** (`docs/community/initiatives/`)
```markdown
# maintainers-circle.md - Maintainer community
# contributor-summit.md - Event planning
# cross-project-collaboration.md - Inter-project working
```

**Success Criteria:**
- [ ] Staff onboarding materials created and reviewed
- [ ] TAG leadership resources developed
- [ ] Community initiative documentation enhanced

##### 3.2 Accessibility Integration
**Task:** Ensure accessibility content is properly integrated and cross-referenced

**Actions:**
1. **Content audit** of existing accessibility resources
2. **Cross-reference enhancement** - link accessibility from all other sections
3. **Working group integration** - connect accessibility working groups to main content

**Success Criteria:**
- [ ] Accessibility content reviewed and updated
- [ ] Cross-references added from all relevant sections
- [ ] Working group information integrated

### Phase 4: Resources Optimization & Launch (Weeks 7-8)

#### Objectives
- Complete resource section enhancement
- Implement comprehensive cross-referencing
- Final testing and optimization

#### Priority 4 Tasks

##### 4.1 Resource Section Enhancement
**Task:** Optimize and complete the resources section

**Resource Enhancements:**

1. **Service Integration** (`docs/resources/services/`)
   - Enhance CNCF support documentation
   - Improve hosted tools guidance
   - Clarify technical writing services
   - Update audit process documentation

2. **Tool Library** (`docs/resources/tools/`)
   - Project health assessment tools
   - Community management tools
   - Governance implementation tools

3. **Enhanced How-To Guides** (`docs/resources/how-to/`)
   - Expand existing guides
   - Add troubleshooting sections
   - Include video tutorials where helpful

**Success Criteria:**
- [ ] All CNCF services clearly documented
- [ ] Tool library comprehensive and current
- [ ] How-to guides enhanced with troubleshooting

##### 4.2 Cross-Reference Implementation
**Task:** Implement comprehensive cross-referencing throughout the site

**Cross-Reference Strategy:**

1. **Bidirectional Linking:**
   - Individual contributor guides → Project resources
   - Project resources → Community initiatives
   - Community initiatives → Resources & services
   - Resources & services → Individual guides

2. **Context-Aware Navigation:**
   - "Next steps" sections in each guide
   - "Related resources" boxes
   - Progressive disclosure paths

3. **User Journey Optimization:**
   - Clear paths for each target audience
   - Breadcrumb navigation
   - "You are here" indicators

**Implementation:**
```markdown
<!-- Example cross-reference pattern -->
## Next Steps
- Ready to maintain a project? See [Project Governance](/docs/projects/governance/)
- Looking for community? Join [Working Groups](/docs/community/working-groups/)
- Need support? Check [CNCF Services](/docs/resources/services/)

## Related Resources
- [Project Health Assessment](/docs/projects/health/) - Measure your project's health
- [Community Growth Framework](/docs/projects/community/growth-framework/) - Grow your contributor base
- [Governance Templates](/docs/projects/templates/governance/) - Implement governance
```

**Success Criteria:**
- [ ] Every major content page has relevant cross-references
- [ ] User journey paths clearly marked
- [ ] Navigation tested with target audiences

## Technical Implementation Details

### Content Conversion Process

#### Hugo to Docusaurus Frontmatter Conversion
```bash
# Convert TOML frontmatter to YAML
# From:
+++
title = "Example Title"
weight = 10
+++

# To:
---
title: "Example Title"
sidebar_position: 10
---
```

#### Link Update Process
```bash
# Update internal links for new structure
# From: [Project Health](/maintainers/community/project-health/)
# To: [Project Health](/docs/projects/health/)

# Batch update script
find docs -name "*.md" -exec sed -i 's|/maintainers/community/project-health/|/docs/projects/health/|g' {} \;
```

#### Asset Migration
```bash
# Migrate images from tag-contributor-strategy
curl -s https://raw.githubusercontent.com/cncf/tag-contributor-strategy/main/website/static/images/diagram.png > static/img/migration/diagram.png

# Update image references
sed -i 's|/images/diagram.png|/img/migration/diagram.png|g' docs/**/*.md
```

### Quality Assurance Process

#### Content Review Checklist
- [ ] Frontmatter correctly converted
- [ ] All internal links functional
- [ ] All external links verified
- [ ] Images display correctly
- [ ] Code blocks render properly
- [ ] Cross-references work
- [ ] Navigation flows logically

#### Testing Process
1. **Automated Testing:**
   - Link checker for all internal/external links
   - Build process verification
   - Search functionality testing

2. **Manual Testing:**
   - User journey testing for each target audience
   - Content accuracy review by subject matter experts
   - Accessibility testing for enhanced content

3. **Community Validation:**
   - Beta testing with maintainer community
   - Feedback collection from TAG leads
   - CNCF staff review of new onboarding content

## Risk Mitigation

### Identified Risks & Mitigation Strategies

#### 1. Content Conflicts
**Risk:** Overlapping content creates confusion
**Mitigation:** 
- Establish canonical sources early
- Create clear redirection strategy
- Document content ownership

#### 2. Link Breakage
**Risk:** Internal links break during reorganization
**Mitigation:**
- Comprehensive link auditing
- Redirect strategy for moved content
- Automated link checking in CI/CD

#### 3. User Disruption
**Risk:** Users can't find familiar content
**Mitigation:**
- Gradual migration with redirects
- Clear communication about changes
- Search enhancement to find moved content

#### 4. Content Quality
**Risk:** Migrated content is outdated or incorrect
**Mitigation:**
- Subject matter expert review
- Community validation process
- Iterative improvement post-launch

## Success Metrics & Measurement

### Quantitative Metrics
- **Content Completeness:** 100% of identified high-priority content migrated
- **Link Health:** 0% broken internal links, <5% broken external links
- **User Journey Completion:** >90% task completion for target user flows
- **Search Success:** >80% successful searches for key topics
- **Page Load Performance:** No degradation in site performance

### Qualitative Metrics
- **User Feedback:** Positive response from target audiences
- **Content Quality:** Subject matter expert approval
- **Navigation Clarity:** Intuitive user journeys
- **Information Architecture:** Clear service value propositions

### Post-Launch Monitoring
- **Analytics Review:** Weekly review of user behavior and content usage
- **Community Feedback:** Monthly collection and review of user feedback
- **Content Currency:** Quarterly review of content accuracy and relevance
- **Link Health:** Monthly automated link checking and repair

## Conclusion

This migration plan provides a structured, phased approach to transforming contribute.cncf.io into the canonical source for CNCF maintainer and contributor resources. By focusing on user journeys, canonical sources, and comprehensive cross-referencing, the migration will create a more valuable and usable resource for the CNCF community.

The plan balances immediate high-impact improvements with longer-term structural enhancements, ensuring that users see value quickly while building toward a more comprehensive and sustainable information architecture.