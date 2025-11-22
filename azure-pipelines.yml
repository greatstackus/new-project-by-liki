trigger:
- main   # Runs when you push to main branch

pool:
  name: 'Default'   # Use your self-hosted agent pool

steps:
- script: echo "Hello World from Azure DevOps Self-Hosted Agent!"
  displayName: 'Print Hello World'

- script: |
    echo "Checking current directory:"
    cd
    echo "Listing files:"
    dir
  displayName: 'Show workspace details'

- script: echo "Pipeline completed successfully!"
  displayName: 'Final Step'
