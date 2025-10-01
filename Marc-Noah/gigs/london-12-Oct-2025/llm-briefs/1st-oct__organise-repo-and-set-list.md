# Claude Code Brief: GitHub Repository Organization for Marc Noah Concert

## Project Context
Organize the GitHub repository at `https://github.com/DinisCruz/Cruz-and-Cruz__Music` to manage all materials for the "Marc Noah and the Cruzes" concert at The Roebuck on October 12, 2025.

Current location of concert files: `/Marc-Noah/gigs/london-12-Oct-2025/`

## Objective
Create a comprehensive folder structure and tracking system to manage all concert materials, enable collaboration, track progress, and prepare content for eventual static website generation.

## Required Folder Structure

### 1. Songs Organization (`/Marc-Noah/gigs/london-12-Oct-2025/songs/`)

Create individual folders for each of the 11 songs in the setlist:
```
songs/
├── 01-road-trip-v1/
├── 02-fast-car-v1/
├── 03-cover-1-TBD/
├── 04-cover-medley-1/
├── 05-more-than-words/
├── 06-marc-original-1-TBD/
├── 07-fast-car-v2/
├── 08-cover-2-TBD/
├── 09-road-trip-v2/
├── 10-cover-medley-2/
└── 11-happy-birthday/
```

### 2. Per-Song Materials Structure

Each song folder should contain:
```
[song-name]/
├── README.md           # Overview and checklist for this song
├── lyrics.md          # Song lyrics
├── chords.md          # Chord progressions and tabs
├── arrangement.md     # Who plays what, specific arrangement notes
├── score/             # Folder for PDFs, music notation files
│   └── README.md      # Links to external scores if needed
├── recordings/        # Audio/video references
│   └── README.md      # Links to YouTube, Google Drive, Spotify
├── transitions.md     # How to enter/exit this song in the set
├── notes.md          # Rationale: Why this song? Meaning, story, performance notes
└── combined-info.md   # OPTIONAL: For simpler songs, combine multiple elements
```

Note: For simpler songs or covers, multiple elements can be combined into fewer files (e.g., `combined-info.md` could contain lyrics, chords, and notes together).

### 3. Master Tracking File

Create `/Marc-Noah/gigs/london-12-Oct-2025/SONG_STATUS.md` with:

```markdown
# Song Status Tracker

| # | Song | Finalized | Lyrics | Chords | Score | Arrangement | Recording | Notes |
|---|------|-----------|--------|--------|-------|-------------|-----------|-------|
| 1 | Road Trip V1 | 🟡 | ✅ | ✅ | 🔴 | 🟡 | ✅ | Ready |
| 2 | Fast Car V1 | 🟡 | ✅ | ✅ | 🟡 | 🔴 | ✅ | Need arrangement |
| 3 | Cover #1 | 🔴 | - | - | - | - | - | **NEEDS SELECTION** |
| ... | ... | ... | ... | ... | ... | ... | ... | ... |

Legend: ✅ Complete | 🟡 In Progress | 🔴 Not Started | - Not Applicable
```

### 4. Media & Design Assets (`/Marc-Noah/gigs/london-12-Oct-2025/media/`)

```
media/
├── README.md              # Overview of all media assets
├── design/
│   ├── logos/
│   ├── posters/
│   └── brand-guidelines.md
├── social-media/
│   ├── instagram/
│   │   ├── templates/
│   │   └── scheduled-posts.md
│   ├── linkedin/
│   └── twitter-bluesky/
└── press/
    ├── press-release.md
    ├── artist-bio.md
    └── fact-sheet.md
```

### 5. Media Briefings (For Press/Industry) (`/Marc-Noah/gigs/london-12-Oct-2025/media-briefings/`)

```
media-briefings/
├── README.md                    # Overview for media professionals
├── press-kit/
│   ├── one-page-summary.md     # Quick facts about the concert
│   ├── full-press-release.md   # Detailed press release
│   ├── artist-bios.md          # Bios for Marc, Emily, Dinis
│   └── high-res-images.md      # Links to press photos
├── about-the-project/
│   ├── music-lab-concept.md    # Explaining the open-source music concept
│   ├── why-this-matters.md     # The innovation and significance
│   ├── previous-work.md        # Marc Noah's history and releases
│   └── future-plans.md         # What happens after Oct 12
├── story-angles/
│   ├── tech-meets-music.md     # The open-source angle
│   ├── local-to-global.md      # Algarve musician goes international
│   ├── zero-budget-music.md    # DIY/community-driven approach
│   └── experimental-live.md    # The two-versions concept
├── interview-materials/
│   ├── key-quotes.md           # Quotable statements
│   ├── faq.md                  # Common questions answered
│   ├── talking-points.md       # Key messages
│   └── contact-info.md         # How to reach the team
└── coverage-tracker.md         # Track media mentions and coverage
```

### 6. Project Management Section

Create `/Marc-Noah/gigs/london-12-Oct-2025/project/`:

```
project/
├── README.md              # Project overview
├── HOW_TO_HELP.md        # For volunteers/contributors
├── TASKS.md              # Task assignments and deadlines
├── TIMELINE.md           # Critical dates and deadlines
├── WORKFLOW.md           # Git workflow and contribution process
├── contacts.md           # Team contacts
└── technical-requirements.md
```

### 7. Marc Noah Resources (`/Marc-Noah/resources/`)

```
resources/
├── README.md             # Overview of Marc's existing materials
├── official-links.md     # Links to marcnoah.pt, Spotify, YouTube, Apple Music
├── existing-songs.md     # Catalog of released songs with streaming links
├── performance-history.md # Past performances, videos from Algarve venues
└── bio-and-press.md      # Official biography and press materials
```

### 8. External Links Management

