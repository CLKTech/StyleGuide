### Commit

All commit messages should be present imperative tense. Commits should be 
relatively frequent. Use your best judgment, but if your commit message
is going to be longer than a sentence or two your commit is probably too big


### Branching


##### Master

Each master branch merge should be coupled with a new version tag. Ex (v0.1 to v0.2).
The dev/development branch is the only branch that is allowed to merge into the
master branch. 


##### Server

If we deem it necessary we will also include a server branch which is a higher
level master branch


##### Dev/Development

No one is allowed to directly push to the dev branch. It'll contain the most up
to date code, and should be pulled from frequently. All test are required to pass
in order to push to merge with the dev branch. For merging to the dev branch
the developer is required to pull and merge the dev branch into their specific
feature branch. Then once everything is ready the developer will submit a pull
request into the dev branch. Pull request will be code reviewed for proper 
CLKTech styling and then merged.


##### Feature

All work will be done off feature branches, and then merged into the dev branch.
Developer are allowed to make as many feature branches as they deem necessary.
2 developers shouldn't be working on the same feature branch at once, unless
there's a good reason that was communicated before hand. If one developer wants
to use the code in another devs feature branch they are allowed to pull code
and create their own branch, and even submit pull request, but they should not
directly push to a feature branch that isn't there's unless previously discussed.


### Learning Git

If you don't know git [here's a great resource](http://learngitbranching.js.org/)
