# Geosmart Use Case Jupyter Book

Badges: <BR><BR>


[![Deploy](https://github.com/geo-smart/use_case_template/actions/workflows/deploy.yaml/badge.svg)](https://github.com/geo-smart/use_case_template/actions/workflows/deploy.yaml)
[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://geo-smart.github.io/simple-template)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/geo-smart/simple-template/HEAD?labpath=book%2Fchapters)
[![GeoSMART Use Case](./book/img/use_case_badge.svg)](https://geo-smart.github.io/usecases)


I advocate for documenting process. Here is how the Geo-Smart organization 'simple skeleton' source repository was used to create a Jupyter Book version of my oceanography work.<br>


- I knew there were two templates available: The simple one (in use here) and a more comprehensive version
    - The website to view these (plus existing books) is [here](https://geo-smart.github.io/usecases).
- From the simple template I followed the 4-step directions...
    - Clicked "Use This Template"; named the new repository (appearing in my personal organization) **`oceanography`**
        - Made sure to click on 'include all branches'
        - I have an existing repository **`ocean`**: Will be the basis of this Jupyter book
            - I am starting with a blank slate here
    - Started editing this `README.md` to trace my steps
    - Edited `book/_config.yml` file to reflect this fork to `my-org/oceanography`
        - Presumably this will get bounced back over to the geo-smart org: For a later day
    - Settings --> Pages --> Source = GitHub Actions
        - To do (?): Enable github pages
    - Notice that instructions include **edit `environment.yml`**... how to create this file?
        - Read up on Python and environments
        - Install the `conda` package manager
            - I use `miniconda`
            - I then install packages / libraries as needed
        - From a working (*activated*) environment I run: `conda env export > environment.yml`
            - There is a corresponding path using `pip freeze` that produces the analogous `requirements.txt` file
            - The `yml` approach seems to be more recent / flexible (also accommodates requirements-style) 


Remaining instructions: 

- Edit environment.yml, modify notebooks, and your JupyterBook will be published for you! 
- edit conda/environment.yml, filling it in with your dependencies (don't worry about the platforms section, in fact you may delete that)
- in the book/chapters folder, add the full, runnable jupyter notebook
- in the book/chapters folder, add split up versions of the notebook however you'd like to split up chapters
- add the file paths for the chapters from the step above to book/_toc.yml (if you followed the same naming scheme of one, two, three etc. then you just have to delete any excess entries in the TOC)
- in the github repository, enable github pages
- push all changes
