## Labor Investment

Goal: Estimate the labor investment in open source projects.

| Name                                                      | Question                                                                                                                                   |
|-----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| [Labor investment by organization](./labor_investment.md) | What was the cost of an organization for its employees to create the counted commits, issues, and pull requests (and other contributions)? |
| [Issue velocity](./issue_velocity.md)                     | What is the development speed for an organization?                                                                                         |
| Commit count by organization                              | How many commits do employees of an organization create?                                                                                   |
| Issue count by organization                               | How many issues do employees of an organization create?                                                                                    |
| Pull request count by organization                        | How many pull requests do employees of an organization create?                                                                             |
| COCOMO by organization                                    | What is value contributed by employees of an organization as measured by COCOMO?                                                           |
| Labor cost by organization                                | What was the cost of an organization for its employees to create the counted commits, issues, and pull requests (and other contributions)? |
| Labor investment by commits by organization               | How much value in commits was contributed by an organization?                                                                              |
| Labor investment by issue by organization                 | How much value in issues was contributed by an organization?                                                                               |
| Labor investment by pull requests by organization         | How much value in pull requests was contributed by an organization?                                                                        |

Comments / Discussion:

- Codebase cost / code counting
- Complexity measures
- Potentially find an average time required for commit/issue/pull request and then apply an assumption of how much that is worth.
- Implementation note: Issues and pull requests are not stored in a repository and will have to be calculated from a collaboration platform like GitHub or other issue trackers.

