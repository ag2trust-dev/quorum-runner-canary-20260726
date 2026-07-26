# Disposable canary instructions

- This repository exists only for Quorum task #205 end-to-end validation.
- Follow the complete role contract in the daemon prompt.
- Workers must make only the requested small text-file change, push their assigned branch,
  open a PR, and use `quorum submit`.
- Reviewers must inspect the PR and repository state, post the required `### Code review`
  comment, and submit the derived verdict. Never merge or formally approve.
- Do not weaken branch protection, checks, approval rules, sandbox, or merge policy.
- Verification is `test -s canary.txt`.
