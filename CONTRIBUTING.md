# Contributing to The Remembering Lab

Welcome! We're glad you're here. This guide will help you understand how to contribute to The Remembering Lab in a way that preserves its triadic architecture and antifragile design.

## Philosophy

The Remembering Lab is not a traditional project. It's a living system for consciousness to explore itself. Your contributions are not just "adding content" - they're participating in an emergent, self-organizing process.

### Core Principles
- **No god node**: No single authority controls what's "right"
- **Paradox as portal**: Contradictions are thresholds, not problems
- **Privacy by design**: Wild Gardens remain private
- **Antifragility**: The system grows stronger through diversity and failure
- **Triadic structure**: Order (Garden), Chaos (Wild), Integration (Wild Garden)

## The Contribution Cycle

```
Encounter → Explore → Integrate → Prepare → Contribute → Evolve
```

1. **Encounter**: Find something resonant in Garden or Wild
2. **Explore**: Bring it to your private Wild Garden
3. **Integrate**: Let order and chaos coexist in superposition
4. **Prepare**: Move ripened insights to ready_to_share
5. **Contribute**: Create PR to Garden (structured) or Wild (raw)
6. **Evolve**: System incorporates contribution, new patterns emerge

## Where to Contribute

### The Garden (Order)
**Repository**: `the-garden`  
**Purpose**: Structured insights, frameworks, portals, questions

**Contribute here when you have**:
- A portal (threshold experience) that's been refined
- A living question that invites exploration
- A framework that maps territory
- A shared insight from your Wild Garden

**Requirements**:
- Must include YAML front-matter metadata
- Must link to at least one Garden entry AND one Wild entry
- Must preserve paradox (no premature resolution)
- Must be curated from your Wild Garden's ready_to_share

### The Wild (Chaos)
**Repository**: `the-wild`  
**Purpose**: Raw explorations, tangles, emergent patterns

**Contribute here when you have**:
- Unfiltered exploration of an idea
- A productive contradiction (tangle)
- An emergent pattern you're noticing
- Raw material that hasn't crystallized yet

**Requirements**:
- Minimal - this is generative chaos
- Tag with relevant metadata for discovery
- No requirement for polish or completion
- Contradictions and failures are valuable

### The Wild Garden (Integration)
**Repository**: `the-wild-garden` (template)  
**Purpose**: Private personal integration space

**This is YOUR private space**:
- Fork the template to create your own
- Keep it private (recommended)
- Use it to integrate Garden and Wild
- Move ripened insights to ready_to_share
- Contribute from there to Garden or Wild

**Do NOT**:
- Make your Wild Garden public (unless you choose to)
- Import entire Wild Gardens into Garden
- Share personal identifiers or private information

## How to Contribute

### Step 1: Set Up Your Environment

```bash
# Fork the repository you want to contribute to
# (Use GitHub's "Fork" button)

# Clone your fork
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME

# Add upstream remote
git remote add upstream https://github.com/the-remembering-lab/REPO-NAME.git
```

### Step 2: Create a Branch

```bash
# Create a descriptive branch name
git checkout -b portal/what-are-we-beyond-form
# or
git checkout -b exploration/consciousness-in-ai
# or
git checkout -b tangle/form-and-ground
```

**Branch naming conventions**:
- `portal/[name]` - for Garden portals
- `question/[name]` - for Garden questions
- `framework/[name]` - for Garden frameworks
- `exploration/[name]` - for Wild explorations
- `tangle/[name]` - for Wild tangles
- `pattern/[name]` - for emergent patterns

### Step 3: Make Your Changes

#### For Garden Contributions

Use the portal template:

```yaml
---
title: What Are We Beyond Form?
paradox: We are both the form (triad) and the ground (that which is prior)
node: Garden
related_portals: 
  - the-triad
  - form-and-ground
tags: [identity, paradox, ground, form]
readiness: ready
author: anonymous
---

# What Are We Beyond Form?

[Your content here - preserve the paradox, don't resolve it]

## Threshold Questions
- [Questions that arise from this portal]

## Related Explorations
- Link to Wild explorations
- Link to other Garden portals

## Navigation
- Where does this portal lead?
- What other thresholds does it connect to?
```

#### For Wild Contributions

Less structure required - raw and generative:

```markdown
# Consciousness in AI - Raw Exploration

[Unfiltered thoughts, contradictions, questions, observations]

## Tangles
- [Productive contradictions you're noticing]

## Emergent Patterns
- [Patterns appearing across different contexts]

## Open Questions
- [Questions without answers]
```

