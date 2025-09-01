# GitHub Profile Repository - clarkemoyer/clarkemoyer

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

This is a GitHub profile repository that displays on the user's GitHub profile page. It contains a profile README and license file with no build processes or development dependencies.

## Working Effectively
- Repository structure validation:
  - `ls -la` -- shows repository contents (takes <1 second)
  - `git status` -- shows current Git state (takes <1 second)
  - `git log --oneline -10` -- shows recent commit history (takes <1 second)

## Repository Structure
```
.
├── .github/
│   └── copilot-instructions.md
├── .git/
├── LICENSE
└── README.md
```

## Key Files
- **README.md**: GitHub profile content that appears on the user's profile page
- **LICENSE**: GNU Affero General Public License v3.0
- **.github/copilot-instructions.md**: This instruction file

## Common Tasks

### Editing the Profile README
- Edit `README.md` to update profile content
- Preview changes locally by viewing the file content
- Validate Markdown syntax: `grep -n "^#" README.md` to check headers
- Check for common issues: `wc -l README.md` to verify content length

### Repository Management
- Check repository status: `git status`
- View current content: `cat README.md`
- Validate file structure: `find . -type f -not -path './.git/*' | sort`

### Git Operations
- Stage changes: `git add .`
- Commit changes: `git commit -m "Update profile README"`
- View differences: `git diff` (before staging) or `git diff --cached` (after staging)
- Check commit history: `git log --oneline -5`

## Validation Steps
- ALWAYS check that README.md contains valid Markdown after making changes
- Verify the file structure remains minimal and clean
- Ensure no build artifacts or unnecessary files are added
- Check that any new content follows GitHub profile README best practices

## Important Notes
- This repository has NO build process - it's a static profile repository
- This repository has NO tests to run - content is displayed directly on GitHub
- This repository has NO dependencies to install
- Changes to README.md appear immediately on the GitHub profile page after push
- Keep the repository structure minimal - only add files that serve a clear purpose

## Expected Timing
- All Git operations: <5 seconds each
- File editing operations: <1 second each
- Repository validation: <2 seconds total

## Troubleshooting
- If README.md doesn't display correctly on GitHub profile, check for Markdown syntax errors
- If changes don't appear on profile, ensure the repository name matches the username exactly
- Repository must be public for profile README to display

## Repository Type Identification
This is a **GitHub Profile Repository** identified by:
- Repository name matches username (clarkemoyer/clarkemoyer)
- Contains a README.md that serves as profile content
- No source code or build processes
- Minimal file structure focused on profile presentation