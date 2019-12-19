\## Contents:
\- [Overview](#Overview)
\- [Problem Statement](#Problem-Statement)
\- [Summary of Dataset](#Summary-of-Dataset)
\- [Executive Summary](#Executive-Summary)
\- [Conclusions and Recommendations](#Conclusions-and-Recommendations)---
\## Overview

For our first project, we're going to take a look at aggregate SAT and ACT scores and participation rates from each state in the United States. We'll seek to identify trends in the data and combine our data analysis with outside research to identify likely factors influencing participation rates and scores in various states.

\## Problem Statement

Analyse participation rates across states to determine the appropriate allocation of resources to improve SAT/ACT participation across states.

\## Summary of Dataset 

| Column Name           | Dataset (Test & Year)            | Type  | Description                                                  |
| --------------------- | -------------------------------- | ----- | ------------------------------------------------------------ |
| State                 | SAT 2017 & 2018, ACT 2017 & 2018 | STR   | Name of the State                                            |
| act2017_participation | ACT 2017                         | INT   | Participation rate of students  (in percentage) from the State for the 2017 ACT |
| act2017_eng           | ACT 2017                         | FLOAT | Mean score for the English test for the State                |
| act2017_math          | ACT 2017                         | FLOAT | Mean score for the Math test for the State                   |
| act2017_reading       | ACT 2017                         | FLOAT | Mean score for the Reading test for the State                |
| act2017_science       | ACT 2017                         | FLOAT | Mean score for the Science test for the State                |
| act2017_composite     | ACT 2017                         | FLOAT | Mean composite score for the State in all the tests (English, Math, Reading & Science) |
| sat2017_participation | SAT 2017                         | INT   | Participation rate of students  (in percentage) from the State for the 2017 SAT |
| sat2017_erw           | SAT 2017                         | INT   | Mean score for the Evidence-Based Reading and Writing test for the State |
| sat2017_math          | SAT 2017                         | INT   | Mean score for the Math test for the State                   |
| sat2017_total         | SAT 2017                         | INT   | Mean total score for the state in all SAT tests (Evidence-Based Reading and Writing & Math) |
| act2018_participation | ACT 2018                         | INT   | Participation rate of students  (in percentage) from the State for the 2018 ACT |
| act2018_composite     | ACT 2018                         | FLOAT | Mean composite score for the State in all the tests (English, Math, Reading & Science) |
| act2018_eng           | ACT 2018                         | FLOAT | Mean score for the English test for the State                |
| act2018_math          | ACT 2018                         | FLOAT | Mean score for the Math test for the State                   |
| act2018_reading       | ACT 2018                         | FLOAT | Mean score for the Reading test for the State                |
| act2018_science       | ACT 2018                         | FLOAT | Mean score for the Science test for the State                |
| sat2018_participation | SAT 2018                         | INT   | Participation rate of students  (in percentage) from the State for the 2018 SAT |
| sat2018_erw           | SAT 2018                         | INT   | Mean score for the Evidence-Based Reading and Writing test for the State |
| sat2018_math          | SAT 2018                         | INT   | Mean score for the Math test for the State                   |
| sat2018_total         | SAT 2018                         | INT   | Mean total score for the state in all SAT tests (Evidence-Based Reading and Writing & Math) |

|                          |       |                                                              |
| ------------------------ | ----- | ------------------------------------------------------------ |
| ACT_Participation        | float | Binned state ACT participation in 2017 and 2018              |
| ACT_English              | float | Binned state ACT english scores in 2017 and 2018             |
| ACT_Math                 | float | Binned state ACT math scores in 2017 and 2018                |
| ACT_Reading              | float | Binned state ACT reading scores in 2017 and 2018             |
| ACT_Science              | float | Binned state ACT science scores in 2017 and 2018             |
| ACT_Composite            | float | Binned state ACT composite scores in 2017 and 2018           |
| SAT_Participation        | float | Binned state SAT participation in 2017 and 2018              |
| SAT_ERW                  | float | Binned state SAT reading/writing scores in 2017 and 2018     |
| SAT_Math                 | float | Binned state SAT math scores in 2017 and 2018                |
| SAT_Total                | float | Binned state SAT total scores in 2017 and 2018               |
| sat_change_part_17_to_18 | float | 2018 less 2017 SAT participation                             |
| act_change_part_17_to_18 | float | 2018 less 2017 ACT participation                             |
| ACT_comparision          |       | ACT Participation rate and composite scores in 2017 and 2018 |
| SAT_comparision          |       | SAT Participation rate and total scores in 2017 and 2018     |
| rate_change              | STR   | SAT changes in rate of participation between 2017 and 2018   |
| rate_change_act          | STR   | ACT changes in rate of participation between 2017 and 2018   |
|                          |       |                                                              |

\\## Executive Summary

This project examines data regarding the participation rates and total/composite scores of students who took the SAT and ACT tests in the years of 2017 2018. The data are organised at state level, nationwide of 50 states, and also include the component subject scores. The analysis will follow a cross examination of participation rates and scores at the given years as well as the exploration of relationships between participation rates and scores attained.

The data set is consistent with the observation that there are states mandate of participation in one of the two tests as a requirement and the notion that students are showing a preference of one of the two tests. In addition, a strong negative correlation between test participation and average test score is determined, where states with low participation rates for a given test are likely to see higher total/composite scores as compared to a state with high participation rates on that same test. States with significant participation rate changes is also explored.

\### Trends and Analysis

SAT 

District of Columnbia and Minnesota maintains as the state that achieves the lowest and highest mean total  score respectively in both years. The states with the lowest participation rate of 2% in 2017 are: North Dakota, Mississippi and Iowa, while North Dakota taking the position of the only state in 2018 with the lowest participation rate. Connecticut, Delaware, Michigan remains as the states that has the highest participation rates in both years.

ACT

Maine has the lowest participants in both years. Neveda maintains as the state that achieves the lowest composite score in both years. Connecticut took over New Hampshire as the state that achieves the highest composite score in 2018, with New Hampshire following closely in 3rd. 17 states has the highest participation rate in 2017 and it became 18 states in 2018, with Ohio and Nebraska were added to the list of states and colorada was removed. 

Rate of Change

The state that had a rate change from 2017 to 2018 is the District of Columbia with a decrease in participation of 8% on the SAT.

Participation parameters

There are 22 states that records more than half of students studying in state schools taking the SAT.  ACT sees more success in the sense that more states - 31 - has more than 50% participants.

![2017_Part](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2017_Part.jpg)

![2017_Partvstotal](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2017_Partvstotal.jpg)

![2017act](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2017act.jpg)

![2017e_Part](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2017e_Part.jpg)

![2018_Part](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2018_Part.jpg)

![2018](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2018.jpg)

![2018t](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/2018t.jpg)

![20174](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/20174.jpg)

![20175](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/20175.jpg)

![20182](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/20182.jpg)

![201776](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/201776.jpg)

![box](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/box.jpg)

![box2](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/box2.jpg)

![changert](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/changert.jpg)

Illinois has a massive increase in participation rates between 2017 and 2018, as they traded the ACT for the SAT so their participation rate fell to 43% and SAT's rose from 9%.

Colorado, likewise, shows significant gains in SAT participation after removing the mandate of taking the ACT. 
Rhode Island and Florida have shown increases from 70-85% to near full participation. 

West Virginia shows opportunity as an area for growth, rising to 28% participation in 2018, while ACT rate fell, possibly from no legality. 

States like Nebraska and Ohio have 100% ACT participation in 2018, from 84% and 75% ACT rates in 2017, respectively. This is possibly from state policy changes where ACT is a mandatory test.

![changet](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/changet.jpg)

For ACT participation from 2017 to 2018, Ohio is the only state with more than 20% increase in testers. Alaska, Illinois and Colorado are the states with a decrease of more than 20% drop in participants. 


For SAT participation from 2017 to 2018, Illinois, Colorado and Rhode Island are the only states with more than 20% increase in testers. Florida is the only state with a decrease of more than 10% drop in participants. 

To evaluation participation, the box plot, heatmap, and histogram are constrasting. The correlation between the two tests are -.84, which is out of a scale -1 to 1. The extreme disparity between the highest peaks in the ACT and SAT participation rate histogram, top at 100-90% and bottom at 10–0% rates, highlights the divergence between the two test. Furthermore, SAT median participation rate is slightly above the lower limit of the ACT’s first quantile. Since the category is rather an integral measure of how related the two populations of the tests are, it is maybe not enabling a cross-comparison. 

![corr](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/corr.jpg)

![par1](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/par1.jpg)

![sat](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/sat.jpg)

![sat2017t](/Users/gabriellechases/Documents/Workcopy/Project1234/project_1/graph/sat2017t.jpg)

There are large differences in tester participation rates in some states which might bring biases in the results of certain analysis, which will be explored later. 

In 2017, the highest average SAT scores were found in the states of Minnesota, Wisconsin, and Iowa, where average total scores were over 1270. It’s worth noting that in these states, overall participation was quite low, with only 2 to 3% of students taking the test.

This pattern holds true across the board, with higher scoring states having lower participation rates. This is likely due to state preference or requirements related to the test. Students are not likely to take both the ACT and the SAT unless they know they will score well, and when given the choice, students often choose the test that they believe they’ll score higher on.

Similar states appear to have the same deduction year on year. Delaware, for instance, has low average SAT scores but has the highest SAT participation rates. The lowest average SAT scores were found in the states of Delaware and the District of Columbia where average total scores were all below 1000. On the other hand, highest mean SAT scores - Minnesota, Wisconsin, North Dakota, Missouri, Iowa - all have very low participation rates in the test. An inverse relationship between participation and average score in inferred here, with all the lowest performing states having participation rates above 90%. The analysis that students who do not choose and take the test as part of the requirement or a mandatory legality shows a lower below-average scores holds true as well. 

Mainly, there is selection biasness. Students who took the SAT test in states that prefer ACT tend to achieve higher average scores, especially if those students are looking for scholorships or moving out of state.

West Virginia, however,shows low average SAT scores at low end participation rates. In 2018, it sees an increase in participation too 100% despite not having a mandatory requirement and also because the state law regarding ACT terminated in 2018, and West Virginia has fee coverage for all public school students - (https://www.wsaz.com/content/news/All-WVa-high-school-juniors-to-begin-taking-SAT-exam-beginning-Spring-2018-444248263.html)

In 2018, high school students in the states of Minnesota, and Wisconsin achieved the highest average SAT scores with North Dakota added to the top-three list. The overall participation was between 2 to 3%.

A total of 17 states have 100% participation rates for the ACT in 2017 which can be deduced that ACT might be simply the prefered test as compared to the SAT.

Because higher participation tends to be associated with lower average scores, it is hard to compare SAT and ACT scores by state. Most states with high participation rates in one test have low participation rates, in other words, states that have high averages on one test, have low averages for the other. This is explored in further analysis in a second. 

The inverse relationship can be also seen in the ACT data. Minnesota, for example, despite 100% participation, is ranked low in terms of ACT composite score in the year 2017.

Florida, Georgia and Hawaii were the only states that has more than 50% participation on both tests in consecutive years. These states does not mandate students to sit for any one of the two tests. In both years, Hawaii scored best on the SAT and Georgia scored best on the ACT. Both North Carolina and South Carolina require ACT testing which also joined those three states in achieving a participation rate of above 50% SAT in 2018.

As we have analysed, average scores are highly negatively correlation with rate of participation on a given test. This confirms a selection bias effect.  

Mean scores on subject are highly correlated with mean scores for subject of the other test, or total scores for that test. If a state has high scores on the SAT because either due to low participation or students are high achievers. This holds for 2 years. 

Mean subject scores of the SAT are quite negatively correlated with mean scores on ACT, and vice versa. Again, due to the selection bias effect where higher ACT scores  > lower SAT participation > higher ACT participation > lower ACT scores).

Participation rates on a test is quite positively correlated against scores of the other test. This could be because higher SAT participation > lower ACT participation > higher ACT scores. 

From the diagrams below, mean and median indicate the centre and skewness, standard deviation and 25% or 75% quartiles indicate spread, minimum and maximum indicate range. 

The histogram on participation rates indicates that the distributions are somewhat trimodal. SAT has a huge peak around 0 and a smaller peak around 1. ACT has a huge peak around 1 and a smaller peak around 0. Both display a center peaks.

Distribution for both years did not change much from 2017 to 2018. SAT has a number of states with very low single digit participation rate of less than 10%, of the median to 75%, of the 100% participation. The ACT barely compares to the SAT with states of less than 10% participation, with largely concentrated at or near 100%. 

The histograms on math scores is a little like a normal distribution, a slight right skew. 

The histograms of reading/ verbal scores is distinctive bimodal with a  peak in the middle and a slight peak at the higher end. This shows there are limitations to the descriptive statistics.

These scatter plots exhibit a downward trend but not accurate for forecasting nonetheless. It's like stars in the dark sky. There is weak correlation. The degree of relationship is inverse, for instance a 21 average score in ACT to a 620 in SAT, a certain state shows high school seniors focuses and performs better in one test as compared to the other. The preference for one standardised test over another tends to be quite geographical in nature. In states with high SAT participation, ACT participation tends to be much lower, and vice versa.

Most states maintain the total SAT score from 2017 to 2018. Most states maintain the composite ACT score from 2017 to 2018. For the ACT Composite Scores in 2017 and 2018, most states follow the trend as seen in the congretion of dots along the best fit line. 

\##Conclusions/Recommendations 

![states that require the ACT and states that require the SAT magoosh](https://2aih25gkk2pi65s8wfa8kzvi-wpengine.netdna-ssl.com/hs/files/2017/05/bcc0207f-6fdd-4400-b7b4-30d6e4c8b0b5-600x398.png)



![img](https://www.applerouth.com/blog/wp-content/uploads/2018/11/Picture2-300x189.png)



![Average_SAT_Score_by_state_640_px](https://thumbor.forbes.com/thumbor/960x0/https%3A%2F%2Fblogs-images.forbes.com%2Fbentaylor%2Ffiles%2F2014%2F07%2FAverage_SAT_Score_by_state_640_px.jpg)

An issue with the comparison moving forward is not as disruptive as doing a hypothesis testing but still necessary to address. The heaet map concludes the analysis that there is a negative correlation between participation rates and scores, in that low participation rates in a state is highly correlated to high scores on a test. Considering the macro factors - demographically and the legality mandate to take the test - the connection between the two groups seem to be linked by an unseen third factor. The comparison will then be pivoted on analysing states with a certain threshold - a significant change in participation rates from 2017 to 2018. 


The ACT and SAT participation distributions are roughly the same with states tend to have a preference over a given test. ACT shows a large group of committed states with participation at 100% which also shows a higher baseline participation statewide. 

ACT and SAT scores are inversely correlated with their participation rates. This is likely due to selection bias, as low participation means those who are taking the test might be high achievers, whereas high participation dilutes the quality of performance by takers as reflected by the low scores. 

There are strong regional association with preference between ACT and SAT. Progressive states leans towards the SAT, while Midwestern conservative states favours the ACT.

The SAT made significant gains in 2018 relative to the ACT.

Moving forward, it is appropriate to focus on states showing similar positions to 2018.

Recommendations:

First and foremost, liaising with the respective states of education and retaining the relationship with states implementary a mandatory testing will bring an efficiency and a positive impact to the participation rates. 

Fee waivers or subsidies of the total costs of test for low income familities or even target high-achievers from these demograohic: providing impartial information and resources in order to get accepted for higher education.

University admission criteria and the scores current or past students had been accepted on and the composition of students are other aspects to improve the participation rates of a given test as the perceived value to succeed in the test increases. More univerisities are opting for the test-optional program so to reticy the rate of participation, this change of attitude has to be address. 

Partnership with test centers can help in strategising state targets.