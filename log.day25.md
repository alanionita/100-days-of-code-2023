25/100 : Build a terminal app to manage a large collection of text notes [Python]

100 Days Of Code

**Day 25 Log: 06/02/2023**

**Today's Progress**:

- BUG: get_store() testing util fails in CI
- Likely an uncaught / unhandled error in the `store status` command
- Tracked down the issues to the `init` command + the use of the `store status` command
- Seems like the issue stems from having multiple locations for the `context.jso`

**Thoughts**:
- 2days off for rest + chores

**Next**: 
- Fix CI/CD: fix remaining tests
- Fix CI/CD: add caching for packages and conda
- Package and deploy the module for PyPi

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool