---
layout: post
title: Week notes
date: 2020-10-09
---

This week has been rather hectic, early starts and late evenings. I've tried to keep the post short and sweet: new team things, celebrating Black Tech, the mysterious case of the inexplicable log lines, and can't let it go.

### All the new team things

This week I joined a new team, a team which has nearly doubled in size. 

It was a blur of 1-1s, a fast-tracked session on the team charter, and reading up on trello protocols and etiquette.

The whole week got me thinking about on-boarding and the different experiences I've had across companies and teams: what's worked, what's not worked as well, and what-I-definitely-would-never-do-again.

It also made me reflect on _why_ on-boarding is so critical, worth getting right, and worth celebrating –– but so hard to convince people is necessary.

I'd love to delve into this more. 

### Celebrating Black History Month

We're celebrating Black History Month where I work. One of the ways we're celebrating is by posting weekly in Slack channels on Black excellence in that channel's theme (e.g., tech, mental health, sustainability).

If you don't know about these incredible organisations<sup>*</sup> that celebrate BlackTech, well, you should:

- [UKBlackTech](https://ukblacktech.com/)
- [AfroTech Fest](https://www.afrotechfest.co.uk/)
- [Coding Black Females](https://codingblackfemales.com/)
- [Black in AI](blackinai.org)
- [BLCK VC](blckvc.com)
- [Black Women in Tech](https://www.techlondonadvocates.org.uk/working-groups/black-women-in-tech/)
- [colorintech](colorintech.org)
- [Somalis In Tech](somalisintech.com)
- [Melanin.Tech](https://twitter.com/MelaninTech)
- [Black Tech Pipeline](blacktechpipeline.com)
- [Women in Tech Caribbean Community](https://twitter.com/WomenCaribbean)
- [blackdevslondon](https://twitter.com/blackdevslondon)
- [amplify](amplifytech.uk)
- [Black Female Founders](blackfemalefounders.org)
- [Coders of Color](https://twitter.com/CodersofColor_)

Also check out [the 50 most inspiring, prominent, and influential black voices in UK tech](https://technation.io/news/50-inspiring-black-voices-uk-tech-scene/).

There isn't a pipeline problem, there's a hiring problem.

<sup>*</sup>This list is not exhaustive. There are more. Do the research.

### The mysterious case of the inexplicable log lines

Recently I noticed something mysterious going on in one of our log groups. 

I don't want to go into to much detail here, but effectively we have FreeRadius running in a container. It talks to Foo API and a logging API. 

Every time FreeRadius receives a request from a client it should make *one* call to Foo API to do some foo things and then *one* call to the logging API to log what it did. This is what the radius configuration indicates it is doing.

But no.

For some, but not all, clients there are *two* calls to Foo API and *one* call to our logging API. The two calls are milliseconds apart.

The plot thickens.

During an AWS networking outage these double calls stopped.

Now they're back.

As one of the team's networking sleuths, I **will** get to the bottom of this (I've got a few hypotheses already).

### Can't let it go

This week in our tech community channel we celebrated the work of [Dr. Anne-Marie Imafidon](https://aimafidon.com/), computer scientist, speaker, and advocate for women finding a role in tech. She's awesome. You can [follow her on twitter](https://twitter.com/aimafidon) and [read her blog](https://aimafidon.com/blog/).

In researching her work, I realised that Dr. Imafidon is one of the reasons I became a developer.

I met her back in December 2013 when I attended a [Stemettes](https://stemettes.org/) event at [Makers](https://makers.tech/). At the time I was deciding between pursuing a PhD in organisational culture or trying a career in tech.

Hearing her speak about all the ways women can find joy and purpose in STEM fields was life changing. I'd never thought of myself as someone who could belong in a tech role. 

I applied to Makers the following weekend.