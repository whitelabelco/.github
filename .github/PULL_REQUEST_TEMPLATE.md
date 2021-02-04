<!--- In a PR, you are presenting an implementation to a reviewer. Depending on the reviewers role, they may not have the full context of the problem you are trying to solve, why you chose this implementation, or how to test it. The more detail you provide here translates into a better review of the code and less questions in the process -->
# DescriptiveTitleHere
<!-- "One"-liner: A brief description for the PR-->
This branch adds a spinner to be displayed while data is loaded in the background

## Resolves
<!-- Call out the issues that this PR will resolve -->
Resolves: Issue #35

## Description of Changes
DescribeChangesMadeInParagraphForm

## How to Test
<!-- Guide the reviewer on how to observe evidence of the changes you made in action to give proof that they are working. This depends on the PR. It can be steps to run tests, observations in a locally running service, QA-type steps to follow, all or any of the above. -->
##### Run the unit tests
You might need to update installed packages by running `npm i`

Run `npm run tests`

<!-- For frontend changes -->
#### Observe the interface changes
All tests should pass

Run `npm run start`

Browse to: `http://localhost:8000/fantastic-spinner`

Oberserve that a spinner is rendered when data is loading

<!-- For backend changes -->
#### Observe the endpoint changes
Run `npm run start`

Query `GET http://localhost:8080/fantastic-endpoints?color=green`

Supported query params and values include:

<!-- Add some failure scenarios when appropriate -->
##### Suggested failure scenarios
Stop backend or change config to point to a non-existing site

Browse to: `http://localhost:8000/fantastic-spinner`

Oberserve that a spinner is rendered for 5 seconds then gives an error message
