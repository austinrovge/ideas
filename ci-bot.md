# ci-bot

Looking through some of the pull requests for [rust](https://github.com/rust-lang/rust) and [swift](https://github.com/apple/swift) I noticed that they have their own bots to handle running tests and merging into `main`. That would be cool to implement! Of course none of my side projects are big enough to warrant something like that, but it would be nice to be able to run ad-hoc commands for pull requests.

This can easily be achieved with GitHub actions for individual repositories by doing something like this:

```yml
on:
  issue_comment:
    types: [created]

jobs:
  do_work:
    name: Do work
    if: github.event.issue.pull_request && contains(github.event.comment.body, '!Zhu Li, do the thing!')
```

Which defeats the purpose of a bot like this. So what features could this have that a GitHub actions bot wouldn't easily have? Others like [bors](https://github.com/bors-ng/bors-ng) have integration with various CI platforms but I don't need that. Plus, just using GitHub actions would prevent coupling between individual projects and the bot. Maybe not worth creating!

### Scope

TBD

### Technologies

* Something yml - since everything CI uses it :eyeroll:
