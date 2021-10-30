# “FEVER” CROWDFUNDING ANALYSIS REPORT

## *Section I: Project Overview*

This project is to help the client Louis figure out how to successfully develop a crowdfunding campaign for her upcoming play “Fever”. She has a $10,000 budget and needs to utilize her resources carefully. Given that she does not have much experience in the area, she has turned to us, SATC Consulting, to assist her fundraising efforts. We believed that if we could analyze enough data from past Kickstarter crowdfunding campaigns (successful, failed, canceled, and live), then we could reasonably uncover factors that contributed to their outcomes. The main focus of this report are the crowdfunding campaigns that relate to theater-based fundraisers and even more specifically, play-based fundraisers. 

## *Section II: Analysis And Challenges*

We gathered data of 4,113 crowdfunding campaigns in the United States and Great Britain. The campaigns were organized into 9 parent categories with 41 subcategories. As previously mentioned, we were specifically interested in crowdfunding campaigns related to the parent category of theater and the subcategory of play. We analyzed play Kickstarter campaigns both within the United States and Great Britain. 

### Subsection A: Analyzing Outcomes Among Parent Categories and Sub-Categories

Our initial analysis included breaking down outcomes by the 9 parent categories and then the 41 sub-categories in the U.S. We wanted to acquire a more general understanding as to the nature of how successful Kickstarter campaigns were based on their campaign types. For instance, since Louis is attempting to raise funds for a play, what is the typical success and fail rates for theater campaigns and then to break it down even further, what are those rates for plays? 

The results of our analysis are presented in **Figures 1-1, 1-2,** and **1-3**:

<img src='images/Parent Category Outcomes.png'>

**Figure 1-1**


<img src='images/Parent Category Success Rates.png'>

**Figure 1-2**

<img src='images/Subcategory Outcomes.png'>

**Figure 1-3**

We can see theaters by far had the most crowdfunding campaigns with 912 out of the 3,038 campaigns in the U.S. (**Figure 1-1**). Upon closer inspection, we can see that the theaters category was one of the more successful campaigns in raising funds. Notice that the “successful” part of the bar is larger than the other nine categories. We went out to calculate the success rate of all nine parent categories in order to obtain a more precise estimate of their success rates (**Figure 1-2**). Theaters finished in the top three categories in this list by having a success rate of 58%, only losing out to music (77%) and film & video (62%). This means that given that plays are within the theater category, Louis has a much greater chance of reaching her fundraising goals than other campaigns. 

Still, we wanted to see what were the outcomes for plays, a subcategory of theaters and more directly related to Louis’ fundraising campaign. As result, we performed another pivot table analysis of outcomes for subcategories and produced the results in **Figure 1-3**. Interestingly, plays consisted of the most crowdfunding activity of any of the other subcategories by far. Indeed, of the 912 theater campaigns, 671 were plays, which is a great sign in terms of making inferences with data since we have such a large set. We proceeded to calculate the success rate for plays to determine if it was indeed close to the success rate for theaters. To our surprise, the success rate for plays was 61%, which was higher than that for its parent category theaters at 57%. This insight should provide Louis with more confidence that she can raise the funds that she needs through crowdsourcing given how successful other plays were in reaching their fundraising goals. 

Now that we understand the general success rates for theater and play crowdfunding campaigns, we wanted to dig deeper and understand why certain theater and play campaigns were successful and other were not. We conducted this analysis in the next subsection.

### Subsection B: Possible Reasons For The Success Rates In Theaters And Play Crowdfunding Campaigns

We performed additional quantitative analysis on the Kickstarter data. Specifically, we focused a majority of our analysis on the plays subcategory of the data. We looked at the plays data from several angels:

- Central tendency statistics.

- A breakdown of the goals for all successful and failed Kickstarter plays.

- An analysis of the timing effects of the launch date on fundraising successfulness for plays.

- Drawing inferences from a sample of Louis’ favorite Great Britain plays that were successful (“Edinburgh data”).

We believe that the areas we covered should provide sufficient justification for our conclusions and recommendations.

### Subsection B.1: Central Tendency Statistics

