# Documentation Repo
This documents everything I am learning

## Setup GitHub Pages Workflow
In GitHub go to Settings -> Pages. Change the deployment branch to gh-pages. gh-pages is where all files get published. publish-gh-pages.yml will publish the code whenever changes are pushed to the main branch.

## Create mkdocs.yml
This generates all static content. Create navigations as needed. That's it mkdocs is simple, minimalistic, and straight to the point.

## Run using Python

> Install mkdocs with Python
```text
pip install mkdocs
```

> Install mkdocs-material
```text
pip install mkdocs-material
```

> Optional show Python package locations
```text
pip show mkdocs
```

> Run locall if mkdocs in Path variable
```
mkdocs serve
```

> Run locally if mkdocs ```NOT``` in Path variable
```text
python -m mkdocs serve
```