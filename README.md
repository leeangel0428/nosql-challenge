# Introduction
Hello viewer and welcome to my submission for Challenge 12 aka the nosql-challenge. For context, at the time of writing this, I am enrolled in the Data Analytics and Visualizations bootcamp with the University of MN. We are assigned a challenge homework per module. This is Module 12's challenge on NoSQL. I am using a windows/PC laptop.

# Overview
"The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles."

Part One: Database and Jupyter Notebook Setup.

Part Two: Update the Database.

Given Reference Image to include in code: 
![7](https://github.com/leeangel0428/nosql-challenge/assets/137225965/e4f8b778-4e9f-4cb3-bb51-a3c36c451346)

Part Three: Exploratory Analysis.

Question 1: Which establishments have a hygiene score equal to 20? 

Question 2: Which establishments in London have a RatingValue greater than or equal to 4?

Question 3: What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

Q4.Question 4: How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

Given Reference image on what the final dataframe should look like:

![8](https://github.com/leeangel0428/nosql-challenge/assets/137225965/89db8349-42a8-492d-be90-d689dd38bede)

# Additional Information:
In this repository, you will find the Starter_Code folder that contains the NoSQL_analysis_starter and NoSQL_setup_starter codes that complete the assignment. There is also a Resources folder that contains the establishments JSON file. Aside from the sources cited below, everything used was retained information gathered from my classes and class activities. As always shout out to my bootcamp TAs Sam and Randy for all their help answering my questions during office hours, my instructor Hunter for always being clear in his articulation of the course material, and my classmates for their encouragement and support.

# Troubleshooting:
In the NoSQL_setup_starter code, I ran into an issue on Part 2, task 2. The output was long and continous. See image.
![1](https://github.com/leeangel0428/nosql-challenge/assets/137225965/c3d20543-53a7-45cd-972a-ec3398d1c672)

I then fixed it by using ".find_one". See image.
![2](https://github.com/leeangel0428/nosql-challenge/assets/137225965/352b701e-223c-4846-a4ac-81d2f747b063)

In the NoSQL_analysis_starter code, I ran into another issue on Part 3, question 4. My output included the "LocalAuthorityName" which later on caused another issue with my dataframe where the id included "LocalAuthorityName:" in each element. This does not match the given reference image for how the dataframe should appear. See images.
![3](https://github.com/leeangel0428/nosql-challenge/assets/137225965/f4fd8cba-44fc-4c43-aff0-baabf18df011)
![4](https://github.com/leeangel0428/nosql-challenge/assets/137225965/89534a90-791b-48c1-a4c8-2d9da9e83e61)

I then fixed it by correcting the "group_query" to exclude it. See image.
![5](https://github.com/leeangel0428/nosql-challenge/assets/137225965/acfa1383-0a88-40f5-96fd-dead5faca038)
![6](https://github.com/leeangel0428/nosql-challenge/assets/137225965/00f5dec7-d3d8-4c41-8608-16d5a6f0a655)

# Resources and Citations:
#### Used to update data types:

MongoDB. (2023). $toDecimal(aggregation). MongoDB Manual. Retrieved from: https://www.mongodb.com/docs/manual/reference/operator/aggregation/toDecimal/

MongoDB. (2023). $toDouble(aggregation). MongoDB Manual. Retrieved from: https://www.mongodb.com/docs/manual/reference/operator/aggregation/toDouble/

MongoDB. (2023). $toInt(aggregation). MongoDB Manual. Retrieved from:  https://www.mongodb.com/docs/manual/reference/operator/aggregation/toInt/

#### Used to add images onto readme:

Tech Projects. (2020, September 18). Add image/screenshot of your project to your GitHub repository [Video]. https://www.youtube.com/watch?v=NVibWKkon74&ab_channel=TechProjects

#### Used for indepth learning on "update_many":

Tyagi, A. (n.d.). Python MongoDB- Update_many Query. Geeks for Geeks. Retrieved from: https://www.geeksforgeeks.org/python-mongodb-update_many-query/





