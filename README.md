# amalinifernando.github.io

Personal academic website of **Amalini Fernando**, Ph.D. candidate in Political Science at the University at Albany (SUNY).

Built with Jekyll using the [Minimal Academic Site](https://github.com/minimalacademicsite/minimalacademicsite.github.io) template (MIT License), which is based on [Academic Pages](https://github.com/academicpages/academicpages.github.io).

## Where to edit content

| What | File |
| --- | --- |
| Name, title, email, LinkedIn, Google Scholar, CV path | `_config.yml` (the `author:` section) |
| Header tabs (Work, Research, Teaching, CV) | `_data/navigation.yml` |
| Biography and research interests (home page) | `_pages/about.md` |
| "Featured" links on the home page | `_data/featured.yml` |
| Work experience | `_data/work.yml` |
| Papers and their links | `_data/papers.yml` |
| Conference presentations | `_data/presentations.yml` |
| Classes on the Teaching page | `_data/teaching.yml` |
| Course materials hubs (one page per course) | `_teaching/rpos-303.html`, `rpos-399.html`, `rpos-522.html` |
| CV PDF (linked from the CV tab and the sidebar button) | `files/Amalini_Fernando_CV.pdf` |
| Profile photo | `images/` (then set `avatar` in `_config.yml`) |

### Adding course materials

1. Put the files (PDFs, slides, etc.) in `files/teaching/<course>/`, e.g. `files/teaching/rpos-303/syllabus.pdf`.
2. List them in the front matter of the course page in `_teaching/`, under `syllabus:` and `materials:` (there is a commented example in each file).

Sections with nothing listed show a "coming soon" note.

## Local preview

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open http://localhost:4000.
