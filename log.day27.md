27/100 : Build a terminal app to manage a large collection of text notes [Python]

100 Days Of Code

**Day 27 Log: 11/02/2023**

**Today's Progress**:
- Debugging Github Actions Day
- Started looking into simulating the runner locally using [act](https://github.com/nektos/act/blob/master/README.md), but `act` is configured to use small Docker images by default vs the standard 15gb Github Actions Runner image. Not quite what I'm looking for. 
- Added [tmate](https://github.com/mxschmitt/action-tmate) to the CI workflow
- With `tmate` found out that the default notes storage folder was missing. Managed to replicate the issue locally. Win for `tmate`, but need to make sure that I add a timeout to the step, otherwise it keeps my runner alive for far too long and could end up being costly.
- Fixed the bug that's triggered the debug session

**Thoughts**:
- Not sure `act` is an option here. The Docker image limitation seems reasonable, but stunting to anyone who isn't building a Node app on gh-actions. 
- Need to figure out how to remove it now. Also next time use something like nix to install - helps to keep the main environment clean.
- `tmate` aka a simple shell into my Github Action is exactly what I needed to discover the root cause of the bug.
- Looks like we might actually complete this project tomorrow. Fingers crossed!

**Next**: 
- Fix CI/CD: add caching for packages and conda
- Package and deploy the module for PyPi

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool