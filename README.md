# Assignment 1: Protests
The past few years in the United States, there has been a surge in protests in support of Black Lives Matter, gender equity, and other social issues. In this assignment, you'll work with data from [CountLove](https://countlove.org/) -- the same data often [cited](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html) by the New York Times -- to learn more about demonstrations over the past few years. 

By completing the assignment, you will demonstrate the following skills:

- Use of **version control** for managing your code
- Declaring document rendering using **markdown** syntax
- Foundational programming skills in R. 


## Background Research
Before diving into this (or any) dataset, it's important to have _domain familiarity_ (i.e., to know something about the topic). As preparation, I'm asking that you read **three articles** about protests in the U.S., and provide a brief 1 - 2 sentence summary or takeaway from each one. 

In the section below, create an **unordered list** of the three articles you found. Make sure to provide an appropriate markdown link (_not_ just the URL) to the article in addition to your 1 - 2 sentence summary. 

1.[This is an article](https://www.nytimes.com/interactive/2020/07/03/us/george-floyd-protests-crowd-size.html) about the significance and overall importance of the George Floyd Protests. I didn't really understand how big those protests were when they were happening and this article helps put it into perspective.

2.Another [George Floyd Article] (https://www.usatoday.com/in-depth/graphics/2020/06/03/map-protests-wake-george-floyds-death/5310149002/) that shows a map of protests that happened as a response to George Floyd's Death

3.
This [George Floyd](https://www.nytimes.com/2020/06/06/us/protests-today-police-george-floyd.html) article is closer to the death of George Floyd. This was about 1-2 weeks after his death, and focuses more on the different memorials that happened throughout the USA. 


## Accompanying Image 
In this section, please **display one image** to accompany your text, and describe _why_ you included it (~2 - 3 sentences). This will require that you download an image into your project folder. In your description, use **bold** and _italics_ (at least once, for practice) to emphasize some of your points. 

## Analysis
At this point, you should open up your `analysis.R` script to begin working with the data. The script will guide you through an initial analysis of the data. Throughout the script, there are prompts labeled **Reflection**. Please write 1 - 2 sentences for each of these reflections below:

- What does the difference between the mean and the median tell you about the *distribution* of the data?

The difference between the mean and the median will tell us that theresome protests that have high turnout, for example, the max attendees is 725k but the min attendees is 0 .This shows that there is a high variability for attendees in a protests. The median being 100, shows us that there are more protests that are lower in volume compared to protests that have higher turnout. There are lots of protests going on and most of them are small in terms of attendees. 

- Does the number of protests in Washington surprise you? Why or why not?

Three percent at first doesn't seem like a lot of protests, but looking at it compared to the number of protests and how many states there are in the US, three percent is a lot of protests. I am not surprised that WA has a lot of protests. WA is a progressive state in general and historically. We had big protests in the 90's and recent protests such as the woman's march and BLM.

- Looking at the `state_table` variable, what data quality issues do you notice, and how would you use that to change your analysis (no need to actually change your analysis)?

Some states are written in lower case letters so they count as another state. There aren't alot of them but they do skew the overall data set. I would change the states vector to only extract capital letters with another stringer subset function, maybe either str_extract or str_match. 

- Does the change in the number of protests from 2019 to 2020 surprise you? Why or why not?
This does not surprise me because 2020 was a tough year compared to 2020. Significant events that happened in 2020 ranges from  George Floyd Protests, Trumps end of presidency, the eletion, BLM Protests, and etc.  2020 was a tough year for everyone in the world but the pandemic highlighted a lot of the injustices of the previous president and also the racial injustices that have plagued the United States for years.

- Do a bit of research. Find at least *two specific policies* that have been changed as a result of protests in 2020. These may be at the city, state, or University level. Please provide a basic summary, as well as a link to each article.
- Take a look (`View()`) your `high_level_table` variable. What picture does this paint of the U.S.?

[This article](https://www.seattlepi.com/coronavirus/article/washington-state-coronavirus-outbreak-timeline-15188450.php) basically looks at the history of washington and coronavirus. The lockdown was a really big policy change that affected lots of people in WA. 
[This article](https://www.statnews.com/2020/05/29/trump-us-terminate-who-relationship/) is about Trump terminating our relationship with WHO. When COVID started I immediately took a global health class and I researched a lot about WHO and what they did. It was crazy to think that our previous president would terminate a relationship with WHO during a pandemic. 


When looking at this table I Can see some patterns here and there and contrast them with different time periods in history. One positive aspect I can take away from this table is that, if change needs to happen we go out and declare our rights and fight for that change. The problem is, most of the problems that are happening right now are the same problems that keep repeating themselves. 


## Final Thoughts
When you are finished, with your analysis, please answer the following questions in 1-2 sentences each. 

- What about the analysis surprised you?

Nothing too big was a surprise too many, It kind of just reassured a lot of the assumptions that I had when it comes to protests
in the USA. The biggest surprise was the fact that you can have protests with no people and that there were protests in places that I personally have never heard of. 

- What parts of this analysis did you find challenging?

The most chellenging part of the analysis was dealing with the dates and using the stringr package. Also, I personally don't like reading the news because it's personally very frustrating for me, looking at articles about George Floyd made me really angry at the state of the USA today and made me realize how big of a deal that whole situation was, it is now 2021 and because of the constant events that is happening in the USA it feels as if the George Floyd Incident was centuries ago. 

- What types of analysis do you wish you were able to do with the dataset, but currently don't have the technical skills to do?

What I really wanted to do in terms of the personal function at the end was to able to return more information about the protests in terms of the row itself. Like for example if I ask if there was a protest in this location, I would like it to return yes or no, and if yes how many and if I want to, I can inquire about all the other information about those protests like Attendees, Purpose, Article, and etc. With the Stringr package I felt like I was confined to one column, I was trying to use the join functions but it didn't really work out the way I wanted it to be. 
