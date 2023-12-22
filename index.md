---
    feature_text: |
        ## The Road to Adminship
        <div style="color: white;font-style: italic;">A Guide for Aspiring Wikipedia Administrators</div>
    feature_image: "image_0.jpeg"
---

> Welcome to the realm of Wikipedia where information flows seamlessly and knowledge is at your fingertips.

Since its creation in 2001, Wikipedia stands as a testament to collective knowledge that transcends geographical and linguistic boundaries. This collaborative online encyclopedia has become a cornerstone of information access for billions worldwide. With millions of articles available in numerous languages, Wikipedia remains a primary gateway to knowledge, facilitating learning and understanding on an unprecedented scale. 

This expansive platform owes much of its success to the dedicated administrators who form the backbone of its operation. These committed volunteers play a pivotal role in fostering a collaborative and high-quality environment. Administrators are entrusted with crucial responsibilities, including maintaining content standards, resolving disputes, and safeguarding the encyclopedia from vandalism, copyright problems and misinformation. 

Now dear reader, if you find yourself drawn to the idea of contributing at a more impactful level within the Wikipedia community, you might be contemplating taking the step towards becoming a Wikipedia administrator. 

First, you should know that there are no official prerequisites; any registered user can request administrator privileges. However, you are expected to be active, experienced, and trusted members of the community. So if you are interested, you can easily apply for Wikipedia administrator status by submitting a request for adminship (RfA). Subsequently, any Wikipedia member may cast a supporting, neutral, or opposing vote for you. 

As you embark on this journey, it's essential to understand the intricacies of the election process and equip yourself with valuable insights to enhance your candidacy. In the following sections, we'll guide you through the adminship election process, offering tips and advice to help you navigate the path toward becoming an esteemed Wikipedia administrator.

### Let’s uncover General Trends of Elections
The dataset captures a decade-long snapshot of Wikipedia's Request for Adminship (RFA) elections, from 2003 to May 2013. By examining the details of these elections, we may uncover some patterns that can offer valuable insights. Therefore, before providing you with some useful tips for a successful election, let's first analyze the general trends of the elections. While doing so, we will try to answer several important questions, providing a comprehensive understanding of the landscape.

##### How has the amount of elections changed over time? Are there consistent trends in the distribution of won and lost elections across different years?

<iframe src="https://chart-studio.plotly.com/~iradukun/126.embed" width="800" height="500" frameborder="0" scrolling="no"></iframe>
The variation in the number of candidates each year, forming a normal distribution with a peak around 2006 and 2007, could potentially be influenced by the expansion of Wikipedia. It's worth considering that  in those particular years, there might have been increased awareness and participation in elections, leading to a surge in the number of candidates documented on Wikipedia. 

To make it easier to compare between won and lost elections amounts, let’s plot a yearly pie-chart of their corresponding percentages from 2003 to 2013.

<iframe src="https://chart-studio.plotly.com/~iradukun/38.embed" width="800" height="500" frameborder="0" scrolling="no"></iframe>
Examining the chart reveals that the early years of the wiki-RfA process, up to 2005, boasted a notably high acceptance rate—hitting 100% and 80.3% for 2003 and 2004, respectively. However, starting from 2006, coinciding with the growing number of candidates mentioned in the paragraph above, the acceptance rate began to drop drastically, reaching a mere 30% in 2012.
It's crucial to note that the data for 2013 only covers up to May, making the acceptance rate for this year less representative of the overall scenario.
With an average acceptance rate of 38% from 2006 to 2012, it's evident that adminship has become highly selective. So, remember the saying: many are called, but few are chosen. Getting that admin badge won't be a walk in the park; preparation is key to standing out as a strong candidate. Are you up for the challenge?

##### What is the Average Number of Votes Received in Wikipedia RFA Elections Over the Years ?
By examining the trend of the average number of votes per election over the years, you can gain insight into the anticipated vote count you might receive in the future during the voting process.

