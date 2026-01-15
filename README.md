# MA22019: Introduction to Data Science

Course website for MA22019 at the University of Bath.

## Local Development

### Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) (v1.4 or later)
- [R](https://cran.r-project.org/) (v4.0 or later)
- [Python](https://www.python.org/) (v3.9 or later)
- [VS Code](https://code.visualstudio.com/) with [Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto)

### Preview Locally

To preview the website locally, run:

```bash
quarto preview
```

This will start a local server and open the site in your browser. Changes will automatically reload.

### Render the Site

To build the static site (output to `docs/` folder):

```bash
quarto render
```

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the `main` branch. The GitHub Actions workflow handles:

1. Installing R and Python dependencies
2. Rendering the Quarto project
3. Deploying to GitHub Pages

## Project Structure

```
.
├── _quarto.yml           # Quarto configuration
├── index.qmd             # Homepage with schedule
├── course-syllabus.qmd   # Course syllabus
├── course-team.qmd       # Teaching team
├── course-overview.qmd   # Course overview
├── course-support.qmd    # Getting help
├── course-links.qmd      # Useful links
├── styles.scss           # Custom styling (Bath branding)
├── lectures/             # Lecture materials
├── labs/                 # Lab exercises
├── problem-sheets/       # Weekly problem sheets
├── problem-classes/      # Problem class materials
├── images/               # Images and logos
└── .github/workflows/    # GitHub Actions
```

## Contributing

1. Clone the repository
2. Make your changes
3. Preview locally with `quarto preview`
4. Commit and push to trigger deployment

## License

Content © University of Bath. Built with [Quarto](https://quarto.org/).
