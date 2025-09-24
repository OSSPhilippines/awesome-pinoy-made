# Contributing Guides

## Rules

There are no complicated rules, just follow the following:

1. Always add your new entries at the end of the list.
2. Every entry should have a working anchor link in the "Table of Contents" section.
3. Make sure to supply a proper description of your project. 1 sentence minimum.
4. Links to the website or repository are required.
5. **IMPORTANT**: You must also add your project to the `data.json` file at the end of the projects array. See the [Data Format](#data-format) section below.
6. You can make a PR for awesome projects that you know even if you're not the author given that the following are met:

   a. The project is public.

   b. The project is not yet on the list.

## Acceptance Criteria

1. Your project MUST be open-source.
2. Your project MUST have `LICENSE`, `CODE_OF_CONDUCT.md`, and `CONTRIBUTING.md`.
3. Your project doesn't have to be original, but it MUST NOT be plagiarized.
4. Your project MUST NOT be a fork of an existing active project.
5. The core maintainer/s is/are Filipino.
6. To maintain high-quality projects in the list, ~~your project must have at least 20 stars.~~ We will review the projects thoroughly. 

## Data Format

When adding your project to `data.json`, please add it at the end of the `projects` array with the following structure:

```json
{
  "id": "your-project-id",
  "name": "Your Project Name",
  "slug": "your-project-slug",
  "description": "A brief description of what your project does",
  "iconUrl": null,
  "bannerUrl": null,
  "category": "library|tool|framework|template|plugin|application|sdk|cms|database|visualization|resource",
  "tags": ["relevant", "tags", "for", "filtering"],
  "technologies": ["Technology Stack", "Used"],
  "author": {
    "name": "yourgithubusername",
    "github": "https://github.com/yourgithubusername",
    "twitter": "@yourtwitterhandle"
  },
  "links": {
    "website": "https://your-project-website.com",
    "github": "https://github.com/yourusername/yourproject",
    "npm": null,
    "documentation": null
  },
  "organization": null,
  "addedDate": null,
  "stars": null
}
```

### Field Guidelines:
- **id**: Use kebab-case (lowercase with hyphens)
- **slug**: URL-friendly version, usually same as id
- **iconUrl**: URL to project logo/icon (square image, recommended: 256x256 or 512x512)
- **bannerUrl**: URL to project banner/screenshot (recommended: 1200x630 for social media)
- **category**: Choose the most appropriate category from the list
- **tags**: Include relevant technologies, domains, and platforms
- **technologies**: List the main technologies/frameworks used
- **author**: Use GitHub username (without @ symbol) for name field
- **links**: Set to `null` if not applicable
- **organization**: Set if maintained by a company/organization

### Image URL Guidelines:
- Both **iconUrl** and **bannerUrl** should use HTTPS URLs
- Images must be publicly accessible
- Can be hosted on GitHub, project website, or CDN
- Set to `null` if no image is available
