---
name: Bug Report
description: File a bug report to help us improve PEGit
title: "[Bug]: "
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
        
  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Describe the bug and expected behavior...
    validations:
      required: true

  - type: textarea
    id: reproduction
    attributes:
      label: Steps to reproduce
      description: Steps to reproduce the behavior
      placeholder: |
        1. Run '...'
        2. Execute '...'
        3. See error
    validations:
      required: true

  - type: input
    id: version
    attributes:
      label: PEGit Version
      description: What version of PEGit are you running?
      placeholder: "e.g., 0.1.0"
    validations:
      required: true

  - type: dropdown
    id: os
    attributes:
      label: Operating System
      description: What operating system are you using?
      options:
        - macOS
        - Linux
        - Windows
        - Other
    validations:
      required: true

  - type: input
    id: python
    attributes:
      label: Python Version
      description: What Python version are you using?
      placeholder: "e.g., 3.11.0"
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste any relevant log output
      render: shell

  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our Code of Conduct
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
