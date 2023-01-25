Goal: Build a terminal app to manage a large collection of text notes [Python]

18/100 - 100 Days Of Code

**Day 18 Log: 25/01/2023**

**Today's Progress**:
- Back from a little 2day holiday in Bali (I wish!!!)
- Started by adding coverage reports and updating dependencies
- Damn - just 6% coverage
- Added a new `TESTING.md` readme to figure out where to start the testing
- Added tests for the `generators/store` module
- Coverage up to 17%. Winning!!!

**Thoughts**: 
- Dreading the tests but look, they ALWAYS improve your implementation
- `generators/store` was interesting because I was making some call-based assumptions that meant my function would only run correctly if run at a certain level in the project tree. Very nasty! 
- `generators/store` also is a method that reads a file, but contained a path generation method within. This is the method that had the tight coupling mentioned
- Equally `generators/store` depends not only on this .json file existing, but also on a specific key to exist.
- No question about it, I think I picked the right starting point for the testing and without a bit of planning + chucking it all in a file (for your perusal) was beneficial. Put it this way: last module I wrote tests for got prioritised last. 

**Next**: 
- Get those test coverage score into the 90's (the best generation)
- Start running tests on CI with Github Actions
- Upload module to `pypi`

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool