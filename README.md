# Saturdays on Sunday

Saturdays on Sunday is a Reddit app that groups NFL players by college and ranks schools by their alumni's performance. It includes total and average rankings, individual player breakdowns, and two-school rankings selected manually or from your Reddit flair.

The current version is a historical demo using 2024 regular-season Week 1. Scores are provisional; automatic weekly updates are not yet available. Moderators control when rankings posts are created.

## Background

I often found myself watching NFL games just to follow players I liked in college. As a Texas fan, after years of feeling like my school didn't have much of a presence in the NFL, I was excited to see more familiar players making their way into the league. I wanted to keep up with how they were doing and see how they stacked up against players from other schools.

There are a few sites that track college alumni in the NFL, but I couldn't find one place that brought together the players, their stats, and school rankings. So I decided to build the view I wanted to use.

I've mostly been a lurker on r/CFB, and Reddit felt like the right home for this. My hope is that it gives college football fans something to follow and discuss between Saturdays, when most of the football on offer is in the NFL.

## Documentation

- [Scoring methodology](scoring.md)
- [Terms and Conditions](terms.md)
- [Privacy Policy](privacy.md)

## AI use during development

Yes, AI was used in the development of this app. That being said, I do have nine years of professional experience as a software engineer, much of it before AI coding tools were available.

Honestly, I think I'm a pretty good use case for vibe coding because I was never a particularly good coder to begin with. AI generally writes better code than I ever did. What I do have is accumulated scar tissue and a reasonable sense of what I don't know. In my experience, those unknowns are where a lot of the pitfalls show up when someone without that background uses AI to build software.

I also think this app is a good fit for agentic coding because the stakes are relatively low. It ranks football stats; it doesn't provide critical functionality or ask users for sensitive information like passwords, payment details, or health data. It does use Reddit account context and flair to select schools, so there are still privacy considerations to take seriously.

That said, I've taken care to review the code and check the functionality, drawing on the many, many MRs and PRs I've reviewed as a team lead. That doesn't mean I've caught everything, but I'm applying that experience here and taking responsibility for what I ship.

## Contact

Developer: [u/letseatbreakfast](https://www.reddit.com/user/letseatbreakfast/)

Support and privacy requests: [u/letseatbreakfast via Reddit private message](https://www.reddit.com/message/compose/?to=letseatbreakfast)

Do not include sensitive information in public GitHub issues.

## Publication status

The Terms and Privacy Policy have been reviewed by the developer and are effective September 21, 2026. Recheck the Privacy Policy when live data fetching or storage is added.

This repository contains public-facing documentation only. It does not grant a license to the app's source code. Third-party data and materials retain their respective licenses.
