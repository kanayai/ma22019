# MA22019: Introduction to Data Science

[![Quarto Publish](https://github.com/kanayai/ma22019/actions/workflows/publish.yml/badge.svg)](https://github.com/kanayai/ma22019/actions/workflows/publish.yml)

Course website for **MA22019 - Introduction to Data Science** at the University of Bath.

🔗 **Live Site:** [https://kanayai.github.io/ma22019/](https://kanayai.github.io/ma22019/)

---

## 📚 Course Overview

| Component | Details |
|-----------|---------|
| **Course Code** | MA22019 |
| **Level** | Year 2 Undergraduate |
| **Languages** | R and Python |
| **Duration** | 9 weeks |
| **Format** | 2 lectures + 1 lab + 1 problem sheet + 1 problem class per week |

### Learning Objectives

- Wrangle and explore data using tidyverse (R) and pandas (Python)
- Visualize data effectively using ggplot2 and matplotlib/seaborn
- Apply statistical models for inference and prediction
- Communicate findings through reproducible reports using Quarto
- Collaborate on data science projects using Git and GitHub

---

## 🛠️ Technology Stack

| Tool | Purpose |
|------|---------|
| [Quarto](https://quarto.org/) | Website generation and reproducible documents |
| [R](https://www.r-project.org/) + [tidyverse](https://www.tidyverse.org/) | Data wrangling and visualization |
| [Python](https://www.python.org/) + [pandas](https://pandas.pydata.org/) | Data analysis and machine learning |
| [GitHub Actions](https://github.com/features/actions) | Automated deployment |
| [GitHub Pages](https://pages.github.com/) | Website hosting |

---

## 📁 Project Structure

```
.
├── _quarto.yml              # Quarto configuration
├── index.qmd                # Homepage with 9-week schedule
├── course-syllabus.qmd      # Full syllabus and policies
├── course-overview.qmd      # Course description and prerequisites
├── course-team.qmd          # Teaching team information
├── course-support.qmd       # Getting help resources
├── course-links.qmd         # Useful links and references
├── styles.scss              # Custom styling (Bath branding)
│
├── computing-vscode.qmd     # VS Code setup guide
├── computing-terminal.qmd   # Terminal basics (Mac/Linux/Windows)
├── computing-git.qmd        # Git & GitHub visual guide
├── computing-assignments.qmd # Assignment workflow + 3-commit policy
│
├── lectures/                # Lecture materials
│   ├── week-01-lec-01.qmd
│   └── week-01-lec-02.qmd
│
├── labs/                    # Lab exercises
│   └── lab-01.qmd
│
├── problem-sheets/          # Weekly problem sets
│   └── ps-01.qmd
│
├── problem-classes/         # Problem class materials
│   └── pc-01.qmd
│
├── images/                  # Images and logos
│   └── bath-logo.svg
│
├── .github/workflows/       # CI/CD
│   └── publish.yml
│
├── ROADMAP.md               # Future plans (tracked for multi-Mac sync)
│
└── docs/                    # Built website (generated, gitignored)
```

---

## 💻 Computing Guides

The site includes comprehensive guides for students:

| Guide | Content |
|-------|---------|
| **VS Code Setup** | Installation, extensions (Python/R/Quarto), shortcuts |
| **Terminal Basics** | Mac, Linux, and Windows command line |
| **Git & GitHub** | Visual intro to version control |
| **Assignment Workflow** | GitHub submission + 3-commit grading policy |

---

## 🚀 Local Development

### Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) (v1.4+)
- [R](https://cran.r-project.org/) (v4.0+) with knitr and rmarkdown
- [Python](https://www.python.org/) (v3.9+) with Jupyter
- [VS Code](https://code.visualstudio.com/) with [Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto) (recommended)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kanayai/ma22019.git
   cd ma22019
   ```

2. **Install R packages (optional, for executable code):**
   ```r
   install.packages(c("tidyverse", "knitr", "rmarkdown"))
   ```

3. **Install Python packages (optional, for executable code):**
   ```bash
   pip install jupyter pandas numpy matplotlib seaborn
   ```

### Preview Locally

Start a live preview server with hot-reload:

```bash
quarto preview
```

This opens the site at `http://localhost:4567/` and automatically refreshes when you save changes.

### Build the Site

Generate the static site to the `docs/` directory:

```bash
quarto render
```

### Check Quarto Setup

Verify your Quarto installation:

```bash
quarto check
```

---

## 📤 Deployment

### Automatic Deployment (Recommended)

The site automatically deploys to GitHub Pages when you push to `main`. The GitHub Actions workflow:

1. Installs R and Python dependencies
2. Renders the Quarto project
3. Deploys to GitHub Pages

### Enable GitHub Pages

1. Go to repository **Settings** → **Pages**
2. Under **Build and deployment**, select **GitHub Actions**

### Manual Deployment

If needed, you can manually trigger the workflow from the **Actions** tab.

---

## ✏️ Adding Content

### Adding a New Lecture

1. Create a new file in `lectures/`:
   ```bash
   touch lectures/week-02-lec-01.qmd
   ```

2. Add YAML front matter:
   ```yaml
   ---
   title: "Week 2, Lecture 1: Your Title"
   ---
   ```

3. Update the schedule table in `index.qmd` with the link.

### Adding a New Lab/Problem Sheet

Follow the same pattern in `labs/` or `problem-sheets/` directories.

### Naming Conventions

| Content Type | File Pattern | Example |
|--------------|--------------|---------|
| Lectures | `week-XX-lec-YY.qmd` | `week-03-lec-01.qmd` |
| Labs | `lab-XX.qmd` | `lab-04.qmd` |
| Problem Sheets | `ps-XX.qmd` | `ps-05.qmd` |
| Problem Classes | `pc-XX.qmd` | `pc-06.qmd` |

---

## 🎨 Customization

### University of Bath Branding

Colors are defined in `styles.scss`:

| Color | Hex | Variable |
|-------|-----|----------|
| Granite | `#202329` | `$bath-granite` |
| Coral | `#EC0836` | `$bath-coral` |
| Cornflower | `#14C8E1` | `$bath-cornflower` |
| Steel | `#C7C7C7` | `$bath-steel` |
| Violet | `#673AB7` | `$bath-violet` |
| Mint | `#64FFDA` | `$bath-mint` |

### Modifying Navigation

Edit the `navbar` section in `_quarto.yml` to add/remove/reorder navigation items.

---

## 🤝 Contributing

1. Create a feature branch:
   ```bash
   git checkout -b feature/add-week-2-content
   ```

2. Make your changes and preview locally

3. Commit and push:
   ```bash
   git add .
   git commit -m "Add Week 2 lecture materials"
   git push origin feature/add-week-2-content
   ```

4. Create a Pull Request

---

## 📖 Resources

### Course Textbooks (Free Online)
- [R for Data Science (2e)](https://r4ds.hadley.nz/)
- [Python for Data Analysis (3e)](https://wesmckinney.com/book/)
- [Introduction to Modern Statistics](https://openintro-ims.netlify.app/)

### Quarto Documentation
- [Quarto Guide](https://quarto.org/docs/guide/)
- [Quarto Websites](https://quarto.org/docs/websites/)
- [GitHub Pages Publishing](https://quarto.org/docs/publishing/github-pages.html)

---

## 📄 License

Content © University of Bath, Department of Mathematical Sciences.

Built with [Quarto](https://quarto.org/).
