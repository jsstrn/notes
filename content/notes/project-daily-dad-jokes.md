---
title: "Daily Dad Jokes"
summary: "How I built an event-driven serverless Telegram bot"
categories: ["development", "projects"]
tags: ["node.js", "serverless", "telegram api", "aws", "aws lambda", "aws cloudwatch"]
---

I created a Telegram channel to deliver dad jokes every day. I did not want to be build a Node.js server and host it on Digital Ocean or Linode because that would be cost inefficient. Instead, I wanted to build an event-driven serverless architecture. We can achieve this with [AWS Lambda](https://aws.amazon.com/lambda/) for the lambda functions and [AWS CloudWatch](https://aws.amazon.com/cloudwatch/) to trigger the lambda through scheduled events.

I first built a Telegram bot and then added it to the Telegram channel. The bot fetches a dad joke from [icanhazdadjoke.com](https://icanhazdadjoke.com/api) and publishes it to the channel. The last step was to schedule a daily trigger to run the lambda function on a regular schedule.

You can view the [Daily Dad Jokes](https://t.me/s/DailyDadJokes) public channel. If you have a Telegram account you can also subscribe to the [channel](https://t.me/DailyDadJokes).