<iframe src="https://chart-studio.plotly.com/~iradukun/22.embed" width="800" height="500" frameborder="0" scrolling="no"></iframe>
You might think that every election generates the same interest in the Wikipedia community, but it turns out that voter interest varies significantly across elections. In fact, excluding the year 2013, which has the lowest number of elections recorded in our dataset and is not the most representative, 25% of the elections in a given year have fewer than 20 voters participating. Some elections even have only one voter.

It's important to note that, according to the data we found on [the Guide to Requests for Adminship](https://en.wikipedia.org/wiki/Wikipedia:Guide_to_requests_for_adminship#Closure) in the closure section, the page  states that a bureaucrat will close the RfA as soon as it is feasible. This could be hours or even a day or two after the formal closing date. Additionally, our research indicates that several candidates withdraw their own candidacy shortly after the beginning of the election. But don't let that worry you; every year, there are a few outlier candidates who generate above and beyond interest. In one election, for the candidate 'TenPoundHammer,' an outstanding number of 561 votes were recorded.

##### Who votes? How does the nature of the voting populations evolve?
The answer to this question is pretty straightforward: any Wikipedia member can give a supporting, neutral, or opposing vote. But let's dig a bit deeper. Can we figure out who might cast their vote for your election? That is, of course, if you decide to throw your hat in the ring after going through our guide.

{% include figure.html image="./voters_heatmap.png" %}

The heatmap reads as follow, for any pair of years 𝑦<sub>i</sub>, 𝑦<sub>j</sub>, the value in the 𝑖-th row and 𝑗-th column represents the percentage of voters in year 𝑖 who also voted in year 𝑗. We can see that, over the last six years, on average, 52.68% of voters in a given year continue to vote in the following year, and about 40.46% still cast votes two years later.  Understanding the voting patterns can be a strategic advantage. If you succeed in convincing voters from the previous year and even those from two years prior, you already have a good chance of success.

### Let’s provide you with some useful tips 
##### How many votes should you get to win?
As you can see in the figure above, the number of voters in a specific election can vary quite a bit. If you're aiming for a successful election, you might be curious about how the distribution of votes differs between won and lost elections. Join us in the paragraph below, and let's uncover the answer together.
<iframe src="https://chart-studio.plotly.com/~iradukun/150.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>
Upon examining the boxplot, a disparity in the distribution of total votes between successful and unsuccessful elections becomes evident. The median for unsuccessful elections is approximately 20%, while for successful elections, it is 59%. This suggests a tendency for unsuccessful elections to garner a lower total vote count. Now, do these results hold significant differences? Absolutely. We conduct a statistical t-test, leading us to confidently reject the null hypothesis. Thus, it appears that the total number of votes may indeed play a role in determining election outcomes.

You might be wondering why we used the term "may" in attributing a role to total votes. The reason is that, at this point, we cannot be entirely certain. Correlation does not imply causation, and various confounding factors undoubtedly impact the results. To try to isolate the effect of the total number of votes, we conduct a paired matching, accounting for the percentage of positive and negative votes as confounders. In this case, the treatment involves receiving a number of votes above the average, which stands at 50.4.
<iframe src="https://chart-studio.plotly.com/~iradukun/156.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>
The proportions of elections won and lost in the control group are fairly balanced (49% won and 51% lost). In contrast, a substantial disparity emerges in the treated group—those with an above-average number of votes—where 69% are won and 31% are lost. Therefore, if at the end of your election, you notice you had a high number of voters, you definitely have higher chances to see your candidacy accepted.

##### So, a lot of voters…But, what percentage of positive votes to secure an adminship position?

