# Dingo Tiles - Ask for Help: Slackbot

This is the source code for the `dingobot` in our http://slack.dingotiles.com/ outback land of Support & Sales help.

In any channel type `/download`:

![](http://cl.ly/3y0b3a113n0L/download/Image%202016-02-18%20at%203.08.48%20pm.png)

## Configuration of Slack commands

See https://dingotiles-askforhelp.slack.com/apps/A0F82E8CA-slash-commands

## Deployment

```
cf push --no-start
cf set-env slackbot DOWNLOAD_S3_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_S3_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_HAPROXY_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_HAPROXY_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_KAFKA_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_KAFKA_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_POSTGRESQL_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_POSTGRESQL_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_PROMETHEUS_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_PROMETHEUS_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_REDIS_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_REDIS_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_SECRETS_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_SHIELD_SLACK_TOKEN tokenxx
cf set-env slackbot DOWNLOAD_SHIELD_RC_SLACK_TOKEN tokenxx
cf set-env slackbot DINGOTILES-ASKFORHELP_IN_URL  https://hooks.slack.com/services/xxx/yyy/zzz
cf set-env slackbot AWS_ACCESS_KEY access
cf set-env slackbot AWS_SECRET_KEY secret
cf restart slackbot
```
