# jira-slack [![Build Status](https://travis-ci.org/24i/jira-slack.svg?branch=master)](https://travis-ci.org/24i/jira-slack)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/24i/jira-slack)

This is a JIRA-Slack integration, it does the following:

* Sends summaries of issues to your selected channel
* Links to the issues on your JIRA location
* Links mail adresses to the issue creator and assignee

## Install and Run

Run the following things to install:

```
git clone git@github.com:24i/jira-slack.git
cd jira-slack
npm install

# set your env variables
export JIRA_URL=https://your-jira-location.atlassian.net
export SLACK_HOOK_URL=https://hooks.slack.com/services/HOOK-PARAMS

npm start
```

This will run the integration server and you can now add it as a JIRA WebHook

## Environment variables
* `JIRA_URL` - The location of your JIRA installation (either your own or cloud)
* `SLACK_HOOK_URL` - The incoming slack hook URL generated by slack

## Running tests
Running the tests is easy as pie, just run the following command `npm test` and it'll run all of the tests for you

## Contributing
You can find more info about contributing at [contributing.md](contributing.md)