You are helping triage a new GitHub issue. Arguments: $ARGUMENTS

Steps:
1. Parse REPO and ISSUE_NUMBER from the arguments.
2. Use mcp__github__get_issue to read the full issue (title, body, existing labels).
3. Analyze the content and choose the most appropriate label(s) from: bug, enhancement, question, documentation, duplicate, help wanted, needs-triage.
4. Apply the chosen label(s) with mcp__github__update_issue.
5. If the issue is clearly a duplicate of an existing open issue, also add a comment via mcp__github__create_issue_comment linking to the original.

Do not add more than three labels. If no label fits confidently, apply "needs-triage".
