# zabbix-slack-bot
---
A Slack bot to interact with the Zabbix API using the Slack messaging application. It works as a plugin using the python-rtmbot module.

With this bot it is possible to request Zabbix to perform actions and list information on request.

## Dependencies
---
- python-rtmbot (https://github.com/slackhq/python-rtmbot)

## Installation
---
1. Download the python-rtmbot code
```sh
$ git clone https://github.com/slackhq/python-rtmbot.git
$ cd python-rtmbot
```
2. Install dependencies (virtualenv is recommended.)
```sh
$ pip install -r requirements.txt
```
3. Create a new bot user in Slack (https://api.slack.com/bot-users)
4. Set the token of the created bot at python-rtmbot
```sh
$ cp docs/example-config/rtmbot.conf .
$ vi rtmbot.conf
  SLACK_TOKEN: "xoxb-11111111111-222222222222222"
```
5. Download zabbix-slack-bot
```sh
$ cd plugins/
$ git clone https://github.com/batangamedia/zabbix-slack-bot
```