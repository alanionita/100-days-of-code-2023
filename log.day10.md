Goal: Build a terminal app to manage a large collection of text notes [Python]

100 Days Of Code - Log

**Day 10: 17/01/2023**

**Today's Progress**:
- Improved dependencies by include the correct dependencies in the setup.cfg, and only having click in the conda environment
- Replaced the `python-frontmatter` package with a simpler solution using pyyaml and regex matching
- General tidy up of the docs and placement of .md files: move them outside of src

**Thoughts**: 
- Figured out where the stray `frontmatter` package was coming from, it was a typo in the setup.cfg. This was installing the dependencies each time I used pip to install the module locally. Really was driving me crazy! 
- I should be able to enable the VSCode Python extension and Pylance, since Pylance was complaining about a missing method from the `python-frontmatter` which has now been removed
- Just shows you that it's usually better to DIY! 

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool