# new-project-by-liki
trigger:
- main

pool:
  vmImage: 'ubuntu-latest'     # Runs on Microsoft-hosted agent
  # If using self-hosted agent, replace with:
  # name: 'Default'

steps:
- script: echo "Hello from Azure Pipeline!"
  displayName: 'Print Hello'

- script: |
    echo "Current directory:"
    pwd
    echo "Listing files:"
    ls -la
  displayName: 'Show workspace details'

- task: Bash@3
  inputs:
    targetType: 'inline'
    script: |
      echo "Pipeline completed successfully!"
  displayName: 'Final step'

