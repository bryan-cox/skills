# Issue tracker: Jira

Issues for this repo live in Jira. Use the installed `acli` CLI for issue-tracker operations, not GitHub Issues, `.scratch/`, or the Atlassian MCP.

## Conventions

- The project key is not fixed. Determine it from the task or parent issue. Ask if it is ambiguous; do not guess.
- Search: `acli jira workitem search --jql "<JQL>" --json`.
- Read: `acli jira workitem view <KEY> --json`.
- Create: `acli jira workitem create --project <PROJECT_KEY> --type <TYPE> --summary "<summary>"`; follow that project's required fields and issue conventions.
- Edit, link, comment, or transition with the corresponding `acli jira workitem` command, then verify the result.
- If the CLI is unavailable or unauthenticated, ask for help rather than switching trackers.
