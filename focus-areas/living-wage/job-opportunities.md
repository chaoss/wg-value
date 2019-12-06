# Job Opportunities

Question: How many job postings request skills with technologies from a project?


## Description

A common way for open source contributors to earn a living wage is to be employed by a company or be a self-employed or freelance developer. Skills in a specific project may improve a job applicant’s prospects of getting a job. The most obvious indicator for demand related to a skill learned in a specific open source project is when that project or its technology is included in job postings.


## Objectives

The metric gives contributors a sense of how much skills learned in a specific open source project are valued by companies.


## Implementation

To obtain this metric on a job search platform (e.g., LinkedIn, Indeed, or Dice), go to the job search and type in the name of the open source project. The number of returned job postings is the metric. Periodically collecting the metric through an API of a job search platform and storing the results allows to see trends.


### Filters

* Age of job posting; postings get stale and may not be removed when filled


### Visualizations

The metric can be extended by looking at:

* Salary ranges for jobs returned
* Level of seniority for jobs returned
* Availability of jobs like on-site or off-site
* Location of job
* Geography


## References

* LinkedIn Job Search API: https://developer.linkedin.com/docs/v1/jobs/job-search-api#
* Indeed Job Search API: https://opensource.indeedeng.io/api-documentation/docs/job-search/ 
* Dice.com Job Search API: http://www.dice.com/external/content/documentation/api.html
* Monster Job Search API: https://partner.monster.com/job-search
* Ziprecruiter API (Requires Partnership): https://www.ziprecruiter.com/zipsearch

_Note:_ This metric is limited to individual projects but engagement in open source can be 
beneficial for other reasons. This metric could be tweaked to look beyond a single project 
and instead use related skills such as programming languages, processes, open source 
experience, or frameworks as search parameters for jobs.
