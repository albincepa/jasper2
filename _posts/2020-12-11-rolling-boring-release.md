---
layout: post
current: post
cover:  assets/images/kevin-mueller-Q-fL04RhuMg-unsplash.jpg
navigation: True
title: Why Your Releases Needs to be Rolling & Boring?
date: 2020-12-10 19:30:00
tags: [tech]
class: post-template
subclass: 'post'
author: albince
---

**TL;DR:** Add features incrementally to production. Make Releases a routine task so that it becomes boring.

Are you excited about your next release?

Do you have **No deploy Fridays**? Are you waiting for the client's business closing hours for production deployment?

If something is keeping you on your toes for the next production release, you need to improve.

---


## Keep the Code Rolling

The aim is to get the code to be on production deployment as soon as possible. [Time to production](https://en.wikipedia.org/wiki/Lead_time){:target="_blank"} should be minimised at all cost.

The agile method advocates keeping the tasks atomic. For this to work, the **Definition of Done** should be clearly stated for each task.

If something is marked as done after the different phases of **Automated testing, QA verification and Product Owner's approval**, why should it be further delayed to production.

Something that shouldn't be accessible to the end user, can be hidden using [Feature Flags](https://devops.com/5-best-practices-for-feature-flagging/){:target="_blank"}. With the page/component behind the feature flag, you get to test your task while on production. This task can be further re-iterated by issuing subsequent tasks.

---

![Thing on Fire](assets/images/stephen-radford-hLUTRzcVkqg-unsplash.jpg "A cute kitten")

## Minimise the Risk and Blast Radius
Things may and will go wrong sometimes. This is applicable even if your release is occurring every Month/Quater/Year. But with incremental changes being delivered, the Definition of Done should include the steps required in case things go sideways.

This may include 
- Automated Database Snapshots before deployment
- Rollback scripts in case of a destructive upgrade
- [A/B testing](https://vwo.com/ab-testing/){:target="_blank"}
- [Different update strategy](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#strategy){:target="_blank"}

---

![Calm Cat in Bed](assets/images/edan-cohen-iSIiW--ACDs-unsplash.jpg "A cute kitten")


## Boring Deployments

Keep the deployments as boring as you can. The chimes in Teams/Slack during the production release/deployment needs to be minimal. 

Having a nightly job for production release may be a bit ambitious(Or is it **:P**). But with a click of a button, the continuous deployment tool should deploy the new release to the production environment. 

To ensure a sound release, you can check the current status and analytics using tools like [Grafana](https://grafana.com/){:target="_blank"}. Also having a fine-tuned alert system, like [Prometheus](https://prometheus.io/){:target="_blank"} is encouraged.


**Keep Calm and Enjoy Life**
