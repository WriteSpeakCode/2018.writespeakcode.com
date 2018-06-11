# 2018.writespeakcode.com
[2018 Conference Website](https://2018.writespeakcode.com)

## Contributing

Please take a look at our [contributing](CONTRIBUTE.md) guidelines (coming soon!).

We have volunteers who work on our website to make sure it is up-to-date for all of our events. You are welcome to work on it too!

### Installation

1. `git clone https://github.com/WriteSpeakCode/2018.writespeakcode.com.git`
1. Open `index.html` in your favorite browser
1. Profit!

### Create a pull request

- Create changes on a feature branch, **squashing all your work into 1 commit**
- Submit a pull request to the `master` branch
 - `master` branch must always be deployable, do not merge your branch until accepted by Jessica or team
- Deploy to staging (see below)
- Ping the [website team on Slack](https://writespeakcode.slack.com/messages/2018_conf_website/) for comments

### Publish

Our site is deployed to Heroku. If you have rights, you can publish
the site there (ping Jessica if you don't). The workflow is as follows:

#### Deploy to staging:

- `git pull origin master` to get latest update
- `git rebase master` on your branch (to prevent regression!)
- Navigate to [staging deployment page](https://dashboard.heroku.com/apps/writespeakcode2018-staging/deploy/github)
- Scroll to `Manual deploy` & select your branch from `Deploy a GitHub branch`
- Click the `Deploy Branch` button
- Verify that [staging looks & works right](https://writespeakcode2018-staging.herokuapp.com/index.html)
 - Looks good on Chrome, Safari, and mobile
 - Link to sponsor prospectus works
 - Link to ticketing works
 - Your feature works
- Ping Jessica [on Slack](https://writespeakcode.slack.com/messages/@jarmstrong/) for acceptance
- Move Trello card to `QA` column

#### Once your work is verified & accepted:

Merge your branch to master on GitHub & delete your branch

Push to Heroku production:

- Navigate to [production deployment page](https://dashboard.heroku.com/apps/writespeakcode2018-production/deploy/github)
- Scroll to `Manual deploy` & select 'master' branch from `Deploy a GitHub branch`
- Click the `Deploy Branch` button
- Verify the [production website](https://2018.writespeakcode.com/)
 - Looks good on Chrome, Safari, and mobile
 - Link to sponsor prospectus works
 - Link to ticketing works
 - Your feature works

Move Trello card to Done

Celebrate! :tada:
