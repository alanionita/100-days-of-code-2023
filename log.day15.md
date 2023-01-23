Goal: Build a terminal app to manage a large collection of text notes [Python]

15/100 - 100 Days Of Code

**Day 15 Log: 22/01/2023**

**Today's Progress**:
- Started working through PY4E videos on OOP. Quite basic atm, but worth a refresh.
- BUG: context breaking across the running of commands
- Tried another Singleton + context pattern. No joy.
- Tried a pattern using environment variables. No joy because `click` spawns a new sub-process for each command runtime, so you end up with an empty environment.
- Tried a pattern using file-based storage. Working as expected across the running of each command.
- Implemented a context system based on a json file `context.json`


**Thoughts**: 
- Wow this took a lot longer than expected, but now I can change the location of these notes.
- I'm suprised by the `click` subprocess behaviour and the fact that the docs are really, really shallow. When I say `shallow` I'm still referring to a set of docs of above 50 pages [shrug].
- Seems strange that this behaviour has no prominent place in the docs since this is how you use git every day: `git status` (shows a state of the repo), `git add .` (updates the state), `git status` (now shows an updated state). Click somehow assumed that you would make those commands in other go - allowing `click` to share context properly. If you got through that process as normal `click` starts afresh for each command
- This is some niche CLI development experience.
- Excited to put this one problem behind me!

**Next**: 
- Get back to adding tests
- Start testing on CI with Github Actions

**Link to work**: 
- [Repo - pkm-cli-tool](https://github.com/alanionita/pkm-cli-tool