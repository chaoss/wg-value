# CHAOSS Value Metrics CHANGELOG

## 2020 June

Building off the relaunch to include value as aligned with individuals, organizations, communities, and society. 

## 2020 March

Relaunching the Value group with the goal of centering on funding community initiatives. Specifically: 

- Aligning to **business value**. Metrics must center on an ability to receive or sustain funding. All other metrics will be archived.
- Organizing files for ease of access, including adding a RESOURCES.md file for those who wish to share external recommendations outside of metrics.
- Structuring the repository and guidelines (like code of conduct linking) based on other working groups.

## 2019 July

This is our first release of CHAOSS value-metrics. In this context "value" refers to economic value, which typically is represented in a numeric/monetary form.

### Stakeholders

Our work centers on corporate projects sponsored by "Open Source Program
Offices" (OSPO).  Within this segment, we focus on two types of stakeholders:

* OSPO Managers *

Profile:
- full-time organization employee 
- coder / product manager / 

Activities:
- outreach to outside developers
- outreach to internal developers
- release coordination
- coordination and reporting with internal management

Key value questions: How can I justify my OSPO budget to corporate managers?

We believe that OSPO will be interested in metrics that supports two claims:
- OSPO can reduce labor costs (labor costs)
- OSPO can reduce the time that it takes to close issues (issue velocity)

* Workers *

Activities:
- find an interesting project 
- learn the community and the tech
- write code and submit a PR
- decide wether to get more invested, or move on
- leverage skills and reputation for economic opportunity

Key value question: How can I make a living wage in open source?

We believe that workers will be interested in metrics that show:
- which projects are backed by corporate money?
- which projects are growing rapidly?
- which projects have an underserved developer community?
- what types of salaries are being paid for specific technical specialties?

### Parametrized Metrics

Many economic values are context-dependant.  

For example, we may wish to measure the $USD value of a closed issue.  The
formula to calculate the $USD value would be something like "number of issues *
average labor hours to close an issue * fully-loaded average hourly labor
rate".

In this context, the number of closed issues is an objective measure.  But the
time-estimate to close issues varies from organization to organization, as does
the hourly labor rate.

To accommodate this context-dependency, we will introduce the idea of
"parameterized value metrics".  

Terms:
- base metric - an observed value like "number of closed issues"
- parameters - like "hourly labor rate" or "hours labor to close issue"
- computed metric - like "cost per closed issue"

The initial implementation of "parameterized value metrics" is brutally simple:
export CSV with base metrics, load CSV into a spreadsheet and apply formulas
with your own context-specific parameters.

