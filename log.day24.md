24/100 : Build a terminal app to manage a large collection of text notes [Python]

100 Days Of Code

**Day 24 Log: 03/02/2023**

**Today's Progress**:

- Created new command for initialising the store file - init command 
- Adds tests for this new command
- Updates create command tests to use this new init commmand
- Fixes path dependencies that were breaking tests on the CI


**Thoughts**:
- Still some bugs to fix to get the CI/CD to go green. This time around the bug is weirder and I haven't been able to replicate locally

**Next**: 
- Fix CI/CD: fix tests; currently failing because of a hardcoded local path
- Fix CI/CD: add caching for packages and conda
- Package and deploy the module for PyPi

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool