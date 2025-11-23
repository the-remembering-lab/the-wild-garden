# Security Policy

## Philosophy

The Remembering Lab is designed with security and privacy as foundational principles:
- **No secrets in repositories** - ever
- **Privacy by design** - Wild Gardens remain private
- **Transparency** - security practices are documented and auditable
- **Least privilege** - minimal permissions for all accounts and automation

## Supported Versions

All repositories in The Remembering Lab organization follow the same security practices. We maintain security for:

| Repository | Status |
| --- | --- |
| the-garden | ✅ Actively maintained |
| the-wild | ✅ Actively maintained |
| the-wild-garden (template) | ✅ Actively maintained |

## Reporting a Vulnerability

### What to Report

Please report any security concerns including:
- Exposed credentials or tokens
- Unauthorized access or permissions issues
- Malicious code in contributions
- Supply chain vulnerabilities in dependencies or Actions
- Privacy leaks from Wild Gardens
- Automation or bot account compromises

### How to Report

**DO NOT** open public issues for security vulnerabilities.

Instead:
1. **Email**: [To be added - secure contact method]
2. **Subject line**: "SECURITY: [brief description]"
3. **Include**:
   - Description of the vulnerability
   - Steps to reproduce (if applicable)
   - Potential impact
   - Suggested fix (if you have one)

### What to Expect

- **Acknowledgment**: Within 48 hours
- **Assessment**: Within 7 days we'll assess severity and impact
- **Updates**: Regular communication about progress
- **Resolution**: Timeline depends on severity
  - Critical: 24-48 hours
  - High: 7 days
  - Medium: 30 days
  - Low: 90 days
- **Disclosure**: After fix is deployed, we'll coordinate public disclosure with you

## Security Practices

### Repository Security

#### No Secrets Policy
- **Never commit**: API keys, tokens, passwords, private keys
- **Use GitHub Secrets**: For automation that requires credentials
- **Rotate regularly**: All tokens and credentials every 90 days
- **Scope minimally**: Tokens have only necessary permissions

#### Branch Protection
- **Main branches protected**: Require PR and review before merge
- **No direct pushes**: Even administrators must use PRs
- **Signed commits**: Recommended for all contributors
- **Status checks**: Automated validation before merge

### Automation Security

#### GitHub Actions
- **Pin to commit SHAs**: Never use `@latest` or branch names
  ```yaml
  # ✅ Good
  uses: actions/checkout@a81bbbf8298c0fa03ea29cdc473d45769f953675
  
  # ❌ Bad
  uses: actions/checkout@v3
  ```
- **Audit before use**: Review source code of third-party Actions
- **Minimal permissions**: GITHUB_TOKEN has least privilege needed
- **No automatic merges**: Human review always required

#### Bot/AI Accounts
- **Dedicated service accounts**: Separate from human accounts
- **Scoped PATs**: Personal Access Tokens with minimal permissions
- **Clear identification**: Bot commits clearly marked
- **Regular audits**: Review bot activity monthly
- **Token rotation**: Every 90 days minimum

### Dependency Security

#### Current Dependencies
This project has minimal dependencies by design:
- No npm packages
- No Python packages
- No external libraries
- Pure markdown and YAML content

#### If Dependencies Added
- **Audit before adding**: Review security history
- **Pin versions**: Use exact versions, not ranges
- **Regular updates**: Check for security patches monthly
- **Automated scanning**: Use Dependabot or similar

### Privacy & Data Protection

#### Wild Garden Privacy
- **Private by default**: Wild Gardens are private repositories
- **No tracking**: No centralized user database or activity logs
- **Anonymization**: ready_to_share content must be anonymized
- **No identifiers**: Personal information removed before contribution

#### Contribution Privacy
- **Optional anonymity**: Contributors may use pseudonyms
- **Email privacy**: Use GitHub's noreply email if desired
- **Metadata minimal**: Only necessary metadata collected
- **Right to deletion**: Contributors can request content removal

## Security Checklist for Contributors

Before submitting a PR, verify:

- [ ] No secrets, tokens, or credentials in code
- [ ] No personal identifying information (unless intentional)
- [ ] No malicious code or suspicious links
- [ ] Dependencies (if any) are pinned and audited
- [ ] Commit messages are clear and descriptive
- [ ] Changes align with security practices above

## Security Checklist for Maintainers

Before merging a PR, verify:

- [ ] Code review completed by human maintainer
- [ ] No secrets or credentials exposed
- [ ] Automated checks passed (if configured)
- [ ] Contributor followed security guidelines
- [ ] Changes don't introduce new vulnerabilities
- [ ] Bot/AI contributions clearly identified

## Incident Response Plan

### Detection
- Regular security audits (quarterly)
- Automated scanning (if configured)
- Community reports via security email
- GitHub security alerts

### Response Steps
1. **Assess**: Determine severity and scope
2. **Contain**: Disable compromised accounts, revoke tokens, lock repos if needed
3. **Investigate**: Determine root cause and impact
4. **Remediate**: Fix vulnerability and deploy patches
5. **Document**: Record incident details in private log
6. **Communicate**: Inform affected parties and community
7. **Learn**: Update practices to prevent recurrence

### Severity Levels
- **Critical**: Immediate action required (exposed credentials, active exploit)
- **High**: Urgent action needed (potential data breach, privilege escalation)
- **Medium**: Important but not urgent (minor vulnerabilities, outdated practices)
- **Low**: Informational (suggestions, best practices)

## Compliance & Standards

### GitHub Security Features
- ✅ **2FA required** for organization members
- ✅ **Branch protection** enabled on main branches
- ✅ **Signed commits** recommended
- ✅ **Security advisories** enabled
- ⏳ **Dependabot alerts** (when dependencies added)
- ⏳ **Code scanning** (when applicable)

### Best Practices Followed
- OWASP secure coding guidelines
- Principle of least privilege
- Defense in depth
- Secure by default
- Privacy by design

## Security Contacts

### Maintainers
- **Kelly** (@infinite-playing-finite)

### Reporting
- **Security issues**: [To be added - secure contact method]
- **General questions**: Open issue in appropriate repository
- **Governance concerns**: See GOVERNANCE.md

## Updates to This Policy

This security policy may be updated as:
- New threats emerge
- Best practices evolve
- The system grows and changes
- Community feedback suggests improvements

All changes follow the governance process documented in GOVERNANCE.md.

---

**Last Updated**: 2024-11-23  
**Version**: 1.0  
**Source**: Monday's security audit recommendations

*Security is not a state but a practice. This policy is a living document that evolves with the system it protects.*