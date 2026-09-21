# Scoring methodology

Last updated: September 21, 2026. Applies to the historical 2024 regular-season Week 1 demo.


The current scoring version is `mvp-1`. Players count toward their final college before entering the NFL, including undrafted players. The snapshot uses season-roster college metadata resolved through the school registry; transfer histories have not yet been exhaustively verified.

A player participates with at least one offensive, defensive, or special-teams snap. Players without a college affiliation remain in the snapshot but are excluded from college rankings.

### Individual points

| Offensive statistic | Points |
| --- | ---: |
| Passing yard | 0.04 |
| Passing touchdown | 4 |
| Interception thrown | -2 |
| Rushing or receiving yard | 0.1 |
| Passing, rushing, or receiving two-point conversion | 2 |
| Individual touchdown (rushing, receiving, defensive, or return) | 6 |
| Lost fumble | -2 |

There are no reception points or yardage bonuses. Individual touchdowns and lost fumbles are credited once using play-by-play, including special-teams events.

| Defensive statistic | Points |
| --- | ---: |
| Primary tackle, solo or with assistance | 1 |
| Tackle assist | 0.5 |
| Sack | 4 (fractional sacks prorated) |
| Interception | 4 |
| Forced fumble | 2 |
| Opponent fumble recovery | 2 |
| Pass defended | 1 |
| Individually credited safety | 2 |

Distinct events stack: an interception returned for a touchdown earns interception and touchdown points. Safeties without an individually credited player earn no individual points.

| Special-teams statistic | Points |
| --- | ---: |
| Extra point made | 1 |
| Extra point missed or blocked | -1 |
| Field goal made, under 40 yards | 3 |
| Field goal made, 40–49 yards | 4 |
| Field goal made, 50+ yards | 5 |
| Field goal missed or blocked | -1 |
| Kickoff or punt return yard | 0.04 |
| Blocked kick | 2 |
| Punt inside the 20 | 1 |
| Punt touchback | -1 |

The source reports missed and blocked kicking attempts separately; both receive the miss penalty. Long snapping itself does not earn points.

### Offensive line estimate

Offensive linemen make up nearly half the offense on the field, but their individual contributions are difficult to measure with standard box-score statistics. We include an estimate so their contribution counts toward their schools' scores.

For each NFL team, take the mean offensive fantasy score of its QB/RB/WR/TE players who played at least 25% of offensive snaps. Each lineman receives that mean multiplied by their offensive snap share, plus any directly credited individual events.

This estimate rewards linemen on NFL teams with higher-scoring skill players, even though that output depends on more than blocking. Within the same NFL team, offensive snap share is the only distinction between linemen in this estimate; it does not measure individual blocking quality. Directly credited events can still change their final scores. Future versions may use a more individual measure of offensive-line performance as suitable data becomes available.

Fullbacks are excluded from the skill-player pool, and defensive/return points do not enter its mean. Snap shares use the source's published percentages, rounded to two decimal places.

### College and flair-pair rankings

- **Total:** sum of all participating alumni's points.
- **Average:** total points divided by participating alumni. Zero and negative scores count, with no minimum player count or additional snap threshold.
- **Pair total:** sum of the two schools' totals.
- **Pair average:** combined total divided by combined participating players, rather than the mean of the two school averages.

The 25% snap threshold applies only to the offensive-line reference pool. It does not filter players from school averages. Small schools can therefore have high averages based on very few players.

Pair rankings include every unique unordered pair of supported schools, counting each school once. Scores are stored to six decimal places and displayed to two. Ties use competition ranks (1, 2, 2, 4), with alphabetical ordering within ties.

### Data quality

The historical snapshot is provisional. Snap participants without a weekly stat row receive zero observed individual event stats. Identity corrections for Alec Anderson and Detroit's Chris Smith, and a quarantined Josh Gable stat row, are recorded in the snapshot's `quality` metadata. Source roster college labels take precedence over conflicting player metadata.

## Sources and attribution

Statistics are derived from [nflverse](https://github.com/nflverse/nflverse-data), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), and modified for alumni scoring. Inputs include weekly player statistics, snap counts, season rosters, player metadata, and play-by-play. Flair mappings use the public [r/CFB Flair Wizard catalog](https://cfb.flairwizard.com/). School-pair rankings compare school combinations, not individual Reddit users.

[Documentation home](README.md)
