# Vahab Jabrayilov's Personal Website

This is a Jekyll-based academic profile website for Vahab Jabrayilov, PhD Candidate in Computer Science at Columbia University.

## About

This website showcases:
- Personal bio and research interests
- Education background
- Work experience
- Publications
- CV/Resume

## Site Structure

The site is built using Jekyll and organized as follows:

```
├── _config.yml          # Site configuration
├── _data/
│   ├── bio.yml          # Personal biography
│   ├── education.yml    # Educational background
│   ├── experience.yml   # Work experience
│   ├── publications.yml # Publications list
│   ├── teaching.yml     # Teaching positions
│   └── awards.yml       # Awards and honors
├── _includes/           # Reusable HTML components
├── _layouts/            # Page templates
├── assets/
│   ├── css/            # Stylesheets
│   ├── images/         # Images (profile, logos)
│   └── pdf/            # Documents (resume)
└── index.markdown      # Homepage
```

## Local Development

### Prerequisites

- Ruby
- Jekyll
- Bundler

### Running Locally

```bash
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.

## Deployment

This site is configured for GitHub Pages. It automatically deploys when changes are pushed to the main branch.

## Updating Content

### Personal Information

Edit `_config.yml` to update:
- Name, email, and URLs
- Social media links
- Profile image path

### Biography

Edit `_data/bio.yml` to update your personal bio.

### Education

Edit `_data/education.yml` to add or modify educational entries.

### Experience

Edit `_data/experience.yml` to add or modify work experience.

### Publications

Edit `_data/publications.yml` to add or modify publications.

## License

Based on the panjason.github.io template.
