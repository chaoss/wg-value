# Downstream Organizational Impact of a Project Software

**Question:** Which organizations are using this project?

## 1. Description
Organizations engage with open source projects through use and dependencies.
This metric is aimed at determining downstream impact of an open source
project. This metric looks at organizations that deploy a project as part of an
IT infrastructure, other open source projects with declared dependencies, and
reference to the project through social media, conference mentions, blog posts,
and similar activities.

## 2. Objectives
As a developer, I'd like to invest my skills and time in a project that has a
likelihood of getting me a decent paying job in the future. People can use the
Downstream Organizational Impact of a Project Software metric to discover which
projects are used by organizations, and they may, therefore, be able to pursue
job opportunities with, possibly requiring IT support services.

## 3. Formula

Base metrics include:
- Number of issues created by organizations
- Number of pull requests created by organizations
- Number of downstream projects dependendent on the project in question
- Number of blog posts and/or tweets
- Number of open hiring requests
- Number of meetups
- Number of books on Amazon
- Google search trends

## 4. Sample Filter and Visualization

The following visualization demonstrates the number of downstream projects
dependendent on the project in question. While this visualization does not
capture the entirety of the Downstream Organizational Impact of a Project
Software metric, it provides a visual for a portion.

![paper image](https://raw.githubusercontent.com/chaoss/wg-value/master/focus-areas/living-wage/_paper.png)

Other visualizations could include Google search trends (React vs. Angular vs. Vue.js)

https://raw.githubusercontent.com/chaoss/wg-value/master/focus-areas/living-wage/
![Google Trends](https://raw.githubusercontent.com/chaoss/wg-value/master/focus-areas/living-wage/_google_trends.png)

ThoughtWorks publishes a series called 'Tech Radar' that shows the popularity of technologies for their

![TechRadar](https://raw.githubusercontent.com/chaoss/wg-value/master/focus-areas/living-wage/_tech_radar.png)

Tech Radar allows you to drill down on projects to see how the assessment has changed over time.

![Assessment](https://raw.githubusercontent.com/chaoss/wg-value/master/focus-areas/living-wage/_tech_react.png)

StackOverview publishes an annual developer's survey

![StackOverflow](https://raw.githubusercontent.com/chaoss/wg-value/master/focus-areas/living-wage/_stack_overflow.png)

## 5. Reference Implementation

## 6. Known Implementations

1. Augur - for dependencies as an API endpoint
2. Google Trends - for showing search interest over time
3. ThoughtWorks TechRadar - project assessments from a tech consultancy
4. StackOverflow Developer's Survey - annual project rankings

## 7. Examples

1. Available in the Augur test schema for multiple repositories:

- Rails
- ReactJS
- SaltStack

## 8. Resources

- [Open Source Sponsors][l1]
- [Fiscal Sponsors and Open Source][l2]
- [Large Corporate OpenSource Sponsors][l3]
- [Google Trends API][l4]
- [Measuring Open Source Software Impact][l5]
- [ThoughtWorks Tech Radar][l6]
- [Stack Overflow Developer's Survey][l7]

[l1]: https://opensource.org/sponsors

[l2]: https://opensource.com/article/19/1/fiscal-sponsors-open-source

[l3]: https://www.networkworld.com/article/2867020/big-names-like-google-dominate-open-source-funding.html

[l4]: https://www.npmjs.com/package/google-trends-api

[l5]: https://aisel.aisnet.org/cgi/viewcontent.cgi?article=1496&context=amcis2018

[l6]: https://www.thoughtworks.com/radar

[l7]: https://insights.stackoverflow.com/survey/2019#technology
