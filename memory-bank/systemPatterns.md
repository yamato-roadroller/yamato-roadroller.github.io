# System Patterns

## Architecture Overview
The website follows a simple, static site architecture using GitHub Pages:
- **Single Page Design**: All content consolidated in `index.md`
- **Markdown-based**: Uses GitHub Flavored Markdown for content
- **Static Hosting**: GitHub Pages automatically builds and serves the site
- **Asset Management**: Images hosted via GitHub repository assets
- **Citation Management**: Separate BibTeX files in `/bib/` directory

## Key Technical Decisions
1. **Markdown over HTML**: Easier maintenance and GitHub Pages compatibility
2. **Single Page Layout**: Comprehensive view without navigation complexity
3. **External Asset Hosting**: GitHub repository assets for images
4. **Separate BibTeX Files**: Individual citation files for each publication

## Design Patterns in Use

### Publication Entry Pattern
```markdown
- Title: Authors, Conference/Journal, Year ([arXiv](link), <a href="bib/filename.bib">BibTeX</a>)
```
- Consistent formatting across all publications
- Direct links to arXiv and BibTeX files
- Chronological ordering (newest first)

### Section Organization Pattern
```markdown
# Major Section
### Subsection
- List items with consistent formatting
```

### Image Display Pattern
```markdown
<img height="180" alt="description" src="github-asset-url">
```
- Consistent height for profile images
- GitHub repository asset URLs
- Descriptive alt text

### Link Pattern
- External links: `[text](url)`
- BibTeX links: `<a href="bib/filename.bib">BibTeX</a>`
- Mixed format for publication entries

## Component Relationships
1. **Main Content** (`index.md`) → **BibTeX Files** (`bib/*.bib`)
2. **Profile Images** → **GitHub Repository Assets**
3. **Publication Entries** → **External Resources** (arXiv, conference sites)

## Critical Implementation Paths
1. **Adding Publications**: Create BibTeX file → Update index.md → Verify links
2. **Image Updates**: Upload to repository → Update image URLs in index.md
3. **Content Updates**: Direct markdown editing in index.md

## File Structure
```
/
├── index.md (main content)
├── README.md (repository documentation)
├── bib/ (citation files)
│   ├── okamoto2023constructing.bib
│   └── okamoto2024crepe.bib
└── memory-bank/ (project documentation)
    ├── projectbrief.md
    ├── productContext.md
    ├── systemPatterns.md
    ├── techContext.md
    ├── activeContext.md
    └── progress.md
