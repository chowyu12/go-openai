# Upstream synchronization

- Repository: https://github.com/sashabaranov/go-openai
- Release: v1.43.0
- Commit: 95e34b8feea9913544cb655069a1b59df9cde993
- Synchronized: 2026-10-13

This fork retains its `github.com/chowyu12/go-openai` module path and
Go 1.25.3 minimum. The sanity and compatibility jobs use that minimum to keep golangci-lint
compatible with the Go compiler export data.

The fork's `ChatCompletionRequest.ExtraBody` still merges vendor parameters
into the root JSON object. The pre-existing local change omitting empty
content from tool-call messages is also preserved.
