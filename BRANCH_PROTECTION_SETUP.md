# Branch Protection Setup Guide

This guide will walk you through setting up branch protection rules for The Remembering Lab repositories. This is a critical security measure recommended by Monday's audit.

## Why Branch Protection?

Branch protection ensures:
- **No accidental overwrites** - Changes require review
- **Human oversight** - Even AI contributions need approval
- **Audit trail** - All changes are documented
- **Quality control** - Maintainers can review before merge
- **Security** - Prevents malicious or accidental damage

## What You Need to Do

You'll need to set up branch protection for all three repositories:
1. `the-garden`
2. `the-wild`
3. `the-wild-garden`

## Step-by-Step Instructions

### For Each Repository:

#### Step 1: Navigate to Repository Settings

1. Go to https://github.com/the-remembering-lab/[REPO-NAME]
2. Click **Settings** (top right, near the repository name)
3. In the left sidebar, click **Branches** (under "Code and automation")

#### Step 2: Add Branch Protection Rule

1. Click **Add branch protection rule** (or **Add rule**)
2. In "Branch name pattern" field, enter: `main`

#### Step 3: Configure Protection Settings

Check these boxes:

**Require a pull request before merging**
- ✅ Check this box
- Then check: **Require approvals**
  - Set "Required number of approvals before merging" to: **1**
- ✅ Check: **Dismiss stale pull request approvals when new commits are pushed**

**Require status checks to pass before merging** (optional for now)
- Leave unchecked unless you add automated tests later

**Require conversation resolution before merging** (optional but recommended)
- ✅ Check this box
- Ensures all review comments are addressed

**Require signed commits** (optional but recommended)
- ✅ Check this box if you want extra security
- Note: Contributors will need to set up GPG signing

**Require linear history** (optional)
- Leave unchecked for now (allows merge commits)

**Include administrators**
- ✅ **IMPORTANT: Check this box**
- This ensures even you (as admin) must follow the rules
- Prevents accidental direct pushes

**Allow force pushes**
- ❌ Leave unchecked (prevents rewriting history)

**Allow deletions**
- ❌ Leave unchecked (prevents accidental branch deletion)

#### Step 4: Save Changes

1. Scroll to bottom
2. Click **Create** (or **Save changes**)
3. You should see a green success message

#### Step 5: Repeat for Other Repositories

Repeat Steps 1-4 for:
- `the-garden`
- `the-wild`
- `the-wild-garden`

## Verification

After setting up, verify it worked:

1. Try to push directly to main (it should fail):
   ```bash
   cd /path/to/repo
   echo "test" >> README.md
   git add README.md
   git commit -m "Test direct push"
   git push origin main
   ```

2. You should see an error like:
   ```
   remote: error: GH006: Protected branch update failed
   ```

3. This is GOOD! It means protection is working.

## What This Means for Workflow

### For You (Kelly)
- You can no longer push directly to main
- You must create a branch and PR (even for your own changes)
- You must approve PRs before merging (even your own)
- This is intentional - prevents accidents!

### For SuperNinja (and other AI agents)
- Can push to branches (not main)
- Cannot merge without your approval
- You review all AI contributions before they go live
- This preserves human oversight

### For Future Contributors
- Must fork and create PRs
- Must wait for your approval
- Cannot bypass the review process
- Ensures quality and security

## Example Workflow After Protection

```bash
# Create a new branch
git checkout -b add-new-portal

# Make changes
# ... edit files ...

# Commit changes
git commit -m "Add new portal: consciousness-in-ai"

# Push branch (this works)
git push origin add-new-portal

# Go to GitHub and create Pull Request
# You (or another maintainer) review and approve
# Then merge via GitHub UI
```

## Troubleshooting

### "I can't push to main anymore"
- This is correct! Create a branch instead.
- See example workflow above.

### "I need to make a quick fix"
- Still need to use a branch and PR
- You can approve your own PR immediately
- This creates an audit trail

### "SuperNinja's pushes are failing"
- SuperNinja should push to branches, not main
- I'll create PRs that you can review
- This is the intended workflow

### "I want to disable this temporarily"
- Not recommended! This defeats the purpose
- If absolutely necessary:
  - Go to Settings → Branches
  - Click Edit on the rule
  - Uncheck "Include administrators"
  - Make your change
  - Re-enable immediately

## Additional Security: 2FA Requirement

While you're in GitHub settings, also enable 2FA requirement:

1. Go to https://github.com/organizations/the-remembering-lab/settings/security
2. Under "Two-factor authentication", click **Require two-factor authentication**
3. This ensures all organization members use 2FA
4. Critical for security!

## Questions?

If you run into issues:
1. Check GitHub's documentation: https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches
2. Open an issue in the appropriate repository
3. The protection rules can be adjusted if needed

## Summary Checklist

For each repository (the-garden, the-wild, the-wild-garden):

- [ ] Navigate to Settings → Branches
- [ ] Add branch protection rule for `main`
- [ ] Require pull request before merging
- [ ] Require 1 approval
- [ ] Dismiss stale approvals
- [ ] Include administrators
- [ ] Disable force pushes
- [ ] Disable deletions
- [ ] Save changes
- [ ] Verify protection is working

Organization-level:
- [ ] Enable 2FA requirement for organization

---

**Once you've completed this setup, let me know and I'll update the workflow to use branches and PRs!**

This is a critical security measure that protects the integrity of The Remembering Lab. Thank you for taking the time to set this up properly! 🔒