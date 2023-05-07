# Rates of Competitive Success in High School Debate Between Private and Public Schools

**Introduction:**  
The question we wanted to answer with our project was, what is the difference in competitive success between private and public schools in high school debate? There is a huge disparity in the number of resources offered to students at public and private schools. We think that comparing the competitive outcomes between these two groups could give policy makers key insight about resource disparities and educational inequality. Our hypothesis is that Private schools have statistically significant higher rates of competitive success in high school debate than public schools. This means that we should see debaters from private schools receiving higher speaker scores and z-scores than debaters from public schools.  


**Dataset:** We decided to limit our dataset to LD octas bid tournaments from 2020-2021 for a few reasons. First, we decided to limit the time-frame to 2020-2021 because it would eliminate the possibility of varying results do to a transition to online debate. We also wanted to limit our dataset to just LD debate because it is a 1v1 format versus other forms of debate being 2v2 or 3v3. This allowed us to look at individual competitive success. Finally, we used only octas bid tournaments because these are national tournaments that are the most organized, have the most attendees, most qualified judges, and most impactful for debaters’ competitive success. In order to compile our data, first, we created a scrape function to scrape the data and export it to a dataframe from the website [tabroom.com](https://www.tabroom.com/index/index.mhtml) which is a website that hosts debate tournaments online as well as stores the results of past tournaments. Then we cleaned up our data so each dataset would have the same columns and column names, this was very code intensive. We also manually created a key for each unique school in our dataset because some schools had weird names (ex: independent entries), and there were only 300 unique school names. When we are analyzing our data, we will be utilizing the 1HL Speaker Scores and the Z-scores. For context, in Lincoln-Douglas Debate, students are awarded a speaker score ranging from 0-30 (speaker scores most typically range from 25-30, 25 being very bad and 30 being perfect; anything below 25 is reserved for speeches that had some other problem, like if the speaker said something offensive). The 1HL Speaker Total Score is the sum of the speaker points subtracting the highest and lowest speaks. The Z-score is a score that just sums the speaks but tries to account for judge biases (ie. some judges just naturally give higher or lower speaks) and standardized everyone's score.

**Methodology:** First, we will take initial counts of public vs. private school attendance at tournaments to gauge representation. Next, we will start our initial mean comparisons and to get an initial understanding of our data. Then, we will switch our analysis to be tournament by tournament and round by round. We will then find the difference in round average speaks and find the 95% and 99% confidence intervals for the difference between private and public schools. We will then run these tests again using Z-score to try and account for judge biases.



* Edit 05/06/2023: Code for webscraping Berkeley was changed since the start of the project. This is because the original website split the data table into 3. The new code scrapes all 3 tables and combines/cleans them. If the website gets fixed, I will put the old code back!