**Figure 1-4** provides the results of our analysis of the central tendency statistics for the plays Kickstarter data. We broke down the data within the following two categories based on their fundraising outcomes: successful and failed. The metrics we observed were based on the goal and pledge amounts for the crowdfunding campaigns. We provided an additional table below to analyze supplementary metrics that we believed were important for the analysis. Please review **Figure 1-4**.


<img src='images/Central Tendency Measures For U.S. Plays.png'>

**Figure 1-4**

A general theme that we can surmise from the data is that crowdfunding campaigns that are successful do not ask for significant amounts of money whereas those that are unsuccessful tend to ask for substantially more money. What do we mean by substantial? The mean goal for successful group was at $5,049 which was almost half of that of the failed group’s mean goal at $10,554. What was interesting, however, was that although the median goal for successful campaigns at $3,000 was not too far away from the mean, the median goal of $5,000 for unsuccessful campaigns was considerably less than its mean goals. To give context as to why this important, the differences between the medians and means between both sets of data suggests that unsuccessful campaigns have greater variation and potentially even more outliers than successful campaigns. This affects our ability to make inferences from the data. Since the data for successful campaigns is more centralized, then we can make more inferences about it and come up with conclusions that are more applicable to Louis’ fundraising campaign. 

A recommendation that we can make thus far from analyzing the summary statistics is that Louis would be better off breaking up her $10,000 budget into a few smaller fundraisers, specially ones that are around $3,000 (the median of successful ccampaigns) but not more than $5,000 (the mean of successful campaigns). Based on the data, if she tried to raise all of the $10,000 in one sitting (which is around the mean of unsuccessful campaigns), there is a good chance that she will not be able to reach her fundraising goals.

When evaluating each group’s standard deviations of $7,749 for successful campaigns and $21,968 for failed ones, we can see that in general there was considerable variation for both groups but more so for unsuccessful play campaigns than successful ones.

Another interesting insight into the variation of the data is provided by analyzing the quartiles of the goal data between successful and failed campaigns. The upper quartile represents the cutoff for the bottom 75% of the data while the lower quartile represents the threshold for the bottom 25%. For successful campaigns, 75% of the goals data was either less than or equal to $5,000 (which is also the mean of successful play campaigns) and the bottom 25% of the data was less than or equal to $1,500. What this means from an analytical standpoint was that an overwhelming amount of the crowdfunding campaigns that were successful asked for substantially less money than failed fundraisers. This is especially true when you compare these numbers with the upper quartile goal of failed campaigns of $10,000 and the lower quartile of goal campaigns of $2,000 which were both higher than the successful campaign upper and lower quartiles, which further strengthens our argument that Louis needs to break up her $10,000 crowdfunding fundraiser into smaller campaigns.

Let us move on to the pledge data, which represents the actual amounts contributed to plays. As we can see, there is a huge discrepancy between the mean amounts that were pledged in successful play campaigns ($5,602) and those that were allocated in failed play campaigns ($559). This difference shows that there the amount a fundraiser asks in its crowdfunding campaign for plays has a significant impact on funds pledged to it. Compare the mean goal amounts with the mean pledged amounts and you can see that in successful campaigns the amount on average pledged slightly exceeds the average goals, which suggests a high rate of success (over 100%) for these fundraisers. This number drops significantly to less than 6% pledged when the amount sought is $10,000 or above (i.e., for failed play campaigns).

In terms of the variation of pledged play campaigns, we can similar types of dispersion that were in the goals segment for successful play campaigns but not so much for failed play campaigns. This makes sense given that, as previously mentioned, the amounts pledged to play campaigns either met or slightly exceeded the amounts asked for successful play campaigns so naturally the variation between goals and pledged play campaigns would be similar. However, for failed play campaigns, the variation for pledged play campaigns is significantly lower than that of the fundraiser goals group. We ask the reader to compare the standard deviations between the two: $1,331 for pledged campaigns and $21,968 for the goals. Even though the standard deviation is still higher than the mean for the pledged data within the failed play campaigns category, the difference is not as large as it is with the goal play campaigns data. This explanation that we have for this difference and why the pledged data is less variable than the goal data is due to fundraisers having the ability to set all types of fundraising goals, no matter how unrealistic they are, (which would explain the high variability in the goals data for failed play campaigns), but having no control over the amount of money that they receive.