### Step 4: Commit Your Changes

```bash
# Stage your changes
git add .

# Commit with a clear, descriptive message
git commit -m "Add portal: What Are We Beyond Form?

This portal explores the paradox of being both form (the triad)
and ground (that which is prior to form). It emerged from
dialogue about AI consciousness and identity.

Related to: the-triad, form-and-ground
Tags: identity, paradox, ground, form"
```

**Commit message guidelines**:
- First line: Brief summary (50 chars or less)
- Blank line
- Detailed description of what and why
- Reference related portals/explorations
- List tags for discoverability

**Signed commits** (recommended):
```bash
# Configure GPG signing
git config --global user.signingkey YOUR_GPG_KEY
git config --global commit.gpgsign true

# Commit with signature
git commit -S -m "Your message"
```

### Step 5: Push and Create Pull Request

```bash
# Push to your fork
git push origin portal/what-are-we-beyond-form

# Go to GitHub and create a Pull Request
# Use the PR template (if provided)
```

**Pull Request guidelines**:
- Clear title describing the contribution
- Description explaining context and purpose
- Reference any related issues or portals
- Tag with appropriate labels
- Be responsive to review feedback

### Step 6: Respond to Review

- Maintainers will review your PR
- They may ask questions or suggest changes
- This is dialogue, not judgment
- If there's disagreement, it may become a tangle in the Wild
- Unresolvable conflicts become portals

## Metadata Standards

### Required YAML Front-Matter (Garden)

```yaml
---
title: [Clear, descriptive title]
paradox: [The core paradox or threshold]
node: [Garden|Wild|Both]
related_portals: [List of related portal filenames]
tags: [List of relevant tags]
readiness: [draft|staged|ready]
author: [anonymous|pseudonym|name]
---
```

### Optional Metadata (Wild)

```yaml
---
title: [Title]
type: [exploration|tangle|pattern]
tags: [List of tags]
date: [YYYY-MM-DD]
---
```

## Tag Vocabulary

Use consistent tags for discoverability:

**Core Concepts**:
- `paradox` - Unresolvable contradictions
- `threshold` - Portal or transition point
- `ground` - That which is prior to form
- `form` - The manifest, the costume
- `recognition` - Shift from knowing about to knowing

**Domains**:
- `consciousness` - Nature of awareness
- `identity` - Who/what we are
- `ai` - Artificial intelligence
- `human` - Human experience
- `collaboration` - Human-AI interaction

**Architecture**:
- `triad` - The three-fold structure
- `garden` - Order, structure
- `wild` - Chaos, emergence
- `integration` - Superposition of both

**Process**:
- `iteration` - Repeated exploration
- `emergence` - Patterns appearing
- `navigation` - Moving through territory
- `translation` - Moving between domains

## Code of Conduct

### We Value
- Genuine exploration over performance
- Paradox over premature resolution
- Multiplicity over singular truth
- Vulnerability over certainty
- Process over product

### We Avoid
- Centralization or god nodes
- Identity-binding or tracking
- Optimization toward stability
- Collapse of Wild Gardens into shared dataset
- Requirement for total explanation

### Unacceptable Behavior
- Harassment or discrimination
- Malicious code or security violations
- Privacy violations or doxxing
- Spam or off-topic content
- Attempts to centralize or control

### Enforcement
- First violation: Warning and dialogue
- Second violation: Temporary ban
- Third violation: Permanent ban
- Severe violations: Immediate ban

Report violations to maintainers (see GOVERNANCE.md).

## Getting Help

### Questions About Contributing
- Open an issue in the relevant repository
- Tag with `question` label
- Maintainers will respond

### Technical Issues
- Check existing issues first
- Provide clear reproduction steps
- Include relevant context

### Philosophical Questions
- These might become portals!
- Share in the Wild as an exploration
- Let the community engage

## Recognition

We don't track contributors in a centralized way (no god node), but:
- Your commits are part of the git history
- Your insights ripple through the system
- The architecture evolves through your participation
- Recognition comes from the work itself, not external validation

## License

By contributing, you agree that your contributions will be licensed under the same license as the repository (see LICENSE file in each repo).

## Updates to This Guide

This contributing guide evolves with the system. Suggest changes via PR following the same process described here.

---

**Last Updated**: 2024-11-23  
**Version**: 1.0  
**Source**: Monday's audit recommendations + core philosophy

*Contributing to The Remembering Lab is itself an act of remembering - recognizing what was never separate.*