Of course, the type of votes you receive plays a crucial role. [The Wikipedia guide for Requests for Adminship (RfA)](https://en.wikipedia.org/wiki/Wikipedia:Requests_for_adminship#Discussion,_decision,_and_closing_procedures) states that achieving 75% or more positive votes is essential for passing. However, success in RfA goes beyond accumulating positive votes. The final decision rests with the bureaucrats, who evaluate factors beyond mere percentages. They consider the quality of arguments from voters, the strength of comments in the "Neutral" section, and discount any votes deemed invalid.
<iframe src="https://chart-studio.plotly.com/~iradukun/162.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>
You can notice that there are some exceptions that have a very high positive vote percentage, yet end up not being elected, and vice-versa. Which echoes the fact that a certain percentage of votes is not a guarantee of a successful election. Indeed, there are even cases where candidates were rejected even if 100% of the votes they received were positive. But, you should note that for the majority of these elections, either the candidate refused the nomination, or the election was withdrawn by a bureaucrat who deemed the candidate unprepared. Thus, the percentage of positive votes remains at 100% due to the sudden end of the election but the recorded outcome is unsuccessful. 
It's also worth noting that, for the majority of cases, having less than 50% positive votes appears to guarantee election failure. Additionally, only 6.66% of candidates who fall short of the indicative threshold of 75% positive votes manage successful elections. Keep these thresholds in mind as you gather a substantial number of positive votes to enhance your chances of election success.
<iframe src="https://chart-studio.plotly.com/~iradukun/204.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>

##### Do neutral votes matter?

As mentioned before, neutral votes play a pivotal role in cases of indecision, as they are considered by bureaucrats during the evaluation process. Besides,  our analysis has revealed that a positive vote threshold of 75% tends to yield more favorable outcomes.  So, the presence of a substantial number of neutral votes may influence the outcome of your election. 
<iframe src="https://chart-studio.plotly.com/~iradukun/178.embed" width="800" height="500" frameborder="0" scrolling="no"></iframe>

You might initially dismiss the potential impact of neutral votes, given that they constitute only 6.4% of the overall voting history in our dataset. However, a closer examination reveals that this seemingly negligible percentage harbors an uneven distribution across successful and unsuccessful elections. 
<iframe src="https://chart-studio.plotly.com/~iradukun/185.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>
Notably, the median proportion of neutral votes in unsuccessful elections stands at approximately 10%, a significant contrast to the 1% observed in successful elections. This indicates a tendency for unsuccessful elections to have a higher proportion of neutral votes.To attest to the significance of this discrepancy, we conduct a t-test to compare the distribution of neutral percentages between won and lost elections. With a p-value of 9.77e-198, the statistical test allows us to reject the null hypothesis, indicating that neutral votes may indeed play a role in election outcomes.
However, we cannot conclude the analysis here, as the outcome depends on various factors, and the current analysis doesn't permit us to isolate the effect of the percentage of neutral votes. Therefore, we perform an exact one-to-one matching, considering the total number of votes and the percentage of positive votes as confounders that could influence the election outcome. Each election with no neutral votes ("treated group") is matched to an election with at least one neutral vote ("control group").
<iframe src="https://chart-studio.plotly.com/~iradukun/191.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>
From this plot, it is evident that the number of unsuccessful elections is higher in the control group than in the treated group. To quantify this difference, we execute a regression analysis, revealing that, on average, the chance of being elected drops from 60% to 45% when a candidate receives neutral votes.

So, given the observed impact of neutral votes, you should make efforts to minimize indecision among voters. You are advised to clearly articulate your stance, address concerns proactively, and foster an environment that encourages positive engagement. Try to build a consensus around your candidacy.
You finished this part? 

### Do I need any experience?

Yes, of course, you cannot wake up one day and simply decide to be a Wikipedia administrator. Until now, we've discussed factors that you can't directly control: the total number of votes and the percentage of neutral votes. Let's shift our focus to what you can do to enhance your profile as a strong, committed candidate.

Firstly, let's explore whether participating as a voter in a wiki RfA before your candidacy can positively impact your chances of acceptance.

<iframe src="https://chart-studio.plotly.com/~iradukun/170.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>

The bar chart illustrates a distinction between candidates with prior participation in the voting process and those without. Notably, 61% of candidates with previous engagement were successfully accepted as administrators, compared to only 36% of candidates lacking prior participation. Furthermore, employing a chi-square statistical test allowed us to reject the hypothesis that this difference could be attributed to chance alone.

However, it's crucial to recognize that concluding here might be premature. The factor of previous participation could be correlated with the total number of votes one receives or the percentage of positive votes. Therefore, the influence of previous participation may be confounded by these variables. To address this, we delve deeper by evaluating the effect of prior participation, considering covariates like the total number of votes and the percentage of positive and negative votes in the propensity score. This involves matching a candidate with previous participation (treated group) to a candidate without prior engagement (control group) with a similar propensity score.

<iframe src="https://chart-studio.plotly.com/~iradukun/206.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>

The plot highlights a discernible trend: candidates with at least one prior participation as voters exhibit a higher success rate in elections. A regression analysis further reveals that candidates with at least one previous participation as voters have, on average, a 61.3% chance of being elected, compared to only 36.3% for candidates who don't.

In essence, actively engaging as a voter in wiki RfA elections before your candidacy can strategically guide you through the election process. This involvement not only familiarizes you with the election dynamics but also contributes to a higher success rate, as observed in candidates with prior participation.


However, participating previously as a voter in the wiki RfA is not an experience in itself, right? So, let's now analyze the influence of having done revisions on a page of the English Wikipedia.

<iframe src="https://chart-studio.plotly.com/~iradukun/214.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>
The graph above indicates that 81% of the candidates had previously made revisions on a wiki page before their candidacy, with half of them having completed more than 3500 revisions before running for adminship. From our dataset, we cannot precisely determine the significance of these revisions, but as observed, it is a prevalent trend among candidates to showcase their commitment to the Wikipedia community through editing work. If you currently lack an edit history in your account, you might want to reconsider and roll up your sleeves, as this is even cited in 
[the Wikipedia guide for Requests for RfA](https://en.wikipedia.org/wiki/Wikipedia:Guide_to_requests_for_adminship#What_RfA_contributors_look_for_and_hope_to_see)
as one of the characteristics highly expected from a candidate.

<iframe src="https://chart-studio.plotly.com/~iradukun/217.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>
A substantial proportion of candidates without any prior revisions faces rejection, with only 32.2% of them experiencing a successful election. Within the group of candidates with prior revisions, although the numerical difference between the 47.4% of rejected candidates and the 52.6% of accepted candidates may appear small, a statistical t-test suggests that this difference is indeed significant.
Therefore, if you find yourself lacking an edit history, consider actively participating in wiki page revisions to demonstrate your commitment and increase your chances of a successful adminship candidacy.

Overall, in this first part of our analysis, you have seen that while surpassing the 75% threshold for the percentage of positive votes is crucial, there are additional factors that can booster your candidacy. So far, these factors can be categorized into two groups:

- *Factors you can directly influence* : previous participation as a voter in the voting process as well as a history of edits and revisions.
- *Factors you can indirectly influence* : the number of voters participating in the election and the percentage of neutral votes the candidate receives

Although, all of these factors don't depend entirely on you, you are able to influence them by developing the right skills or creating affinity with a Wikipedia community sharing the same interests. Stay with us to know more about this !

##### NLP graphs
{% include figure.html image="low_cloud.png"  position="right" width="600" height="700" %}
{% include figure.html image="need_cloud.png" position="left" width="600" height="700" %}
{% include figure.html image="lack_cloud.png" position="right" width="600" height="700" %}
{% include figure.html image="great_cloud.png"  position="left" width="600" height="700" %}
{% include figure.html image="knowledge_cloud.png"  position="right" width="600" height="700" %}    

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
* **Hint:** Refer to the following resources for a comprehensive understanding:

{% include button.html text="Edit summary ✍️" link="https://en.wikipedia.org/wiki/Help:Edit_summary" %}{% include button.html text="Mainspace 📜" link="https://en.wikipedia.org/wiki/Template:User_mainspace_edits" %}{% include button.html text="Wikipedia policies ⚖️" link="https://en.wikipedia.org/wiki/Category:Wikipedia_policies" %}{% include button.html text="Deletion 🧹" link="https://en.wikipedia.org/wiki/Wikipedia:Guide_to_deletion" %}{% include button.html text="Deal with vandalism ⚠️" link="https://en.wikipedia.org/wiki/Wikipedia:How_to_deal_with_vandalism" %}


### Important point not to neglect
Your interactions, affiliations, and connections will all play a significant role in influencing how other users may or may not support. The following section will show you some important aspects you will have to take into account before you embark on your path towards candidacy.
##### Unveiling the Influence of Group-Belonging on Voting Behavior
Have you ever wondered how belonging to specific groups or communities affects the way people vote? Well, within Wikipedia elections, these affiliations can heavily influence voting tendencies. Whether it's being part of editing circles, sharing common interests, or fostering alliances through interactions, these connections impact how individuals make their electoral choices.

In our quest to uncover these dynamics, we've constructed three essential networks:

* **Directed Voting Network:** Here, each weighted directed edge signifies either a positive or negative vote cast by one user toward another. This network illuminates the intricate web of voting relationships among users.
 
* **Agreement Network:** Within this network, edges connect users who display a significantly similar voting pattern. This network highlights significant congruence in voting behaviors among users.
 
* **Similarity Network:** This network draws connections between users who have regularly interacted with the same Wikipedia articles. By doing so, it unveils the relationships among users based on their shared interactions with specific Wikipedia content.
 
We then apply Louvain's algorithm to extract communities within these graphs, shifting our focus towards analyzing interactions within these communities and exploring the dynamics between different communities.

##### Let's look at the analysis conducted on the communities detected by Louvain's algorithm, both on the agreement network and the similarity network...

**1.** Users with a substantial history of mutual agreement tend to reciprocate with positive votes towards each other more frequently. Therefore, you must focus on fostering agreements and collaborations with other users. Engage actively in discussions, collaborate on editing projects, and aim to align your viewpoints with fellow community members. Building these alliances can increase the likelihood of receiving positive votes for your candidacy.

<iframe src="https://chart-studio.plotly.com/~iradukun/195.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>

**2.** Our analysis identifies communities of users demonstrating consistent agreement. Within these tightly-knit communities, the proportion of positive votes exchanged is above the average voting tendency. Therefore, aim to prioritize active participation within a community. Contribute meaningfully and engage constructively to earn support. Investing effort in building relationships within these groups can significantly boost the chances of your candidacy.

{% include figure.html image="./matrix_akram.png" %}

**3.** Notably, distinct groups of members engage with similar content categories such as Sports, Politics, History, Cinema, among others. These affinity groups exhibit a higher likelihood of casting positive votes toward fellow members with shared interests in specific content types. Thus, tailor your engagement to match these content-based groups. Show your enthusiasm and make substantial contributions within these thematic areas. By aligning your interests with these groups, you'll increase the chances of receiving positive votes from members who share similar passions.

<iframe src="https://chart-studio.plotly.com/~iradukun/198.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>

<iframe src="https://chart-studio.plotly.com/~iradukun/208.embed" width="800" height="700" frameborder="0" scrolling="no"></iframe>

Just like in your day-to-day interactions, here on Wikipedia, networking is crucial. Building positive relationships, engaging with the right individuals, and steering clear of conflicts can significantly boost your chances of success in the elections. Your network of supporters and allies can sway votes in your favor, underscoring the importance of nurturing these social connections.

##### <span style="color:green">A Farewell Message for the Future Administrator:</span>
<br>
Dear Future Wikipedia Administrator,

Becoming a Wikipedia administrator isn't just about gaining a title; it's about embracing a thrilling journey filled with challenges and opportunities. Your path to success combines the finesse of editing and creating content with the art of engaging with the community. Being an active member, contributing regularly, and fostering relationships with your peers are the keys that unlock the doors to victory.

Picture this: You're not just an editor; you're a reliable contributor, a passionate conversationalist, and a committed voter in the elections. These actions aren't just steps; they're leaps toward securing your place in the administrator's realm.

But here's the twist: Within this vibrant community, biases can exist. Users might rally around their own, forming tight-knit groups. But fear not, for networking is your superpower! Find your tribe, engage with those who share your passions, and blend in rather than stand apart. Your alliances will be your strength.

Now, let's talk about ethics. This isn't just a game—it's about shouldering immense responsibility. You're not just vying for a position; you're taking on a vital role in safeguarding the integrity of this encyclopedia. So, take a moment for introspection. Ask yourself, "Am I ready for this responsibility?"


> Remember, this isn't just about winning an election; it's about being a guardian of knowledge, entrusted with upholding the principles that define Wikipedia.
> Best of luck on your exhilarating quest to become a Wikipedia administrator!


