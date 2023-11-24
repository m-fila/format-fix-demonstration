# format-fix-demonstration

Repository to demonstrate how `pre-commit` might be used to simplify formatting CI actions in CERN envrioment with `cvmfs`.

Two actions are used:
1. 'pre-commit' - checking the formatting with `pre-commit`. In case of bad formatting the actions fails and displays readable [message](
https://github.com/m-fila/format-fix-demonstration/actions/runs/6972452177/job/18974645762#step:4:183) in the log.
2. 'pre-commit-fix' - on demand autofixing triggered by a [comment](https://github.com/m-fila/format-fix-demonstration/pull/1#issuecomment-1824723300 on the pull request.

Alternativel, an automtic autofixing can be achieved with external [pre-comit.ci](https://pre-commit.ci/) application or 'pre-commit.ci lite' action. In either case a 3rd party app should be installed on target reposity though.
