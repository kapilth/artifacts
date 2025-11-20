# Artifacts Repository

This repository is used for storing and managing artifacts like images and icons that need to be used and referenced on websites.

## Purpose

This repository serves as a centralized storage location for static assets that can be referenced across multiple websites and projects. By hosting these artifacts in a dedicated repository, we can:

- Version control all visual assets
- Provide stable, permanent URLs for images and icons
- Maintain a single source of truth for branding materials
- Enable easy sharing across different projects and websites

## Directory Structure

```
artifacts/
├── images/
│   ├── logos/          # Company and project logos
│   ├── banners/        # Banner images for websites and promotions
│   └── screenshots/    # Application screenshots and demos
└── icons/
    ├── social/         # Social media icons (Twitter, LinkedIn, etc.)
    └── ui/             # User interface icons
```

## How to Add Artifacts

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kapilth/artifacts.git
   cd artifacts
   ```

2. **Add your artifact to the appropriate directory:**
   - Place logos in `images/logos/`
   - Place banners in `images/banners/`
   - Place screenshots in `images/screenshots/`
   - Place social media icons in `icons/social/`
   - Place UI icons in `icons/ui/`

3. **Commit and push your changes:**
   ```bash
   git add .
   git commit -m "Add [description of artifact]"
   git push origin main
   ```

## How to Reference Artifacts

Once artifacts are pushed to the repository, they can be referenced using GitHub's raw content URLs:

### Format:
```
https://raw.githubusercontent.com/kapilth/artifacts/main/[path-to-file]
```

### Examples:
```
https://raw.githubusercontent.com/kapilth/artifacts/main/images/logos/company-logo.png
https://raw.githubusercontent.com/kapilth/artifacts/main/icons/social/twitter-icon.svg
```

### Usage in HTML:
```html
<img src="https://raw.githubusercontent.com/kapilth/artifacts/main/images/logos/company-logo.png" alt="Company Logo">
```

### Usage in Markdown:
```markdown
![Company Logo](https://raw.githubusercontent.com/kapilth/artifacts/main/images/logos/company-logo.png)
```

## Best Practices

1. **File Naming:**
   - Use lowercase letters
   - Use hyphens (-) instead of spaces
   - Use descriptive names (e.g., `company-logo-dark.png` instead of `logo1.png`)

2. **File Formats:**
   - Use SVG for icons and logos when possible (scalable and small file size)
   - Use PNG for images requiring transparency
   - Use JPG for photographs and complex images
   - Optimize images before uploading to reduce file size

3. **Organization:**
   - Keep files organized in the appropriate directories
   - Avoid creating new top-level directories without discussion
   - Delete outdated artifacts to keep the repository clean

## Contributing

When adding artifacts:
- Ensure you have the right to use and distribute the artifact
- Verify the artifact is optimized for web use
- Use meaningful commit messages describing what artifact was added
- Consider whether the artifact might be useful in multiple contexts

## License

Please ensure that all artifacts added to this repository comply with applicable licenses and usage rights.