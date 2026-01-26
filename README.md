# Hawaiian Drosophila Genomes Project

Static website for the Hawaiian Drosophila Genomes Project built with Jekyll.

## About

The Hawaiian Drosophila Genomes Project is dedicated to advancing our understanding of Hawaiian fruit fly evolution through comprehensive genomic research. This website provides information about the project, research team, and data resources.

## Features

- **Project Information**: Overview of research goals and impact
- **Team Section**: Personnel profiles with headshots
- **Data Resources**: Links to genome assemblies, sequence data, and analysis tools (coming soon)
- **Responsive Design**: Mobile-friendly layout

## Local Development

### Prerequisites

- Ruby 3.x
- Bundler

### Setup

1. Install dependencies:
```bash
bundle install
```

2. Run the Jekyll server:
```bash
bundle exec jekyll serve
```

3. Open your browser to `http://localhost:4000/Hawaiian-Drosophila-Genomes-Project/`

## Deployment

This site is designed to work with GitHub Pages. Simply push changes to the repository and GitHub Pages will automatically build and deploy the site.

## Customization

### Adding Team Members

Add new team member files in the `_team/` directory with the following format:

```markdown
---
name: Team Member Name
title: Position Title
bio: Short biography
photo: /images/photo.jpg
order: 1
---
```

### Updating Content

The main content is in `index.md`. Edit this file to update the project description, research goals, and other sections.

### Styling

Custom styles are in `assets/css/style.css`. Modify this file to change colors, fonts, and layout.

## License

© 2026 Hawaiian Drosophila Genomes Project. All rights reserved.
