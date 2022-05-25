# Templates repository

Hosts the reusable workflows available to all repositories in the organization

## Sample

For an example of a workflow that references a reusable workflow, see the starter-template workflow located at https://github.com/msfred/.github/blob/main/workflow-templates/react-cicd.yml.

## Usage

```
jobs:
  # Build React app
  build:
    name: Build React app
    uses: msfred/templates/.github/workflows/build-react.yml@main
    with:
      project: MyReactApp
    secrets:
      token: ${{ secrets.token }}
```
