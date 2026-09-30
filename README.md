# workflow_run artifact-trust reproduction

Security research harness. Empirically tests documented GitHub Actions behaviour:
whether a `workflow_run` workflow can be steered to check out and execute an
arbitrary repository whose identity came from an artifact produced by an
unprivileged `pull_request` run, and whether repository secrets are exposed to
that code.

Mirrors the structure of `google-gemini/gemini-cli`'s `trigger_e2e.yml` +
`chained_e2e.yml`. Contains no real credentials; `TEST_SECRET` is a dummy value.
