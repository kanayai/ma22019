# MA22019 Course Website - Roadmap

This file tracks future plans and is synced via Git for multi-Mac workflow.

## ✅ Completed
- [x] Initial site structure with 9-week schedule
- [x] Bath University branding (colors, styling)
- [x] All main pages (syllabus, overview, team, support, links)
- [x] Computing guides:
  - [x] VS Code Setup (extensions for Python/R/Quarto)
  - [x] Terminal Basics (Mac/Linux/Windows)
  - [x] Git & GitHub visual guide
  - [x] Assignment Workflow (3-commit policy)
- [x] GitHub repository and Actions workflow
- [x] Comprehensive README and .gitignore

## 📋 Next Steps

### Deployment
- [ ] Enable GitHub Pages: Settings → Pages → GitHub Actions
- [ ] Verify site at https://kanayai.github.io/ma22019/

### Content Population
- [ ] Add instructor info to `course-team.qmd`
- [ ] Set actual dates in schedule and syllabus
- [ ] Create Week 1 lecture content
- [ ] Create Week 1-9 labs and problem sheets

### GitHub Classroom
- [ ] Create GitHub Organization: `github.com/ma22019`
- [ ] Set up GitHub Classroom
- [ ] Create template repos for assignments

---

## Multi-Mac Workflow

```bash
# On new machine
git clone https://github.com/kanayai/ma22019.git
cd ma22019
quarto preview

# Before switching machines
git add . && git commit -m "message" && git push

# On other machine
cd ma22019 && git pull
```
