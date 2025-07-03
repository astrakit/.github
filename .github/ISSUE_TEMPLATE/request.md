name: Request
description: Use this template to request a new feature, improvement, or option.
labels: [request, enhancement]
body:
  - type: input
    id: title
    attributes:
      label: Request Title
      description: Short, descriptive title of your request.
      placeholder: e.g. "Add cat soundpack"
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: Description
      description: What would you like to see added or improved?
      placeholder: |
        - Explain the idea or feature you'd like to see.
        - Why is it useful?
        - Any examples or references?
    validations:
      required: true

  - type: checkboxes
    id: motivation
    attributes:
      label: Motivation
      description: What type of request is this?
      options:
        - label: New Feature
        - label: Improvement to existing feature
        - label: Other
    validations:
      required: false

  - type: textarea
    id: extra
    attributes:
      label: Extra Details (optional)
      description: Add any screenshots, sketches, or links that help explain your request.
    validations:
      required: false
