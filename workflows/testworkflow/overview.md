# Workflow Info
See [nf-testworkflow repo](https://github.com/formbio/nf-testworkflow) for more information regarding this workflow and its development

Current version: 1.0.0

# Test Cases
This workflow is only available in the [sbx-uat project](https://sbx.bantha.tundra.bio/organizations/sbx-uat/projects/sbx-uat/home/).

## Cypress
[workflow-launcher.cy.ts](https://github.com/formbio/colossal/blob/1f7155be32535e3d9fd1720a04dd0a7df97deb9b/services/web-client/cypress/e2e/workflow-launcher.cy.ts) lays out a cypress test for walking through all the workflow launcher's current functionality. Test cases can be examined in code there.

Note: The cypress test verfies that the workflow is launched with the correct parameters but does not actually launch a workflow.

## Manual
Users can also manually smoke test the workflow launcher's functionality by walking through it in the sbx-uat project [here](https://sbx.bantha.tundra.bio/organizations/sbx-uat/projects/sbx-uat/workflows/nf-testworkflow/testworkflow/spreadsheet/?version=v0.1.0&uploadedOrg=1045298e-a419-4d2a-9dd6-9c84a9f869c6&uploadedProj=40c9baa0-9156-4e5e-a784-f3ffffd022ef)

Notes:
- For file-related inputs, there is a directory called **test-workflow-files_DO_NOT_DELETE** that contains all variations of files needed to complete the steps in this workflow's launcher
- Descriptions have been written for higher lever overviews of each step and input within each step
- The side info drawer contains the test cases that should be accounted for in each step. These should be synced with the same cases cypress will be testing for.
