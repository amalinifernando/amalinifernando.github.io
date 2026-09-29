# amalinifernando.github.io

Personal academic website of **Amalini Fernando**, Ph.D. candidate in Political Science at the University at Albany (SUNY).

Built with Jekyll using the [academic-homepage](https://github.com/luost26/academic-homepage) template by Shitong Luo (MIT License).

## Where to edit content

| What | File |
| --- | --- |
| Name, bio, contact links, education, experience summary, awards | `_data/profile.yml` |
| Navigation bar | `_data/navigation.yml` |
| Publications, op-eds and policy briefs (one file each) | `_publications/` |
| News items on the homepage (one file each) | `_news/` |
| Conference presentations | `_data/presentations.yml` |
| Courses and teaching roles | `_data/teaching.yml` |
| Work experience, service, media, editorial work, skills | `_data/cv.yml` |

To add a portrait, put a photo at `assets/images/photos/portrait.jpg` and uncomment `portrait_url` in `_data/profile.yml`.
To link a CV, add a PDF under `assets/files/` and uncomment `cv_link`.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

## Publishing

In the repository's **Settings → Pages**, set the source to *Deploy from a branch* and choose the branch that contains this site (e.g. `main`, root folder). The site will be served at https://amalinifernando.github.io.
