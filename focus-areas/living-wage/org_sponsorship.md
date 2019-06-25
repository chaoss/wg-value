# Org Sponsorship

## 1. Description

In a quest to earn a living wage, workers will be interested in knowing which
projects enjoy corporate support.

## 2. Use Cases

The worker can use the Org Sponsorship metric to discover which repos enjoy org
sponsorship.

## 3. Formula

Base metrics include:
- number of issues
- number of issues broken out by contributor types (internal / external)

Parameters include:
- hourly labor rate

Computed metrics include:
- cost per closed issue
- total labor cost


## 4. Sample Filter and Visualization

Potential filters:
- internal vs external contributors
- project sources: internal, open-source, competitor repos

We envision a time-series visualization that shows a line chart of monthly
labor costs across a portfolio of repos.

## 5. Sample Implementation

TBD

## 6. Known Implementations

1. Augur

## 7. Test Cases (Examples)

1. Available in the Augur test schema for multiple repositories:

- Rails
- ReactJS
- SaltStack 

## 8. External References (Literature)

- [Open Source Sponsors][l1]
- [Fiscal Sponsors and Open Source][l2]
- [Large Corporate OpenSource Sponsors][l3]

[l1]: https://opensource.org/sponsors

[l2]: https://opensource.com/article/19/1/fiscal-sponsors-open-source

[l3]: https://www.networkworld.com/article/2867020/big-names-like-google-dominate-open-source-funding.html

