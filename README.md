# h4la-issue-pr-alerts

To be notified when an issue/ PR opens up, depending on labels

### Setup:

- Fork this repo.
- Create an issue in your repo where the alerts will be posted as comments. Make sure you are subscribed to the issue (see button on right panel of issue). Note the number of that issue (likely #1).
- go to .github/workflows/pr-label-alert.yml and update the env: variables to match the REPO and LABEL you want to check for, and the amount of time you'd like the Github Action to LOOKBACK.

### To test your Github Action:

### To disable the workflow:

Go to the Actions tab for this repo, click the "PRs with label Alert" action, and click the three dots ("...") to the right side of the screen. You'll see an option to disable the workflow from that dropdown.
