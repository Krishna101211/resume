# Resume

Auto-built PDF resumes from LaTeX source files.

## How It Works

Push any `.tex` file to `main` branch and GitHub Actions will automatically compile it into a PDF.

## Repository Structure

```
├── resume.tex          → resume.pdf
├── data_analyst.tex    → data_analyst.pdf
├── resume_sde.tex      → resume_sde.pdf
└── .github/workflows/build.yml
```

## Important Rules

- **`.tex` filenames must NOT contain spaces.** Use underscores or hyphens instead.
  - ✅ `data_analyst.tex`
  - ✅ `resume-sde.tex`
  - ❌ `data analyst.tex`
  - ❌ `my resume.tex`

## PDF Links

After a successful build, access your PDFs at:

```
https://github.com/Krishna101211/resume/raw/main/<filename>.pdf
```

Example:
- https://github.com/Krishna101211/resume/raw/main/resume.pdf
- https://github.com/Krishna101211/resume/raw/main/data_analyst.pdf
