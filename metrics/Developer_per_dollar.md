# {Developer per dollar}

Question: Would it be cheaper for a company to build software in house, or invest in open source software instead?

## Description
The most expensive thing about software is paying programmers to make the thing. Instead of hiring up to complete a project, a company could just invest in an ongoing open source project to reach the same number or more developers than they could hire for that money.
To someone not involved with programming in a business deciding how to go about building software, seeing the value in having many contributors on a project could help them decide.

## Objectives
If an ongoing open source project has many contributors, then a business could invest less money than it would take to salary that many programmers and achieve equivalent results.

## Implementation
This metric would look at the number of people contributing to a project
sources for contributers can come from other metrics
- contributors: https://github.com/chaoss/wg-evolution/blob/master/metrics/contributors.md

### Filters
Developer per dollar = company investment / total contributors 

### Data Collection Strategies
Total contributors -known by those working on the project / observable from the project's github / CHAOSS metrics
Company investment -known by the company investing
