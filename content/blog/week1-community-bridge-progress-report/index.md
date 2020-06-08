---
title: Week 01 - Progress Report with Community Bridge
date: "2020-06-03"
description: "After 30 years and 1 week of lock down, I am feeling productive (Just kidding, i am just 20 😂). Ready to roll with me again? 😉"
---

![Thanos Project](./isolated.gif)
<center><sub>LOCK DOWN & SELF-ISOLATED</sub></center><br/>

After 30 years and 1 week of lock down, I am feeling productive (Just kidding, i am just 20 😂). Ready to roll with me again? 😉

I completed the first week of [my internship](https://soniasingla.com/cncf-intern-with-thanos/) at [Cloud Native Computing Foundation](https://www.cncf.io/) with [Thanos](https://people.communitybridge.org/project/f51284ab-f652-47b1-9819-cd4135e75c00) under the mentorship of [Bartek Plotka](https://www.bwplotka.dev/) and [Povilas Versockas](https://povilasv.me/). At the beginning of the week, I had video call meeting with my mentors, Bartek and Povilas, we talked about the contribution workflow, Introduction to communication channels and had Initial discussions about the project and how to start further. They also explained me about the **LTS (Long Term Storage)** course, how it works and provided me some good issues to start with to have good understanding of the code base.

## WORK DONE :

![Thanos Project](./workdone.gif)
<center><sub>WORK DONE</sub></center><br/>

During the past first week, I worked on automating the TOC (Table of Content) on pages having more than 400 words. [Hugo](https://gohugo.io/) can automatically parse Markdown content and create a Table of Contents which we can use in our templates. The following is a partial template(smaller, context-aware components) that adds slightly more logic for page-level control over TOC (Table of Contents).

```HTML
{{ if and (gt .WordCount 400 ) (.Params.toc) }}
<aside>
    <header>
    <h2>{{.Title}}</h2>
    </header>
    {{.TableOfContents}}
</aside>
{{ end }}
```

For more details, you can visit the site [here](https://gohugo.io/content-management/toc/#template-example-toc-partial). The pull request is under progress, you can check it out [here](https://github.com/thanos-io/thanos/pull/2689) 😻😈

Revised the first existing [Katacoda](https://www.katacoda.com/) tutorial **"[Global View and seamless HA for Prometheus](https://www.katacoda.com/thanos/courses/thanos/1-globalview)"** that transformed vanilla Prometheus to basic [Thanos](https://thanos.io/) deployment enabling:

1. Reliable querying multiple Prometheus instances from single [Prometheus API endpoint](https://prometheus.io/docs/prometheus/latest/querying/api/#expression-queries).
2. Seamless handling of Highly Available Prometheus (multiple replicas).

I managed to provide some short nits that could be more useful, the pull request could be found [here](https://github.com/thanos-io/thanos/pull/2691) 🚀.

Apart from that, I am working on the proposal for the second Katacoda tutorial **"Downsampling and unlimited metric retention for Prometheus"** which we can expect to be in GitHub issue of [Thanos](https://thanos.io/) before the completion of second week.

I managed to send 2 pull requests by the end of my first week, and it's the wonderful feeling 😇❤️

## PLANS FOR NEXT WEEK :

![Thanos Project](./planning.gif)
<center><sub>PLANNING TIME</sub></center><br/>

1. Complete the proposal for **"Downsampling and unlimited metric retention for Promothesus"**.
2. Go through all the documentation of [Thanos](https://thanos.io/), play with all the components and fix all the broken links.
3. Make changes requested for the Pull Requests which are under review.
4. Prepare a short 5 min talk on **"Downsampling and unlimited metric retention for Promothesus"** to be delivered in Mentees Hangout Meet on Friday 🤗

It is a good experience till now, and I look forward to more contributing, learning and growing ! 😇

**Signing off for today, until next week** 👻

**:wq**