However, the data becomes less variable and more stubborn at the low end for the pledged data for failed play campaigns because plays that were unsuccessful were naturally not going to attract much money. What is the significance of this understanding? The fact that the pledged data for failed play campaigns was more centralized than the goals data suggests that we can make a reasonable inference that if Louis raises money in the upper regions of the goal data ($10,000 or more), she can expect not only to not raise the funds that she needs but to substantially underperform her fundraising goals by raising an average of $559 (the mean of the pledged data for failed play campaigns). So based on the historical data, the results could be disastrous if she asks for too much money. 

Other analyses that we conducted that we thought were of interest to the reader were that length of the campaigns, the average donation size, and the number of backers. Interestingly, the duration for successful play campaigns (29 days) was not that much shorter than failed play campaigns (34 days). You would think that if a play was in great demand and had a high number of backers (successful play campaigns had an average of 56 backers while failed play campaigns had an average of 8 backers), that successful campaigns would easily be able to raise money in a short period of time (Like 14 to 21 days). However, this is not the case. We would need more granular information to understand the reason for this occurrence, which was not provided in the data set. As a result, we can assume that however many Kickstarter campaigns Louis will attempt that each will take around 29 – 34 days, or about a month, regardless if it is successful or unsuccessful. Such information will be important to consider for our full recommendation for the client, which is in the “Results” section of this report. 

One positive indicator is that the average donation size for successful campaigns ($80.74) was nearly twice that of failed campaigns ($47.85), which means that the client Louis can ask for more money individually and try to meet her fundraising goals quickly, but the total amounts asked must be around $3,000 - $3,500 per campaign. 

One limitation of this analysis is that based on the data we have, we do not know all the factors that could be attributed to differences between successful and failed campaigns other than the amounts raised. This is just one dimension that we were able to analyze for possible reasons as to why some play crowdfunding campaigns were able to raise the money that they wanted and others were not. There could be other reasons. The type of play, which is not represented in this data, could be a factor as to the fundraising success rate of the campaign. Dramas might be in more demand than Comedies and so are able to raise more money than that category. We also did not have the ability to do a text-based analysis on the blurbs section of the Kickstarter data to determine if there were certain words or descriptions that made a Kickstarter data more likely to raise the money that it wanted. We do have a brief analysis on this subject within the “Edinburgh Research” subsection of this report, which looks at a small sample of five plays within the data set. However, we cannot make more general inferences from the larger data set because we did not have the tools that we needed to do text-based data mining. As a result, there are limitations in our understanding as to the reasons why certain campaigns were successful and others were not.

### Subsection B.2: Outcomes Based On Goals For Plays

In this section, we breakdown the outcomes based on goals by segmenting the amounts asked for into different ranges. We categorized the data among the projects that were successful, that failed, and that were canceled. Our results are presented in **Figures 1-5** and **1-6**.

<img src='images/Play Outcomes Based On Goals Table.png' data-canonical-src='images/Play Outomes Based On Goals Table.png' width='800' height='450'>

**Figure 1-5**

<img src='images/Outcomes Based On Goals Chart.png'>

**Figure 1-6**

This analysis confirms our recommendation that Louis should break up her fundraising campaign into several smaller Kickstarter fundraisers. Look at **Figure 1-5** and see how high the number of successful campaigns under the “Number Successful” column for the two first ranges of “Less than $1,000” and “$1,000 to $4,999” are considerably much higher than the subsequent categories. Given that the percentage successful for both of these play campaign types were higher that those for most of the other segments, we have even more reason to support our previous conclusion that Louis should break up her $10,000 play campaign into smaller fundraisers. We think that she should seek around $2,500 - $3,500 per fundraiser, maybe even smaller amounts if she can manage it. 

