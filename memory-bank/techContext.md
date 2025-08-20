# Technical Context

## Technologies Used
- **GitHub Pages**: Static site hosting with automatic deployment
- **Markdown**: GitHub Flavored Markdown for content authoring
- **Git**: Version control and deployment mechanism
- **HTML**: Embedded HTML tags for advanced formatting (images, links)
- **BibTeX**: Academic citation format for publications

## Development Setup
- **Repository**: https://github.com/yamato-roadroller/yamato-roadroller.github.io.git
- **Hosting**: GitHub Pages automatic deployment from main branch
- **Domain**: yamato-roadroller.github.io
- **Content Management**: Direct file editing via GitHub or local development

## Technical Constraints
1. **GitHub Pages Limitations**:
   - Static content only (no server-side processing)
   - Jekyll processing (though not actively used)
   - File size and repository size limits

2. **Markdown Limitations**:
   - Limited styling options
   - Mixed HTML/Markdown for complex formatting
   - No dynamic content generation

3. **Asset Management**:
   - Images must be hosted externally or in repository
   - Large files should be managed carefully
   - GitHub asset URLs can be lengthy

## Dependencies
- **GitHub Pages**: Automatic Jekyll processing
- **External Services**: 
  - arXiv for paper hosting
  - GitHub repository assets for images
  - External conference/journal websites for links

## Tool Usage Patterns

### Content Updates
1. **Direct GitHub Editing**: For quick text updates
2. **Local Development**: For major changes or multiple file updates
3. **Git Workflow**: Standard commit/push for deployment

### Publication Management
1. **BibTeX Creation**: Individual files for each publication
2. **Link Verification**: Ensure arXiv and external links work
3. **Format Consistency**: Follow established publication entry pattern

### Asset Management
1. **Image Upload**: Via GitHub repository interface
2. **URL Generation**: Copy GitHub asset URLs
3. **Size Optimization**: Maintain consistent image dimensions

## Performance Considerations
- **Single Page Load**: All content loads at once
- **Image Optimization**: Consistent sizing reduces layout shift
- **External Links**: May affect load time if many external resources
- **GitHub Pages CDN**: Automatic global distribution

## Security Considerations
- **Public Repository**: All content is publicly visible
- **External Links**: Verify destination security
- **Asset URLs**: GitHub-hosted assets are secure
