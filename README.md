# Resume

Auto-built PDF resumes from LaTeX source files.

## How It Works

Push any `.tex` file to `src/` folder on `main` branch and GitHub Actions will automatically compile it into a PDF in the `pdfs/` folder.

## Repository Structure

```
├── src/                    ← LaTeX source files
│   ├── resume.tex
│   ├── data_analyst.tex
│   └── manual_testing.tex
├── pdfs/                   ← Auto-generated PDFs
│   ├── resume.pdf
│   ├── data_analyst.pdf
│   └── manual_testing.pdf
├── .github/workflows/
│   └── build.yml
└── README.md
```

## Important Rules

- **`.tex` filenames must NOT contain spaces.** Use underscores or hyphens instead.
  - ✅ `data_analyst.tex`
  - ✅ `resume-sde.tex`
  - ❌ `data analyst.tex`
  - ❌ `my resume.tex`
- **Only place `.tex` files in the `src/` folder.**
- **Only changed `.tex` files are recompiled** — unchanged files are skipped.

## PDF Links

After a successful build, access your PDFs at:

```
https://github.com/Krishna101211/resume/raw/main/pdfs/<filename>.pdf
```

Example:
- https://github.com/Krishna101211/resume/raw/main/pdfs/resume.pdf
- https://github.com/Krishna101211/resume/raw/main/pdfs/data_analyst.pdf