We encourage the reader to look at the percentage success rates for each category in tandem with the number of successful campaigns because looking at the percentages alone (for instance, observe **Figure 1-6** without the context of **Figure 1-5**) can create the false impression that higher dollar amount fundraisers were more successful than they were. Look at the “$35,000 - $39,999” and “$40,000 to $49,999” segments in **Figure 1-5** and **1-6**. If you looked at **Figure 1-6** alone, you would think that there is a good chance that a campaign would be successful if their goals were within these ranges. However, with the inclusion of **Figure 1-5**, you can see that the percentages only represent a small sample of campaigns: eleven in total for the "$35,000 - $39,000" category and six in total for the "$40,000 - $49,999" cateogry. These small numbers do not provide us with a lot of confidence that we could raise $35,000 or $49,999 successfully in a Kickstarter play campaign. The fact that the lower threshold categories (specifically the “Less than $1,000” and “$1,000 to $4,999” segments) have both high success rates and high sample sizes suggests that the trends within these data sets is stronger than those in the higher amount categories.

### Subsection B.3: The Effects Of The Launch Date On Play Kickstarter Campaigns

We compared the outcomes for play and theater Kickstarter categories based on their launch dates for all years under consideration (i.e., from 2009 – 2017). We wanted to see if there were any trends for successful and failed fundraising campaigns during certain times of the year. The results of our analysis are presented in **Figures 1-7** and **1-8**. 

<img src='images/Outcomes Based On Launch Date.png'>

**Figure 1-7**

<img src='images/Play Outcomes Based On Launch Date.png'>

**Figure 1-8**

**Figure 1-7** represents the parent category theaters’ outcomes based on the campaigns’ launch dates while **Figure 1-8** represents the outcomes based on launch date for the play subcategory, which is a category within theaters. Notice that both charts follow a similar pattern where the number of successful campaigns increase from March to May and then significantly decline from May to September and even decline more for the month of December. Given that plays represent about 61% of all the data within the theater parent category, we would expect that both charts would exhibit similar patterns. As a result, of Louis wanting to raise money for her own play and not pursue other activities that are represented within the theater categories, we are going to focus more on **Figure 1-8** for the remainder of this section. 

Due to a majority of successful Kickstarter play campaigns taking place during the late part of the spring and most of the summer, we recommend that Louis run the 3 – 4 Kickstarter campaigns that we recommend between the months of April and August. Since successful Kickstarter play campaigns take about 29 days to reach their goals (see **Figure 1-4** for more details) and given that we have recommended Louis to break up her fundraising campaign from a single $10,000 fundraiser to smaller blocks of three to four campaigns ranging from $2,500 to $3,500 each, we suggest that she plan to run at least one Kickstarter play campaign per month for the five-month window that we recommend. This would mean that she has some flexibility in organizing her campaigns and might even be able to get away with running two campaigns at once in May since that is the peak time for plays to receive funding.

### Subsection B.4: Edinburgh Research

The last piece of analysis that we conducted consisted of analyzing five plays that Louis attended to while she was in Great Britain. Her impressions of these five plays were very positive and so she asked us to provide a brief analysis on them to determine if there were factors that contributed to their fundraising success. We created a table that is provided in this report in **Figure 1-9**.

<img src='images/Edinburgh Research.png' data-canonical-src='images/Edinburgh Research.png' width='650' height='450'>

**Figure 1-9**

One of the biggest items that stood out to us was that the fundraising goals for each of these five plays was $4,000 or less. The fact that what was pledged to each of these campaigns was either matched or exceeded by a marginal amount coincides with the general trend that we have seen from other Kickstarter play campaigns within the data set: smaller fundraisers were more successful in raising money than larger ones. As a result, Louis should be even more comfortable with the part of our recommendation recommending that she break up her $10,000 budget into smaller fundraising campaigns since the plays that she personally liked raised small amounts as well.

Another factor that we could attribute to the success of these five plays was that there were a significant number of backers for each campaign. If you recall in **Figure 1-4**, the average number of backers for successful campaigns was around 56. From this small sample, we can see that the average number of backers for these five campaigns was similar with 62 backers. As a result, Louis should have a better idea as to the number of people that she needs to reach out to in order for her fundraising campaign to be successful.

