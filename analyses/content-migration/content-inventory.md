# Content Inventory: cncf/tag-contributor-strategy/website

## Executive Summary

This document provides a comprehensive inventory of all content in the `cncf/tag-contributor-strategy/website` directory that needs to be considered for migration to the new contribute.cncf.io information architecture.

**Content Overview:**
- **Total Content Areas:** 5 main sections
- **Key Content Types:** Markdown files, templates, guides, runbooks, newsletters, videos
- **Content Maturity:** Well-structured, comprehensive documentation with established patterns
- **Migration Complexity:** Medium - content is already well-organized but needs remapping

## Content Structure Analysis

### 1. **About Section** (`/about/`)
**Purpose:** Information about TAG Contributor Strategy and working groups

**Files:**
- `_index.md` (5,121 bytes) - Main about page with TAG overview
- `contributing.md` (6,956 bytes) - Contributing guidelines to the TAG
- `featured-background.jpg` (103,579 bytes) - Hero image
- `/working-groups/` directory with 6 working group pages

**Content Assessment:**
- ✅ Well-structured organizational information
- ✅ Clear contribution guidelines
- ⚠️ Working groups info may need restructuring for new IA

### 2. **Contributors Section** (`/contributors/`)
**Purpose:** Guidance for individual contributors

**Files:**
- `_index.md` (6,082 bytes) - Landing page for contributors
- `getting-started.md` (22,440 bytes) - Comprehensive getting started guide
- `projects.md` (1,479 bytes) - Project-related information

**Content Assessment:**
- ✅ Excellent getting started content
- ✅ Clear contributor paths
- ✅ Well-aligned with "Maintainers (The Individual)" category

### 3. **Maintainers Section** (`/maintainers/`)
**Purpose:** Resources for project maintainers

**Subsections:**
#### 3.1. Community (`/maintainers/community/`)
- `_index.md` (121 bytes) - Section overview
- `crm-runbook.md` (8,129 bytes) - CRM systems guidance
- `project-health.md` (10,051 bytes) - Project health metrics
- `recruiting-playbook.md` (5,784 bytes) - Contributor recruitment
- `vendor-neutrality.md` (9,741 bytes) - Vendor neutrality guidance
- `/contributor-growth-framework/` - Framework for contributor growth

#### 3.2. Governance (`/maintainers/governance/`)
- `_index.md` (570 bytes) - Section overview
- `charter.md` (4,830 bytes) - Charter guidance
- `leadership-selection.md` (7,595 bytes) - Leadership selection processes
- `overview.md` (6,448 bytes) - Governance overview
- `paperwork-checklist.md` (5,288 bytes) - CNCF paperwork requirements

#### 3.3. Security (`/maintainers/security/`)
- Security-related guidance (structure to be analyzed)

#### 3.4. Templates (`/maintainers/templates/`)
- `_index.md` (3,661 bytes) - Template overview
- `contributing.md` (10,019 bytes) - CONTRIBUTING.md template
- `governance-*.md` - 5 governance templates (49,514 bytes total)
- `issue-labels.md` (9,418 bytes) - Issue labeling template
- `maintainers.md` (2,870 bytes) - MAINTAINERS.md template
- `reviewing.md` (4,626 bytes) - PR review template
- `sample-instructions.png` (38,626 bytes) - Visual guide

**Content Assessment:**
- ✅ Comprehensive maintainer resources
- ✅ Well-organized by topic area
- ✅ Practical templates and runbooks
- ✅ Aligns well with "Projects (The Group)" category

### 4. **Accessibility Section** (`/accessibility/`)
**Purpose:** Accessibility guidance and resources

**Subsections:**
- `_index.md` (1,620 bytes) - Accessibility overview
- `/blind-and-visually-impaired/` - Resources for blind/VI community
- `/deaf-and-hard-of-hearing/` - Resources for deaf/HoH community

**Content Assessment:**
- ✅ Important specialized content
- ✅ Community-focused approach
- ✅ Aligns with "Community (The Group of Groups)" category

### 5. **Resources Section** (`/resources/`)
**Purpose:** Supporting resources, tools, and reference materials

**Content:**
- `_index.md` (214 bytes) - Section overview
- `glossary.md` (15,018 bytes) - Comprehensive glossary
- `templates.md` (223 bytes) - Template links
- `todogroup_resources.md` (2,863 bytes) - TODO Group resources

**Subsections:**
#### 5.1. How-To Guides (`/how-to/`)
- Practical guides for specific tasks

#### 5.2. Newsletters (`/newsletters/`)
- Historical project newsletters (multiple files)

#### 5.3. Project Services (`/project-services/`)
- CNCF services for projects

#### 5.4. Videos (`/videos/`)
- Video content organized by year (2020-2023)

**Content Assessment:**
- ✅ Rich supporting content
- ✅ Well-categorized resources
- ✅ Aligns with "Resources & Services" category

## Content Statistics

### File Count by Section
- **About:** 3 files + working-groups directory
- **Contributors:** 3 files
- **Maintainers:** 20+ files across 4 subsections
- **Accessibility:** 3+ files across 2 subsections  
- **Resources:** 10+ files across 4 subsections

### Content Size Analysis
- **Large Content Files (>10KB):**
  - `contributors/getting-started.md` (22,440 bytes)
  - `resources/glossary.md` (15,018 bytes)
  - `maintainers/templates/governance-subprojects.md` (15,448 bytes)
  - `maintainers/templates/governance-elections.md` (14,053 bytes)

- **Template Files:** 9 template files totaling ~70KB
- **Image Assets:** Multiple images including backgrounds and diagrams

### Content Maturity Assessment
- **High Quality:** Most content is well-written and comprehensive
- **Consistent Structure:** Good use of frontmatter and markdown conventions
- **Cross-References:** Extensive internal and external linking
- **Maintenance Status:** Actively maintained with recent updates

## Migration Considerations

### Content Gaps Identified
1. **Project Lifecycle Guidance:** Limited content on sandbox→incubating→graduated progression
2. **Staff Onboarding:** Minimal CNCF staff-specific content
3. **TAG Lead Resources:** Limited TAG-specific guidance
4. **Mentorship Integration:** Scattered mentorship references need consolidation

### Content Overlaps with Current Site
1. **Maintainer Guidance:** Significant overlap with existing docs/maintainers/
2. **Templates:** Similar templates exist in both repositories
3. **Accessibility:** Content exists in both locations
4. **Resources:** Some duplication in how-to guides and glossary

### Technical Migration Challenges
1. **Hugo → Docusaurus:** Content needs frontmatter conversion
2. **Link Updates:** Internal links need to be updated for new structure
3. **Asset Migration:** Images and other assets need to be moved
4. **Cross-References:** Extensive cross-referencing needs to be maintained

## Recommendations

### High Priority Content for Migration
1. **Contributor getting-started guide** - Foundational content
2. **Maintainer templates** - Practical tools actively used
3. **Project health guidance** - Core maintainer resources
4. **Accessibility content** - Specialized expertise

### Medium Priority Content
1. **Governance guidance** - Important but overlap exists
2. **Community building resources** - Valuable but can be phased
3. **Video content** - Rich content but migration complexity

### Low Priority Content
1. **Historical newsletters** - Archive value but less immediate need
2. **About/working groups** - Organizational info, lower migration priority

## Next Steps

1. **Create detailed mapping strategy** for each content area
2. **Identify canonical source decisions** for overlapping content
3. **Plan phased migration approach** starting with high-priority content
4. **Develop content templates** for new information architecture
5. **Establish content maintenance procedures** post-migration