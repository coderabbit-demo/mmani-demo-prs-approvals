---
id: jira-work-item
name: Jira Work Item
mode: error
report: platform
---
Pass only when the PR title or description references a Jira work item in the SC project
(for example SC-123) and the change stays within that work item's scope. Fail when no SC
key is referenced, or when the PR includes changes the work item does not ask for; list
those changes.
