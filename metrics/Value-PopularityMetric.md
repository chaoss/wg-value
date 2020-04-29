# Project Popularity & Living Wage

Question: How can we quantify the earnings potiential of a project, based on its popularity, that will signal the possibility of earning a living wage by contributing to the project?

## Description

One of the main issues with obtaining contributors or keeping them active on open source projects is the lack of funding. The old saying, "time is money" is very accurate. Nobody will continue contributing significant portions of their time without compensation, unless they have a real passion for the project(s). A developer being able to expand their skillset would make them more attractive to employers. If that skillset is at the forefront of some new process or technology, contributions to those projects could provide a living wage for many years to come.

## Objectives

The metric will give contributors a look at multiple project popularities that can highlight specific technologies or processes that would become useful to earn a living wage.

## Implementation

Project popularity will be determined based on a number of factors:  
* Number of contributors  
* Forks  
* Aggregation of online discussion
* Factors from BOSS Index:  
	* Google score  
	* Job postings    

Using past successful projects as a baseline, differing weight values will be attributed to the factors of this metric to provide the most accurate portrait of project popularity.

These projects would include: Kubernetes, Flutter, React, and Tensorflow among others. These projects seem to have been able to grow into modern technology solutions and proficiency in these applications will no doubt be seen as lucrative to potential employers. 

Augur currently tracks many different metrics that span periods of time. By visualizing the different factors listed above with these metrics over the period of time of their infancy to evolution you can correlate data points that support which factors will matter more than others as to the eventual adoption and potential success of a project.

Once that corellation is obtained, you can apply the weighted factors to newer OSS projects to have a better look at which projects will be potentially influential in the coming months/years. 

### Filters  
* Projects that have a TBD number upswing in forks of their repo
* Projects that are trending updwards in their growth percentage of contributors over a TBD window of time
* Projects that have a TBD percentange of mentions through aggregation of online sites
* Projects that have a upswing in their Google Score by a TBD size


### Visualizations 

<img src="images/popularity-bar-graph.png">
![Bar Graph Showing Popularity Matrix](images/popularity-bar-graph.png)


### Tools Providing the Metric (optional)  




### Data Collection Strategies (Optional)  
* 
* (I know this will be removed, wanted to add a talking point) Make a coordinated effort within CHAOSS to present a feature request to GitHub. If projects had "feature request" functionality, instead of treating everything as an 'issue', many different CHAOSS metrics would be able to utilize that data. Instead of a few different people submitting a request to GitHub, make it a concerted effort and present a formal paper with explaination and examples of how that data could only improve OSS metrics, thus their health, which only supports GitHub in the longer term. The text entry portion of the GitHub contact page, doesn't seem to have a word limit, or send using industry contacts.



## References  

* Examine the pay for different skillsets [Salary by skill](http://payscale.com/research/US/Job=Software_Engineer/Skill)
* Explaination of the [BOSS Index](http://battery.com/powered/boss-index-tracking-explosive-growth-open-source-software/)
* Top 10 most popular OSS projects on Github [Top 10](http://insights.dice.com/2019/11/08/10-popular-open-source-projects-github)