One thing that was interesting was that the average donation size for all five campaigns in this sample were around $40 per fundraiser. This is significantly smaller than the $80.74 donation size that we saw for successful play campaigns within the larger 671 play Kickstarter space. To account for this discrepancy, and to err on the side of caution, we recommend that Louis start off her first campaign around asking for $35 - $40 per donation from potential backers in her first campaign and then see if she can increase these amounts in subsequent fundraisers. 

Finally, we try to assess qualitatively if there was anything in the blurbs that could help us understand why these five campaigns were successful in their fundraising efforts. The only conclusion that we could draw from this sample was that in four out of the five blurbs, there are names mentioned about actors or writers who are part of the plays. This must mean then that the people mentioned in these blurbs must have credible name recognition that would attract audience members to those performances. Therefore, we recommend that when Louis writes up the blurbs for her campaigns that mentions any noteworthy actors, writers, or authors that are somehow involved in her play in order to attract more funding from investors. 

## *Section III: Results*

Although we briefly mentioned parts of our recommendation to the client throughout our report, we will discuss our suggestion in its entirety in this section. **After careful review and analysis of the data presented, we recommend that the client Louis break up her $10,000 budget into 3 – 4 separate fundraising campaigns within the range of $2,500 to $3,500 per fundraiser. We highly suggest from refraining from raising more than $5,000 in a single campaign as that will significantly reduce her odds of acquiring the money that she needs to fund her play. We also recommend that she run her campaigns during the months of April – August during any calendar year since those months typically see the best results of fundraising for play campaigns. Since Kickstarter play campaigns that are successful in reaching their fundraising goals have a duration of less than 30 days, we suggest that Louis run one Kickstarter campaign per month during the recommended time frame. Indeed, when reaching out to individual donors or enlisting a donation size per person on her Kickstarter play campaign, we recommend that Louis asks initially for $35 - $40 in her first one or two campaigns and then gradually increase the donation size thereafter but not more than $80 per person. The data suggests that she should expect around 56 people to back her play campaign if it is successful. This means if she was to go out and enlist backers, then this is the number of people she should reach out to. Finally, we believe that in the blurbs that Louis writes out to solicit funds in her campaigns that she includes the names of noteworthy, actors, authors, or writers within her play so that investors will be even more encouraged to send money her way due to the likelihood that audience members will be attracted to performances by well-known individuals. We believe that the parameters set forth will give Louis the best chance in raising the $10,000 that she needs for her play.**

There are limitations of course to both our recommendations and analysis. We first assume that Louis’ play “Fever” is a quality play and is one that is in-demand. These two factors alone will dominate any of the other contributors that we have identified in the analysis as to the successfulness of a Kickstarter campaign for her play. If audience members do not like the type of play she is offering, it is of poor quality, or they do not recognize any of the actors and are therefore unlikely to attend the performance, then her campaign will most certainly not be successful not matter how hard we try to emulate the contributing factors of other plays in their Kickstarter campaigns. 

In addition, with the data given, we had no way of analyzing qualitatively (which as we established before, might be more helpful than the quantitative analysis that we did) why some of the 671 plays in our sample were successful and why some were not. If some of the data had play types like drama, comedy, romantic, etc., then that could have provided further insights as into the likelihood of Louis successfully raising money for her play. More importantly, it could have provided additional insights as to what she would need to do given the type category her play fell into. For instance, say that comedies have a mean goals and pledges of $3,000 each but the numbers for dramas are $2,000 each. If Louis’ play “Fever” is a drama and she still needs $10,000, then it does her no good to utilize two $3,000 campaigns and one $4,000 campaign to back her budget. This is due to history telling us that instead she needs to utilize five $2,000 campaigns since investors typically do not have the appetite to donate more money for dramas.

These are some of the shortcomings in regards to the Kickstarter play data that we identified. We are certain that there are others. However, we believe that the quantitative analysis that we were able to do provides enough of a framework to help Louis successfully plan her fundraising efforts.




