---
name: Feature request
about: Suggest an idea for this project
title: 'FEAT: featureTitle'
labels: enhancement
assignees: ''

---

<!--- Anything enclosed in arrow-bangs are comments to give you guidance and can be left --->

## User Story
<!--- Why to do this - A statement from a user's POV on what this feature will support.
Include for backend features as well to give higher-level context --->
<!--- Ref: https://martinfowler.com/bliki/UserStory.html --->

As a USER, I want to BLAH  So that BLAH

## Task
<!--- What to do - A task description written as an imperative to the developer --->

FE Ex. Add a profile screen to the app including the following fields ...
BE Ex. Modify the `/users` endpoint to take the following fields ...

## Acceptance Criteria
<!--- How to know when we are done - Expectation statements that when all are true, the task can be considered done.  --->
<!--- Ref: https://martinfowler.com/bliki/GivenWhenThen.html --->

### Scenario: User changes email - success
- **Given:** I have an account
  - **And** I want to change my email address

- **When:** I submit a new email address

- **Then:** My account should reflect the email address change
  - **And** I should be notified that the change was successful

### Scenario: User changes email - failure
- **Given:** I have an account
  - **And** I want to change my email address

- **When:** My email change request fails

- **Then:** My account should reflect the previous email address
  - **And** I should be notified that the change failed
