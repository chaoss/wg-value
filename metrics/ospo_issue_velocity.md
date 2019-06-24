# OSPO Issue Velocity

## 1. Description

Gives an OSPO manager a way to compare the speed of closed issues across a 
portfolio of projects. 

Speed of closing issues is a proxy for 'innovation'.  The faster the issue
turnover, the more innovation.

## 2. Use Cases

The OSPO manager can use the Issue Velocity metric to:
- report issue velocity of contributed vs in-house work
- compare project effectiveness across a portfolio of projects
- compare labor costs of open-source projects vs pure in-house developments

## 3. Formula

Base metrics include:
- number of issues
- number of issues broken out by contributor types (internal / external)
- broken out by time-periods (weekly / monthly / quarterly)

## 4. Sample Filter and Visualization

Potential filters:
- internal vs external contributors
- project sources: internal, open-source, competitor repos

We envision a time-series visualization that shows a line chart of monthly
issue velocity across a portfolio of repos.

## 5. Sample Implementation

TBD

## 6. Known Implementations

1. Augur

## 7. Test Cases (Examples)

1. Available in the Augur test schema for multiple repositories:

- Rails
- ReactJS
- SaltStack 
- etc.

## 8. External References (Literature)

- [Can Open Source Innovation work in the Enterprise?][l1]
- [Open Innovation for a High Performance Culture][l2]
- [Open Source for the Digital Enterprise][l3]

[l1]: https://www.threefivetwo.com/blog/can-open-source-innovation-work-in-the-enterprise

[l2]: https://www.nearform.com/blog/want-a-high-performing-culture-make-way-for-open-innovation/

[l3]: https://www.cio.com/article/3213146/open-source-is-powering-the-digital-enterprise.html

