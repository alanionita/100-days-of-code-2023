26/100 : Build a terminal app to manage a large collection of text notes [Python]

100 Days Of Code

**Day 26 Log: 10/02/2023**

**Today's Progress**:
- Fixed local context related testing issues - this is previous issue I described as 'cannot be replicated' locally. I since found a way to match up the environments,
- Uncovered another issues now with the CI and this time around it's even trickier.

**Thoughts**:
- This actually was a multi-day debugging session, but haven't posted since there's not been any code changes, just a variety of tests and trials.
- Wondering of a bunch of things: is conda configured correctly within the CI, am I running the right commands for it, is the file system slightly different or are the file path structures different

**Next**: 
- Fix CI/CD: fix remaining tests [new]
- Fix CI/CD: add caching for packages and conda
- Package and deploy the module for PyPi

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool