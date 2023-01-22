Goal: Build a terminal app to manage a large collection of text notes [Python]

14/100 - 100 Days Of Code

**Day 14 Log: 21/01/2023**

**Today's Progress**:
- Worked on: Bug: Fix the setting of stores, making it possible to create a note in a different location
- #1 (Bug): 
- Above bug required a lot of exploration and research - no result
- Organised store commands under a sub-folder and then a subgroup in the cli app
- Updated the NotesStore class to use class annotations
- Updated the setup of context and context usage throughout the app
- Added command chaining: one command calling another


**Thoughts**: 
- Running the store commands in certain pattern shows that the context is not updating, after being changed: `pkmcli store status` -> `pkmcli store change` -> `pkmcli store status`
- The `pkmcli store change` delegates the status command and at that point it shows the correct value
- Yet at the 2nd `pkmcli store status`, ctx is reverted to original state, and the `change` is gone
- App still shows signs that the `ctx` is being reset between commands
- Setup seems to match documentation and online resources, could be a potential bug related to the environment
- Eliminated root cause from `add_command()` which adds commands after the fact
- Eliminated root cause from the construction of the NotesStore

**Next**: 
- Fix the setting of stores, making it possible to create a note in a different location
- Get back to adding tests
- Start testing on CI with Github Actions

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool