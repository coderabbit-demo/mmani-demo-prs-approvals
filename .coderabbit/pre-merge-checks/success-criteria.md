---
id: success-criteria
name: Success Criteria
mode: error
report: platform
---
Read the linked Jira work item in project SC and find its "Success criteria" list (items
S1, S2, ...). Evaluate every criterion against this PR's code, schema, and tests. For
each, report Met, Not met, or Not verifiable, with the file and line that shows it.

A criterion is Met only when the code implements it AND a test asserts the stated values;
a test asserting different values does not count. Fail if any criterion is Not met. Pass
only when all criteria are Met.
