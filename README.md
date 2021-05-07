# Cefas and EnvEast Python course 2020

https://ueapy.github.io/pythoncourse2020


Steps to generate pages using mkdocs:
1. Create and activate conda environment using environment.yaml

    1st time
    conda env create

    then
    conda activate mkdocs

2. Generate pages from markdown files and deploy to github as a branch gh-pages

    mkdocs gh-deploy --clean
