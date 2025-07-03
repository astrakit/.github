name: Task
description: Use this template for actionable items that require implementation or changes.
labels: [task, enhancement]
body:
  - type: input
    id: summary
    attributes:
      label: Task Summary
      description: Briefly describe what needs to be done.
      placeholder: e.g. "Migrate from Datalix to 24Fire server"
    validations:
      required: true

  - type: textarea
    id: details
    attributes:
      label: Details
      description: Provide more context, requirements, or steps for this task.
      placeholder: |
        - What needs to be migrated?
        - Any downtime expected?
        - Specific data or configs to consider?
    validations:
      required: false

  - type: input
    id: deadline
    attributes:
      label: Deadline (optional)
      placeholder: e.g. "2025-07-10"
    validations:
      required: false

  - type: input
    id: assignees
    attributes:
      label: Assignees (optional)
      placeholder: GitHub usernames
    validations:
      required: false
