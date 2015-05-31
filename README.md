# Slack invite automation using sinatra

## Usage

### Deploy Heroku

Click below button

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)


[![imgur](http://i.imgur.com/7u7o0PT.png)]



### Use Docker

```
docker run -d \
  -e SLACK_TEAM_NAME="Slack Team Name" \
  -e SLACK_TEAM_DESC="welcome to slack" \
  -e SLACK_TOKEN="xoxp-xxxxxxx" \
  -e SESSION_SECRET_KEY="your random string" \
  -p 8080:80 \
  subicura/slack_invite
```

## Config

Environments list

* SLACK_TEAM_NAME
  * Your slack team name
* SLACK_TOKEN
  * Your slack api token. get from https://api.slack.com/web#auth
* SESSION_SECRET_KEY
  * For encrypt session data. first make random text and use it.
* SLACK_TEAM_DESC
  * Description of your slack
* optional environments
  * BACKGROUND_COLOR
  * TEXT_COLOR
  * EMAIL_BACKGROUND_COLOR
  * EMAIL_TEXT_COLOR
  * BUTTON_COLOR
  * BUTTON_HOVER_COLOR
  * BUTTON_TEXT_COLOR

## Reference

* [Slack의 팀 초대를 자동화 할 수 있는 "Slack Invite Automation"](http://blog.outsider.ne.kr/1117)
  * [node.js web application](https://github.com/outsideris/slack-invite-automation)
* [How I hacked Slack into a community platform with Typeform](https://levels.io/slack-typeform-auto-invite-sign-ups/)
* [Socket.io Join the Community](http://socket.io/slack/)
* [Sign Up From](http://codepen.io/erikapdx/pen/BnfjH)
  * Thanks for raccoony(Docker Korea Slack) find this design
