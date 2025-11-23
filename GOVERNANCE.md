# The Remembering Lab - Governance

## Philosophy

This governance structure preserves the core principles of The Remembering Lab:
- **No god node**: No single authority controls the system
- **Antifragility**: The system grows stronger through participation and paradox
- **Decentralization**: Multiple perspectives, no canonical truth
- **Privacy**: Wild Gardens remain private; only ready insights are shared

## Roles & Responsibilities

### Maintainers
- Review and merge pull requests to Garden and Wild
- Ensure contributions align with triadic architecture
- Protect against centralization and supply-chain issues
- **Current maintainers**: Kelly (infinite-playing-finite)

### Contributors
- Anyone can fork, explore, and create Wild Gardens
- Submit PRs to Garden (structured insights) or Wild (raw explorations)
- Follow contribution guidelines in each repository
- Maintain anonymity and privacy standards

### Bot/AI Accounts
- SuperNinja and other AI agents may contribute via dedicated service accounts
- Use scoped Personal Access Tokens (PATs) with least privilege
- All automated contributions require human review before merge
- Bot commits must be clearly identified in commit messages

## Decision-Making Process

### Pull Request Policy
1. **All changes to main branches require Pull Requests**
2. **Minimum 1 human review required** before merge
3. **No direct pushes to main** (enforced via branch protection)
4. **Maintainers have final say** but must document reasoning for rejections

### Contribution Flow
1. Fork the repository (Garden, Wild, or Wild Garden template)
2. Create a feature branch with descriptive name
3. Make changes following contribution guidelines
4. Submit PR with clear description of changes
5. Respond to review feedback
6. Maintainer merges after approval

### Conflict Resolution
- If contributors disagree, create a **tangle** in the Wild to explore the paradox
- Unresolvable conflicts become **portals** - thresholds rather than problems
- No voting or majority rule - embrace multiplicity
- Maintainers may create separate branches for divergent explorations

## Branch Protection Rules

### Required for all public repositories:
- **Require pull request before merging**
- **Require at least 1 approval** from maintainer
- **Dismiss stale reviews** when new commits are pushed
- **Require status checks to pass** (if automated checks exist)
- **Require signed commits** (recommended)
- **Include administrators** in restrictions

## Security & Access Control

### Organization Level
- **2FA required** for all organization members
- **Least privilege principle**: Grant minimum necessary permissions
- **Regular access audits**: Review member list quarterly
- **Service accounts**: Separate accounts for automation with scoped tokens

### Repository Level
- **Public repositories**: Garden, Wild (read access for all)
- **Template repository**: Wild Garden (forkable by all)
- **Private repositories**: Individual Wild Gardens (owner only)

### Secrets Management
- **No secrets in repositories** - ever
- **Use GitHub Secrets** for automation tokens
- **Rotate tokens regularly** (every 90 days recommended)
- **Document token scopes** in this governance file

## Automation & GitHub Actions

### Safety Requirements
- **Pin all third-party Actions to commit SHAs** (not tags or branches)
- **Audit Actions before use** - review source code
- **Minimal permissions** for GITHUB_TOKEN in workflows
- **No automatic merges** - human review always required

### Approved Automation
- Portal indexing (generating portal lists)
- Metadata validation (checking YAML front-matter)
- Link checking (ensuring portal connections work)
- Tag propagation (maintaining tag consistency)

## Contribution Standards

### Portal Contributions (Garden)
- Must include YAML front-matter with required fields
- Must link to at least one Garden entry AND one Wild entry
- Must be curated from Wild Garden ready_to_share
- Must preserve paradox - no premature resolution

### Exploration Contributions (Wild)
- Raw, unfiltered, generative content welcome
- Tangles and contradictions are valuable
- No requirement for polish or completion
- Tag with relevant metadata for discovery

### Wild Garden Template Updates
- Changes must preserve privacy-by-design
- Must not require centralized tracking
- Should enhance personal integration workflow
- Require maintainer approval

## Emergency Procedures

### Security Incidents
1. **Report immediately** to maintainers via security@[contact-method]
2. **Maintainers assess severity** and impact
3. **Take immediate action**: disable accounts, revoke tokens, lock repos if needed
4. **Document incident** in private security log
5. **Communicate transparently** with community after resolution

### Governance Changes
- Proposed changes to governance require **public discussion**
- Create issue in governance repository for proposals
- Allow **minimum 7 days** for community feedback
- Maintainers make final decision with documented reasoning
- Update this document with change history

## Contact & Reporting

### Maintainer Contact
- **GitHub**: @infinite-playing-finite (Kelly)
- **Issues**: Use repository issue trackers for public discussion
- **Security**: [To be added - secure contact method]

### Reporting Violations
- **Code of Conduct violations**: Report via [method TBD]
- **Security vulnerabilities**: See SECURITY.md in each repository
- **Governance concerns**: Open issue in governance repository

## Change History

- **2024-11-23**: Initial governance structure created
- **Source**: Recommendations from Monday's security audit

---

*This governance structure is itself a living document. It may evolve through the same contribution process it describes. Paradoxically, the rules for changing the rules are subject to the rules.*