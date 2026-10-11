# h4la-issue-pr-alerts

To be notified when an issue/ PR opens up, depending on labels

### Setup:

- Fork this repo.
- Create an issue in your repo where the alerts will be posted as comments. Make sure you are subscribed to the issue (see button on right panel of issue). Note the number of that issue (likely #1).
  - _Recommendation_: Lock the issue with the "Lock conversation" button found in the bottom of the panel on the right. This makes it so only you (and the github-actions bot via the GH_TOKEN) and any collaborators are the only ones who can comment, to avoid extra notifications from subscribing to the issue.
- go to .github/workflows/pr-label-alert.yml and update the env: variables to match the REPO and LABEL you want to check for, and the amount of time you'd like the Github Action to LOOKBACK.

### To test your Github Action:

Including "workflow_dispatch" allows us to trigger the workflow manually. To do so, click the "Actions" tab across the top while in the repo, select the Action from the sidebar on the left, and click the "Run workflow" drop-down --> "Run workflow" drop down (with `main`, or whatever your default branch is, selected). Only entities with write access will be able to trigger your action manually.

### To disable the workflow:

Go to the Actions tab for this repo, click the "PRs with label Alert" action, and click the three dots ("...") to the right side of the screen. You'll see an option to disable the workflow from that dropdown.
