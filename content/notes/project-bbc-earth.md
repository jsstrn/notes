---
title: "BBC Earth videos on Telegram"
summary: "Your daily dose of BBC Earth on Telegram"
categories: ["projects"]
tags: ["bbc", "telegram", "youtube", "api"]
---

I created a Telegram channel to share videos from the BBC Earth YouTube channel. Since this project did not warrant a server to be up 24/7, I leveraged on a serverless architecture to keep the cost low. I used [AWS Lambda](https://aws.amazon.com/lambda/) for the lambda functions and [AWS CloudWatch](https://aws.amazon.com/cloudwatch/) to trigger the lambda through scheduled events.

First, I built a Telegram bot which fetches a random video from the BBC Earth YouTube channel and publishes it to the Telegram channel. I then have it run on a daily schedule.

[BBC Earth Daily](https://t.me/s/BBCEarthDaily) is made publicly available for all to enjoy. If you are on Telegram, you can subscribe [here](https://t.me/BBCEarthDaily). The code is [open sourced](https://github.com/jsstrn/bbc-earth-daily) so you can fork it and build your own.
