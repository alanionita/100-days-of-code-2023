Goal: Build a terminal app to manage a large collection of text notes [Python]

21/100 - 100 Days Of Code

**Day 21 Log: 31/01/2023**

**Today's Progress**:
- Finalised the `generators / file` tests.
- Adds tests for `generators / notes`.
- Learned about session test fixtures, which I used to create a `beforeAll` hook that clears a file created by tests before another round of tests runs.
- Learned about a different mocking and patching pattern applied to datetime and strftime.
- Coverage at 48%.

**Thoughts**:
- Getting close to completing the generators tests to 100% coverage. Most of them are over 85%. All are over 65%.
- Strangely hit 100% coverage on generators / notes a lot earlier than expected. Seems like the coverage is throwing a false positive there, so I spent some time to cover most of the pathways for that generators module.
- Feels like the command tests should be a lot more repeatable.
- Test don't feel very DRY.

**Next**: 
- Get back to adding tests
- Start testing on CI with Github Actions

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool