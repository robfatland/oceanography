# Geosmart Use Case Jupyter Book

Badges: <BR><BR>


[![Deploy](https://github.com/geo-smart/use_case_template/actions/workflows/deploy.yaml/badge.svg)](https://github.com/geo-smart/use_case_template/actions/workflows/deploy.yaml)
[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://geo-smart.github.io/simple-template)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/geo-smart/simple-template/HEAD?labpath=book%2Fchapters)
[![GeoSMART Use Case](./book/img/use_case_badge.svg)](https://geo-smart.github.io/usecases)


How this repository was initiated from the 'simple' skeleton use case book at the Geo-Smart organization.<br>

- I knew there were two templates: A simple one (in use here) and a more comprehensive version
    - The website to view these and existing books is [here](https://geo-smart.github.io/usecases).
- Clicked "Use This Template"; named the new repository (appearing in my personal organization) **`oceanography`**
    - Made sure to click on 'include all branches'
    - I have an existing repository **`ocean`**: Will be the basis of this Jupyter book
        - I am starting with a blank slate here
- Started editing this `README.md` to trace my steps
- Notice that instructions include **edit `environment.yml`**... how to create this file?
    - Read up on Python and environments
    - Install the `conda` package manager
        - I use `miniconda`
        - I then install packages / libraries as needed
    - From a working (*activated*) environment I run: `conda env export > environment.yml`
        - There is a corresponding path using `pip freeze` that produces the analogous `requirements.txt` file
        - The `yml` approach seems to be more recent / flexible (also accommodates requirements-style) 
Remaining instructions: 

2. In your repository edit book/_config.yml
3. Under your repository Settings --> Pages --> Source = GitHub Actions
4. Edit environment.yml, modify notebooks, and your JupyterBook will be published for you! 
