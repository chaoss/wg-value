# Contributor Recommendability

Question: How likely is it that you would recommend a community or project to other people? 

## Description
The contributor recommendability metric seeks to understand two components of community engagement. First, the metric helps you know how happy people are with their participation in a particular community or project. Second, the metric enables you to know how much your community members are willing to promote (or detract from) participation in a particular community or project. 

## Objectives
1. To evaluate the contributors’ satisfaction with a community or project.
2. To determine reasons contributors would leave your community or project and even discourage others from joining.

Using feedback from members, the community would set up a process to improve itself through the cultivation of community members who indicate they would recommend or not recommend a community or project. 

The contributor recomendability metric can identify areas of an open source project where contributors are dissatisfied or leaving. This metric could indicate underlying diversity, equity, and inclusion concerns that may be present in a project. 

Additionally, the contributor recommendability metric can be used to develop contributor net recommendabilty. The following provides a way to consider contributor net  recommendability. 



1. Individuals who provide low, moderate, or high individual scores on this metric are categorized along a continuum from Detractor, to Passive, and, finally, to Promoter through segmentation using a statistical answer distribution determined to be appropriate for the project (e.g., Figure 1). 
2. The percentage of promoters can be subtracted from the percentage of promoters to produce a measure of net recommendability.

---

`![recommendability-scale](https://github.com/chaoss/wg-value/focus-area/communal-value/images/contributor-recommendability_recommendability-scale.png)`


Figure 1: An example of one mapping between a 10-point likert scale and categorization of contributors. 

%Detractors-%Promoters = **Net Recommendability**

---
Net recommendability is inspired by the [Net Promoter Score](https://www.surveymonkey.com/mp/net-promoter-score-definition-formula/).

## Implementation

__The usage and dissemination of health metrics may lead to privacy violations or expose organizations to risk. These risks may flow from compliance with the GDPR in the EU, with state law in the US, or with other laws. There may also be contractual risks flowing from terms of service for data providers such as GitHub and GitLab. The usage of metrics must be examined for risk and potential data ethics problems. Please see [CHAOSS Data Ethics document](To be added within the month) for additional guidance__

### Filters 
By location of engagement. For example, by asking from:


* Code committer 
* Issue reporters
* Issue responders
* Reviewers (e.g., in change requests)
* Event participants
* Release cycle managers
* Community members (e.g., committers, maintainers, board members)
* Demographic segments of respondents
* Length of time in the community, or time since the first contribution
* Activity type (e.g., new contributors, core, regular, casual, episodic)

### Data Collection Strategies 
Implicit Data: 



* Community newcomer inclusion factors, such as responsiveness to issues and change requests. 
* Community health factors like change request acceptance rate and release cadence. 

Explicit Data: 



* Surveys focused on obtaining contributor perspectives on different communities and contributors. Sample questions include: 
    * Could you specify where you primarily contribute to the community/project? 
    * What aspects of this project do you find exceptionally motivating?
    * What aspects of this project do you want to see improved in the future?
    * (optional) Please share your GitHub ID or email address if you wish to help us build some context around your answers as associated with your issues or change requests. This data will not be available to project maintainers or others in the project.
    * How likely is it that you would recommend this community/project to other people? (Likert scale 0-x scores)
        * Not at all likely
        * Neutral
        * Extremely Likely
          * As a result of “Not at all likely”: Why do you not recommend the community to your friends or colleagues?
          * As a result of “Neutral”: Is there anything we can improve?
          * As a result of “Extremely likely”: Which part of work or areas do you recommend the community to your friends or colleagues?

## References
* [Net Promoter Score Definition and Formula](https://www.surveymonkey.com/mp/net-promoter-score-definition-formula/)
* https://www.ipsos.com/en-us/net-promoter-debate
* https://www.ipsos.com/en/ipsos-encyclopedia-net-promoter-score-nps 

## Contributors
* Yehui Wang 
* Matt Germonprez 
* Sean Goggins 
* Vinod Ahuja 
* Benjamin Mako Hill
* Elizabeth Barron 
