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

<iframe src="https://chart-studio.plotly.com/~iradukun/124.embed" width="800" height="500" frameborder="0" scrolling="no"></iframe>
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
<iframe src="https://chart-studio.plotly.com/~iradukun/150.embed" width="900" height="600" frameborder="0" scrolling="no"></iframe>
Upon examining the boxplot, a disparity in the distribution of total votes between successful and unsuccessful elections becomes evident. The median for unsuccessful elections is approximately 20%, while for successful elections, it is 59%. This suggests a tendency for unsuccessful elections to garner a lower total vote count. Now, do these results hold significant differences? Absolutely. We conduct a statistical t-test, leading us to confidently reject the null hypothesis. Thus, it appears that the total number of votes may indeed play a role in determining election outcomes.

You might be wondering why we used the term "may" in attributing a role to total votes. The reason is that, at this point, we cannot be entirely certain. Correlation does not imply causation, and various confounding factors undoubtedly impact the results. To try to isolate the effect of the total number of votes, we conduct a paired matching, accounting for the percentage of positive and negative votes as confounders. In this case, the treatment involves receiving a number of votes above the average, which stands at 50.4.
<iframe src="https://chart-studio.plotly.com/~iradukun/156.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>
The proportions of elections won and lost in the control group are fairly balanced (49% won and 51% lost). In contrast, a substantial disparity emerges in the treated group—those with an above-average number of votes—where 69% are won and 31% are lost. Therefore, if at the end of your election, you notice you had a high number of voters, you definitely have higher chances to see your candidacy accepted.

##### So, a lot of voters…But, what percentage of positive votes to secure an adminship position?

Of course, the type of votes you receive plays a crucial role. [The Wikipedia guide for Requests for Adminship (RfA)](https://en.wikipedia.org/wiki/Wikipedia:Requests_for_adminship#Discussion,_decision,_and_closing_procedures) states that achieving 75% or more positive votes is essential for passing. However, success in RfA goes beyond accumulating positive votes. The final decision rests with the bureaucrats, who evaluate factors beyond mere percentages. They consider the quality of arguments from voters, the strength of comments in the "Neutral" section, and discount any votes deemed invalid.
<iframe src="https://chart-studio.plotly.com/~iradukun/162.embed" width="800" height="600" frameborder="0" scrolling="no"></iframe>
You can notice that there are some exceptions that have a very high positive vote percentage, yet end up not being elected, and vice-versa. Which echoes the fact that a certain percentage of votes is not a guarantee of a successful election. Indeed, there are even cases where candidates were rejected even if 100% of the votes they received were positive. But, you should note that for the majority of these elections, either the candidate refused the nomination, or the election was withdrawn by a bureaucrat who deemed the candidate unprepared. Thus, the percentage of positive votes remains at 100% due to the sudden end of the election but the recorded outcome is unsuccessful. 
It's also worth noting that, for the majority of cases, having less than 50% positive votes appears to guarantee election failure. Additionally, only 6.66% of candidates who fall short of the indicative threshold of 75% positive votes manage successful elections. Keep these thresholds in mind as you gather a substantial number of positive votes to enhance your chances of election success.
<iframe src="https://chart-studio.plotly.com/~iradukun/170.embed" width="700" height="600" frameborder="0" scrolling="no"></iframe>
