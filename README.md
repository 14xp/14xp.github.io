# Minimal Personal Website

A minimal, accessible personal website with landing page and writing section, designed for sharing writings and research results. Built with pure HTML/CSS and optimized for speed, accessibility, and AI crawlability.

## Features

- **Landing page with centerpiece video** - Clean entry point with navigation to all sections
- **Minimal HTML style** - Fast loading with minimal dependencies
- **Tufte-style footnotes** - Elegant sidenotes that become toggleable on mobile
- **LaTeX math support** - Beautiful mathematical notation via KaTeX
- **Inline HTML embedding** - Support for interactive content and visualizations
- **AI-accessible** - Follows principles from gwern.net/llm-writing for maximum crawlability
- **Organized content structure** - Logical hierarchy with all content under pages/

## Structure

```
website/
├── index.html                # Landing page with video centerpiece
├── assets/                   # Static assets
│   ├── css/
│   │   └── style.css        # Minimal stylesheet
│   ├── images/
│   │   └── favicon.png      # Favicon
│   └── media/
│       └── waves.mov        # Landing page video
├── pages/                   # All user-facing content
│   ├── about.html          # About page
│   ├── writing.html        # Writing listing page
│   ├── talks.html          # Talks and presentations
│   └── posts/              # Individual writing posts
│       ├── example-post.html
│       └── getting-started.html
├── feeds/                  # Syndication
│   └── rss.xml            # RSS feed
├── config/                 # Configuration files
│   ├── _config.yml         # GitHub Pages configuration
│   ├── robots.txt          # Crawler instructions
│   └── sitemap.xml         # Sitemap for search engines
└── README.md              # This file
```

## Setup for GitHub Pages

1. Create a new repository on GitHub
2. Upload these files to the repository
3. Go to Settings → Pages
4. Set source to "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Your site will be available at `https://yourusername.github.io/repositoryname`

## Customization

### Update Personal Information

Replace placeholders in all files:
- `Your Name` → Your actual name
- `yourusername` → Your GitHub username
- `website` → Your repository name (if different)

### Adding New Posts

1. Create a new HTML file in the `pages/posts/` directory
2. Copy the structure from `pages/posts/example-post.html`
3. Add the post entry to `pages/writing.html`
4. Update `config/rss.xml` and `config/sitemap.xml`

### Customizing the Landing Page

- Replace `assets/media/waves.mov` with your own video
- Update `assets/images/favicon.png` with your favicon
- Modify navigation links in `index.html` as needed

### Styling

The CSS in `assets/css/style.css` is intentionally minimal. Key features:
- Landing page with centered video and navigation
- Responsive sidenotes that collapse on mobile
- KaTeX math styling
- Clean typography with Palatino font
- Mobile-first responsive design

## Design Philosophy

This writing site prioritizes:
- Content over complexity
- Accessibility for all users and AI systems
- Fast loading times
- No build system dependencies
- Semantic HTML structure
- Long-term maintainability

Inspired by Dan Luu, Gwern, and other minimal web design practitioners.