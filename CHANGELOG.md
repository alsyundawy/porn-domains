# Changelog

This changelog documents changes to the structure, file handling, and background processes related to the domain list. Changes to the lists themselves, such as added or removed domains, are not included here as they can be reviewed directly from the [commit history](https://github.com/search?q=repo%3ABon-Appetit%2Fporn-domains+%22%5BAUTO%5D+Update+list%22&type=commits&s=committer-date&o=desc).

**Format of date is: YYYY-MM-DD**

## 2025-03-15

- DNS checks are now enforced again. They are performed directly after combining the domains across all sources. We will monitor the results to ensure everything works as expected. If you encounter any issues, please send an email to mail@codealdente.ovh.
- DNS checks will exclude whitelist sources. Until we can ensure the results are accurate, a new file named `block.txt.dns_ok` will be placed next to `block.txt`. The `block.txt.dns_ok` file will contain DNS-validated domains, while `block.txt` will include all combined and deduplicated domains from all blacklist sources. **Please note that `block.txt.dns_ok` is TEMPORARY and WILL BE REMOVED once we confirm the results are consistently correct.**

## 2025-03-03

- New whitelist source added to exclude more than 10,000 university domains ([fe30ee9](https://github.com/Bon-Appetit/porn-domains/commit/fe30ee9f677fdfa8f60b3ef3efd0499de9c29b44))

## 2025-03-01

Sources for blacklisting will be considered outdated if they have not been updated within three years. The condition for the archived state will be ignored from now on. [Read more here](https://github.com/Bon-Appetit/porn-domains/discussions/43#discussioncomment-12317915)

## 2025-02-03

- New whitelist source added to exclude common news sites ([9f4f9e4](https://github.com/Bon-Appetit/porn-domains/commit/9f4f9e44574dfd7e90cc8d97bba42cec8d3a315b))

## 2024-12-20

- 24 new blacklist sources added ([08e538a](https://github.com/Bon-Appetit/porn-domains/commit/08e538a211a326062ccdc789bbcac016f3003e38))
- Blacklist source "blocklistproject" updated ([ec41ce9](https://github.com/Bon-Appetit/porn-domains/commit/ec41ce9d25ccf8c1a4bb6d609237e591713308d2))

## 2024-11-21

- **"Outdated" sources are now excluded**: For more details, please [read this](https://github.com/Bon-Appetit/porn-domains/discussions/43#discussioncomment-11306946).