Create `/Marc-Noah/gigs/london-12-Oct-2025/EXTERNAL_LINKS.md`:

```markdown
# External Resources

## Marc Noah Official Channels
- Website: https://www.marcnoah.pt/
- Spotify: [Link]
- YouTube: [Link]
- Apple Music: [Link]
- Instagram: [Link]

## Project Resources
- Google Drive (Large Files): [Link]
- YouTube Unlisted Videos: [Link]
- Discord Channel: [Link]

## Collaboration Tools
- GitHub Repo: https://github.com/DinisCruz/Cruz-and-Cruz__Music
- Project Board: [Link]
```

## README Templates to Create

### Main Concert README (`/Marc-Noah/gigs/london-12-Oct-2025/README.md`)

```markdown
# Marc Noah and the Cruzes - Live at The Roebuck

**Date:** October 12, 2025  
**Venue:** The Roebuck, London  
**Status:** [Current preparation status]

## Quick Links
- [Song Status Tracker](./SONG_STATUS.md)
- [How to Help](./project/HOW_TO_HELP.md)
- [Design Brief](./1st-oct__design-brief.md)
- [Production Brief](./1st-oct__concert-production-brief.md)
- [Setlist](./1st-oct__set-list__version_1.md)

## Project Structure
- `/songs/` - Individual song materials
- `/media/` - Design assets and promotional materials
- `/media-briefings/` - Press kit and information for journalists/industry
- `/project/` - Project management documents

## Next Actions
[List current priorities]

## Team
- Marc Noah - Lead Musician
- Emily - Keyboards/Vocals
- Dinis Cruz - Cajon/Guitar/Producer
```

### Per-Song README Template

```markdown
# [Song Name] - Song #[X]

## Status
- [ ] Song selected/confirmed
- [ ] Lyrics documented
- [ ] Chords finalized
- [ ] Arrangement decided
- [ ] Score obtained/created
- [ ] Reference recording available
- [ ] Transitions planned

## Quick Info
- **Key:** [Key]
- **Duration:** [Duration]
- **Version Notes:** [What makes this version unique]

## Performance Notes
[Key performance considerations]

## Files
- [Lyrics](./lyrics.md)
- [Chords](./chords.md)
- [Arrangement](./arrangement.md)
- [Transitions](./transitions.md)
```

### HOW_TO_HELP.md Template

```markdown
# How to Help

## Immediate Needs
- [ ] Song selection for Cover #1 and Cover #2
- [ ] Medley song choices
- [ ] Chord transcriptions
- [ ] Video recording volunteers
- [ ] Social media content creation

## Skills Needed
- Musicians for arrangement suggestions
- Video editors
- Graphic designers
- Social media managers
- Sound engineers

## How to Contribute
1. Check the [Task List](./TASKS.md)
2. Assign yourself to a task
3. Create a pull request with your contribution
4. Tag @DinisCruz for review

## Contact
[Contact information]
```

### WORKFLOW.md Template

```markdown
# Git Workflow & Contribution Process

## For Contributors
1. Fork or clone the repository
2. Create a feature branch: `git checkout -b feature/song-name-update`
3. Make your changes
4. Commit with clear messages: `git commit -m "Add chords for Fast Car V1"`
5. Push to branch: `git push origin feature/song-name-update`
6. Create Pull Request with description of changes
7. Tag @DinisCruz for review

## File Naming Conventions
- Use kebab-case: `song-name.md` not `SongName.md`
- Date format: `YYYY-MM-DD` (e.g., `2025-10-12`)
- Version format: `v1`, `v2` not `version-1`

## Large Files
- Audio/Video: Upload to Google Drive, link in README
- PDFs under 25MB: Can be committed directly
- Images: Optimize before committing

## Review Process
- Dinis reviews all PRs
- Quick fixes can be merged immediately
- Major changes need team discussion
```

## Implementation Steps for Claude Code

1. **Create the folder structure** as outlined above
2. **Generate README files** for each directory with appropriate templates
3. **Create tracking files** (SONG_STATUS.md, TASKS.md, TIMELINE.md, etc.)
4. **Set up placeholder files** for each song's materials
5. **Add `.gitkeep` files** to empty directories to maintain structure
6. **Create index/navigation system** through README files
7. **Set up templates** for recurring document types
8. **Initialize TIMELINE.md** with critical dates (Oct 7-8 remote rehearsal, Oct 10 Marc arrives, Oct 11 rehearsal, Oct 12 show)

## Critical Timeline Context

**URGENT: Only 11 days until the concert (as of Oct 1, 2025)**

Key Deadlines:
- **ASAP:** Song selections for TBD slots (Cover #1, Cover #2, Medleys)
- **Oct 5:** All arrangements finalized
- **Oct 7-8:** Remote rehearsal with full team
- **Oct 9:** Volunteer briefing call
- **Oct 10:** Marc arrives in London
- **Oct 11:** In-person rehearsal
- **Oct 12:** Show day

## Additional Notes

- All files should be in Markdown for easy version control and future static site generation
- Use relative links between documents for portability
- Include metadata in frontmatter for future Hugo/MkDocs processing
- Keep large media files in Google Drive/YouTube and link to them
- Use checklists liberally for tracking progress
- Maintain consistent naming conventions (kebab-case for files/folders)

## External Resources to Link

- Marc Noah's official website: https://www.marcnoah.pt/
- Marc Noah's Spotify: [To be added]
- Marc Noah's YouTube: [To be added]
- Project Google Drive: [To be added]
- Discord/Communication channel: [To be added]

## Success Criteria

- Every team member can find any needed document within 3 clicks
- Clear status visibility for all songs and tasks
- Easy onboarding for new volunteers
- Ready for static site generation
- All materials tracked and version controlled