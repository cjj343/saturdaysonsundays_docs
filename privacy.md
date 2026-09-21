# Privacy Policy

Effective date: 21SEP2026

## Scope and operator

This policy describes the current historical-demo version of Saturdays on Sunday, operated by [u/letseatbreakfast](https://www.reddit.com/user/letseatbreakfast/) ("the developer"). It covers the app's own handling of information. Reddit hosts the app through Devvit and processes information under its [Privacy Policy](https://www.reddit.com/policies/privacy-policy).

## Information used and why

- **Reddit account context and flair:** when you open the school-pair view, the app requests your current Reddit user through Reddit's API and reads your r/CFB flair text and CSS class to identify schools. In the configured development subreddit, it reads that test subreddit's flair instead. The app receives account context through Reddit; it does not ask for your Reddit password.
- **School selections:** the app sends selected school IDs to its own server to retrieve combined scores and ranks. Manually selecting schools changes the displayed pair, not your Reddit flair. Choosing manually does not prevent the initial flair lookup when the pair view opens.
- **Search and display preferences:** school search text, ranking mode, and selections are held in the current app view. School-name filtering happens in the browser. Ranking mode is sent to the app's server when loading rankings.
- **Community and post context:** the app uses installation context to select the appropriate flair source and to support moderator-requested post creation. Created posts remain on Reddit under Reddit's normal post controls.

The flair response returns recognized school IDs and a lookup status, rather than your username or raw flair text. Pair leaderboards rank school combinations, not user accounts.

## Storage and logs

The current app does not maintain a persistent user-profile database or save account identifiers, flair, searches, or school selections in an app-managed database. It does not set its own tracking cookies or save selections in browser local storage. View state lasts while that view is mounted; it is not a saved account preference. Flair responses instruct clients not to cache them.

The server logs errors if moderator-requested post creation fails. Error messages may contain operational context supplied by Reddit. Reddit may also maintain platform request logs, security records, and usage analytics independently of the app. Their retention is governed by Reddit's platform practices; this policy does not promise deletion of Reddit-controlled records on a developer-defined schedule.

If you contact the developer, the communication includes the account or email address you use and any information you choose to provide. Those messages are handled through the contact service you use. Please send only information needed to resolve your request.

## External services and sharing

The current app serves bundled NFL data; it does not yet make runtime nflverse downloads. It has requested permission for future server-side downloads from `github.com` and `release-assets.githubusercontent.com`. The planned downloads retrieve public sports datasets and do not require sending Reddit usernames, flair, or school selections to those hosts. This policy will be reviewed before that functionality is released.

Flair Wizard mappings are bundled with the app; opening the app does not send your flair to Flair Wizard. The app does not include third-party advertising or tracking SDKs, or sell user information.

If you follow an external source or documentation link, that service receives your visit and handles it under its own policies. In particular, GitHub-hosted documentation is subject to [GitHub's Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Your choices and requests

You can select schools manually, change your subreddit flair through Reddit, or stop using the app. Signed-out visitors can use manual selection where Reddit allows access. Subreddit moderators control installation and app posts.

Contact [u/letseatbreakfast via Reddit private message](https://www.reddit.com/message/compose/?to=letseatbreakfast) with privacy questions or access, correction, or deletion requests. The developer will address requests concerning information under their control, subject to applicable law. The app currently has no saved user-profile or selection record to delete. Requests concerning Reddit account data, platform logs, or Reddit posts may need to be made through Reddit's own controls and support. Avoid posting personal information in public issues.

## Changes

Updates to this policy will appear here with a revised effective date. Material changes to data handling will also be identified in the app's release notes or description.

[Documentation home](README.md)
