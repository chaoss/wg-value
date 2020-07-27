# Comments on Social Currency Metrics System:
## Purpose
Line 9: "SCMS is a combination of [social listening](https://blog.hubspot.com/service/social-listening) practices across multiple channels along with a meaningful set of categorizations. The combination of these tactics can lead to systematic community analysis and can inform a community strategy that leads to measurable business value."

Comment: The purpose of CHAOSS metrics historically is to create standard, atomic definitions that can be used reliably across projects to support comparisons. Meaningful categorizations at the metric level should be common across open source projects. To accomplish this, standardized data will need to be shared. 

This comment does include two distinct items to consider. First, what is the collection of atomic metrics. I think they can be defined post-release, but should be enumerated clearly in the synthetic metric prior to release. Second, the synthetic metric implies both standardized measures and standardized categorizations. I think the standardized categorizations need to be referenced and shared, along with a collection of examples of that standardization sufficient for users of the metric to train people to implement the categorizations consistently. 

## Specificity
Reference: Lines 11-15
"**Theory and Origin**

Social currency or Social Capital is a social scientific theory. It broadly considers how human interactions build relationships and trust in a community. The Social Currency Metric System represents the reputation of a community as measured via community trust, transparency, utility, consistency, and merit.

Interpersonal relationships are the social fabric of communities. This is shown in the [Levinger’s Relationship Model](https://theadminzone.com/ams/levingers-stage-theory.1272/) and [Social Penetration Theory](https://psycnet.apa.org/record/1973-28661-000). Community members' sense of personal and group identity grows as they interact. Members build shared values, accumulate a sense of trust, encourage cooperation, and garner reciprocity through acts of [self-disclosure](https://en.wikipedia.org/wiki/Self-disclosure). These interactions build an increased and measurable sense of connection. The measure of these characteristics is called social currency."

Comment: Are these the atomic metrics that will be developed for the next release?: 
1. community trust, 
2. transparency, 
3. utility, 
4. consistency, and 
5. merit

## Sentiment
Reference: Lines 22-24
**Objectives**

Analyze the qualitative comments in community interactions. Gain an overview of sentiment in a community. Get metrics that show at a glance how a community is and was doing. Use lead metrics from continuous measurements for proactive community strategy development. Instill trust in community members that their thoughts and opinions are valued.

Comment: "An overview of sentiment" seems somewhat incongruent and oversimplified in the context of what I think are the five main atomic metrics that need to be developed: 
1. community trust, 
2. transparency, 
3. utility, 
4. consistency, and 
5. merit

It also seems that "Instill trust in community members that their thoughts and opinions are valued" is a sixth atomic metric that will define a process, and perhaps not be measurable via trace data. 

## Implementation
Reference: Lines 27-51 (Comments inline)

**Implementation" 

The SCMS requires the collection of community comments (communication traces), the definition of a codex, and the on-going review of the communication traces.

**COMMENT: If the codex is an essential part of the metric, a standard codex should be defined, referenced, and continuously updated as part of the metric. I think this should be more than a "toy example", but something sufficient enough for individuals who want to use this metric and draw comparisons across communities to do so in a standardized way. Does the codex include each of the six atomic metrics I think are implied by the definition to this point? **

Set up a Data Collection Platform of your choice as described in the “Tools” section below. Ensure it has a minimum of 4 dimensions and 3 communication channels. Once it is set up, the following method is used to collect, analyze, and interpret results:

![Social Currency Metric System process as a circle](images/scms-0-circle2.png)

1. **Collect Communication Traces** --
 Identify online platforms that your community is communicating on. Set up data funnels from the primary platform to your SCMS tool. The critical data for the system is user generated content.

**COMMENT: There are a finite set of communication trace origins that are common across open source projects. Those should be enumerated here, and where applicable, existing atomic metrics that can be used to describe the data might be referenced. For example, issues and issue comments, pull requests and pull request comments, etc.**

2. **Standardize How Communication Traces Should Be Assessed** --
 Use a codex to define important concepts as a “tracking keyword” or “category” in the focal community. This unified codex of terms ensures consistent analysis as different people read and tag community sentiment. Formalizing the revision and addition structure to this codex on a regular basis is a must.

**COMMENT: One of the aims of the CHAOSS community is the specification of standard metric definitions. Each community may have a "specialized" codex, but given the identifiable atomic metrics in this definition, this seems like a standardizable data set that should be included in the repository in support of SCMS being a standardized metric**

3. **Analyze the Communication Traces** --
 Community sentiment is analyzed in the SCMS tool by tagging data with codex terms. If the tagging is done by a team of people, it is recommended that everyone gets together regularly to discuss trends and ensure consistent tag use. If the tagging is done by an artificial intelligence algorithm, then a human team should supervise and retrain the AI as necessary.

**COMMENT: Given that there is an achievable general codex for open source software, it also seems reasonable, given the nature of the atomic metrics, that a standardized set of tagged examples is also required here, with sufficient detail for the metric to be implemented consistently** 

**COMMENT: The definition of tags suggests supervised machine learning, not unsupervised machine learning (often referred to as "AI" these days.). If there are two things going on here they should be clarified**

4. **Share and Visualize the Aggregated Analysis** --
 Visualize the quantitative count of codex terms over time, e.g., in a dashboard. This is where the qualitative analysis results produce an easy to observe dashboard of trends. Share analysis with team members.

**COMMENT: Visualizations are generally provided in CHAOSS metric definitions as examples. In this context, I think the synthetic metric is defining a process component, which is distinct from the data gathering components. It seems like it should be under the "example visualizations" section of the standard metrics template.**

5. **Benchmark, Set Goals & Predict Future Growth** --
 After getting enough data to form a benchmark, take stock of where your community stands. What are its strengths and weaknesses? What actions can be taken to make the community healthier and more robust? Then form community initiatives with well-defined goals and execute on these projects to affect the social currency metrics for next week.

**COMMENT: I would break this out into a separate metric that focuses on process. Here the definition is defined by a process, whereas much of the rest of the metric is defined by standardized definitions of data that describe what I think are six atomic metrics. Perhaps describe this here, but reference a fuller definition to a seventh atomic metric.** 

6. **Repeat the Process** --
 In regular evaluation meetings, discuss the shortcomings of the dataset or collection methods. Come up with methods to address these shortcomings in the future. Work solutions into the system and move forward. Truth is in the trend, power is in the pattern.

**COMMENT: This seems like a constituent part of the second synthetic metric I suggest for item five. It is the application of the data.  I could also argue that items five and six may be more along the lines of best practice recommendations than they are metrics. They reflect general practices common across metrics deployments, and are therefore conceptually really not "standarizable metrics".  I can see how they could be reframed in this fashion using some of the examples from the D&I working group, though.**

## Standardized Source Data Structure
Reference: Lines 83-97 (Comments Inline)
"### Tools Providing the Metric

To implement the metric any MySQL, smart-sheet, excel, or airtable-like excel datasheet program works fine. This data should be simplified enough to interact with other data interfaces to ensure that data migration is simple, straightforward, and can be automated (such as google data studio). This requires that systems used to implement the SCMS work with CSV and other spreadsheet files, and we heavily recommend open source programs for its implementation.

**COMMENT: I think enumerated a partial list of potential physical storage strategies is unnecessary in a metric definition, and to date we have not included them. This kind of recommendation is also likely to quickly become dated and require frequent updating**

Once you have this, create a data set with the following data points:

| Data Points | Description |
|---|---|
| Date of entry| Date data was imported to SCMS tool|
| Date of comment| Date comment was made on original platform|
| Comment Text| Qualitative data brought in. Decide on how large you want these chunks ported. Some may port an entire email while others will be broken into one row per sentence. It should only have one “sentiment”|
| Data channel| Originating data channel the comment came from |
| Tags (created on codex document below) | Based on the unified codex of terms, decide what tags to track. There can be two kinds of tags. On the one hand, tags can be based on “themes” or recurring sentiment that people voice (e.g., gamer gate, flamewar, or thank you notes). On the other hand, tags based on “categories” can describe different aspects of a community that members comment on (e.g., events, release, or governance). |
| Social Currency Metric| The social currency being awarded or demerited in the system. This will directly affect numbers.|
| Weighted Score | Once you’ve decided what your “weight” will be, you can assign a system of -3 to +3 to provide a weighted view of human-tagged metrics (AI will not assign a weight for several reasons). This enables the “most impactful comment” filter.|"

**COMMENT: This standard dataset definition seems like what needs to be included as a reference in other parts of the metric. Defining the metadata like this gives structure to reference data. The tricky part, here again, is for this to be a metric that can have standard implementations, the inclusion of references to data files that follow this structure in the repository seems essential.**

**COMMENT: I've mentioned this elsewhere, but the reference to "AI" here is a bit hand wavy, and the entire process sounds like supervised machine learning, not unsupervised machine learning** 

## Process Definition II
Reference Lines: 99-116 (Comments Inline)

"Create a second sheet for the Unified Codex of Terms which will define terms. It should look like this:

**COMMENT: At a fundamental level I think a significant percentage of tags arising from categories (themes is a new thing here and should be distinguished from categories) will be common across open source projects. Especially of the type likely to have sufficient visibility and "girth" to offset the cost of this kind of synthetic metric's production. There are surely, again, specialized tags for different types of open source, but for the projects of sufficient girth to invest in tracking SCMS, I suspect the overlap to be substantial, and those standardized tags and example coded data to be essential for this to ultimately exist as a CHAOSS metric. Without that, I think it fails the "standardized metric" test.**

| Category Term | Definition | When to use | When not to use |
|---|---|---|---|
| [Custom Tags - themes and categories] | | | |
| [Community specific jargon]| | | |
| Social Currency Dimensions:| | | |
| TRANSPARENCY | Do people recognize and feel a connection to your community?  |When they have the "words" to pinpoint why they feel you are authentic or personalble.|This is not about good customer service, or doing well.  That is utility.  This is about whether they understand who you are as a business and show they are onboard with it.|
| UTILITY | Is your community doing something useful or is it contributing value? |Provide parameters that exclude when the term is used so that people know when the category tag should not be implemented.|This is not about good customer service, or doing well.  That is utility.  This is about whether they understand who you are as a business and show they are onboard with it.|
| CONSISTENCY | Do you have a history of being reliable and dependable?  |When they suggest they have used your brand, or interacted with you several times |If they've only provided their comment to suggest you were useful once, use utility instead.|
| MERIT | Does your community merit respect and attention for your accomplishments? |When the social currency garnered from customers seems it will continue for a while, and will impact other people's opinions.|When they suggest they will use you again in the future use trust instead as that is a personal trust in the brand. Merit is external.|
| TRUST | Can people trust that your community will continue to provide value and grow in the future? |When they suggest they trust you well enough to continue conversations with you in the future|When there is not substantial enough evidence to suggest they will continue to work with and trust you as a loyal customer or community member.|
| INTERNAL REPUTATION | Do people believe these things strongly enough to warrant conversation or action? | | |
| EXTERNAL REPUTATION | What amount of your reputation in your community is transferable to strangers outside of your community (cold audiences)? | | |

**COMMENT: This table provides initial definitions for five of the seven atomic metrics I've culled from this definition. I suggest this section be a reference to those atomic metrics, so they are more fully fleshed out.

There are also two "new things" here, which are probably atomic metrics eight and nine: Internal reputation and external reputation. The definitions as they exist are too vague to operationalize.**

The codex is filled in by stakeholders on a regular basis by specific communities and forms the basis for analysis of the data. This is the MOST IMPORTANT part. Without this the subjectivity of qualitative data does not follow the rule of generalization:

“A concept applies to B population ONLY SO FAR AS C limitation.” "

**COMMENT: I am intuiting from the surrounding text that the "codex" is the continuous application of the tags, derived from categories, to new conversational data with the aim of continuously improving the supervised machine learning algorithms used against some larger collection of data to generate the values for the atomic metrics that are quantifiable from trace data, and then weighted by the community to arrive at the SCMS score. Perhaps this is a tenth atomic metric along the lines of "social currency trajectory", or perhaps it is a mechanism for maintaining the non-specialized coded data.  Its not clear.**

