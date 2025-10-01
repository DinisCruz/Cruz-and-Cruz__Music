# Git Workflow & Contribution Process

## For Contributors

### Getting Started

1. **Fork or Clone the Repository**
   ```bash
   git clone https://github.com/DinisCruz/Cruz-and-Cruz__Music.git
   cd Cruz-and-Cruz__Music
   ```

2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/song-name-update
   ```

   Branch naming conventions:
   - `feature/song-chords-fast-car` - Adding song materials
   - `docs/update-press-release` - Documentation updates
   - `fix/typo-in-readme` - Bug fixes
   - `media/add-poster-design` - Media assets

3. **Make Your Changes**
   - Edit or create files as needed
   - Follow file naming conventions (see below)
   - Test that markdown renders correctly
   - Keep changes focused and atomic

4. **Commit Your Work**
   ```bash
   git add .
   git commit -m "Add chord chart for Fast Car V1"
   ```

   Commit message guidelines:
   - Use present tense: "Add" not "Added"
   - Be specific: "Add chord chart for Fast Car V1" not "Update files"
   - Reference issues: "Add chords for #12"

5. **Push to Your Branch**
   ```bash
   git push origin feature/song-name-update
   ```

6. **Create Pull Request**
   - Go to GitHub and create a Pull Request
   - Include clear description of changes
   - Reference related Issues
   - Tag @DinisCruz for review

7. **Respond to Feedback**
   - Make requested changes
   - Push updates to same branch
   - PR will update automatically

## File Naming Conventions

### General Rules
- Use **kebab-case**: `song-name.md` NOT `SongName.md` or `song_name.md`
- Be descriptive: `fast-car-chords-v1.md` NOT `fc1.md`
- Use lowercase for all filenames and directories

### Dates
- Format: `YYYY-MM-DD`
- Example: `2025-10-12-show-notes.md`

### Versions
- Format: `v1`, `v2`, NOT `version-1` or `ver1`
- Example: `road-trip-v1`, `road-trip-v2`

### Song Materials
- Lyrics: `lyrics.md`
- Chords: `chords.md`
- Arrangement: `arrangement.md`
- Transitions: `transitions.md`
- Notes: `notes.md`

### Examples
✅ Good:
- `songs/01-road-trip-v1/chords.md`
- `media/design/poster-oct-2025.png`
- `project/timeline.md`

❌ Bad:
- `songs/01_Road_Trip_V1/Chords.MD`
- `media/design/Poster Oct 2025.png`
- `project/TIMELINE.MD`

## File Organization

### Markdown Files
- All text content in Markdown (`.md`)
- Use proper heading hierarchy (# → ## → ###)
- Include frontmatter if applicable
- Use relative links between documents

### Large Files
- **Audio/Video:** Upload to Google Drive, add link in README
- **PDFs under 25MB:** Can be committed directly to `/score/` folders
- **Images:** Optimize before committing (aim for <1MB)
- **High-res photos:** Google Drive + link

### Directory Structure
```
songs/
  01-song-name/
    README.md          # Always include
    lyrics.md
    chords.md
    arrangement.md
    score/             # PDF files OK here
    recordings/        # Links only, not files
```

## Working with Markdown

### Headers
```markdown
# Main Title (H1) - Use once per file
## Section (H2)
### Subsection (H3)
```

### Lists
```markdown
- Unordered list
- Item 2

1. Ordered list
2. Item 2
```

### Task Lists
```markdown
- [ ] Incomplete task
- [x] Completed task
```

### Links
```markdown
[Link Text](./relative/path/to/file.md)
[External Link](https://example.com)
```

### Code Blocks
````markdown
```bash
git commit -m "message"
```
````

## Review Process

### For Contributors
1. All PRs reviewed by @DinisCruz or designated reviewers
2. Address feedback promptly
3. Small changes can be merged quickly
4. Major changes may need team discussion

### For Reviewers
- Check file naming conventions
- Verify markdown formatting
- Ensure content accuracy
- Test links work
- Confirm no large binary files

## Collaboration Etiquette

### Do's
✅ Communicate clearly in PRs
✅ Ask questions if unsure
✅ Keep changes focused
✅ Credit others' work
✅ Be responsive to feedback
✅ Update your PRs based on review

### Don'ts
❌ Commit large binary files without discussion
❌ Make unrelated changes in one PR
❌ Ignore review feedback
❌ Force push to shared branches
❌ Commit secrets or private information

## Git Commands Reference

### Daily Workflow
```bash
# Update your local repo
git pull origin main

# Create new branch
git checkout -b feature/my-feature

# Stage changes
git add .

# Commit
git commit -m "Description"

# Push
git push origin feature/my-feature

# Update branch with latest main
git checkout main
git pull
git checkout feature/my-feature
git merge main
```

### Fixing Mistakes
```bash
# Undo last commit (keep changes)
git reset --soft HEAD~1

# Discard local changes
git checkout -- filename.md

# Update last commit message
git commit --amend -m "New message"
```

## Getting Help

- **General Questions:** Open a GitHub Discussion
- **Technical Issues:** Create a GitHub Issue
- **Urgent Matters:** Contact team directly (see [contacts.md](./contacts.md))
- **Workflow Questions:** Ask in PR comments

## Branch Protection

### Main Branch
- Protected from direct pushes
- Requires PR for all changes
- Reviewed before merge

### Feature Branches
- Can be pushed freely
- Deleted after merge
- Name according to conventions

---

**Remember:** When in doubt, ask! We're here to help and learn together.

**Last Updated:** October 1, 2025
