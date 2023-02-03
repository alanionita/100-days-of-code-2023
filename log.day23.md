Goal: Build a terminal app to manage a large collection of text notes [Python]

23/100 - 100 Days Of Code

**Day 23 Log: 02/02/2023**

**Today's Progress**:
- Github Actions: adds CI/CD workflow
- Github Actions: learned about running Conda within Action containers, updating environments, activating them etc.
- Github Actions: implemented an action that makes it easier to configure Conda environments - https://github.com/conda-incubator/setup-miniconda
- Github Actions: locally installed the package using `pip`
- Github Actions: added a CI/CD task to run the tests

**Thoughts**:
- Still feel like there's more to read on packaging Python apps - https://flask.palletsprojects.com/en/2.0.x/patterns/packages/

**Next**: 
- Fix CI/CD: fix tests; currently failing because of a hardcoded local path
- Fix CI/CD: add caching for packages and conda
- Package and deploy the module for PyPi

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool