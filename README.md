# format-fix-demonstration

Repository to demonstrate how `pre-commit` might be used to simplify formatting CI actions in CERN environment with `cvmfs`.

Two actions are used:
1. 'pre-commit' - checking the formatting with `pre-commit`. In case of bad formatting the actions fails and displays readable [message](https://github.com/m-fila/format-fix-demonstration/actions/runs/7015709215/job/19085498016#step:4:182) in the log.
2. 'pre-commit-fix' - on demand autofixing triggered by a '/fix-style' [comment](https://github.com/m-fila/format-fix-demonstration/pull/2#issuecomment-1829291517) on a pull request.

Alternatively, an automtic autofixing can be achieved with external [pre-comit.ci](https://pre-commit.ci/) service or 'pre-commit.ci lite' action requiring a 3rd party app installed on a repository.
