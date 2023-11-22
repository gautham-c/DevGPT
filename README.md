# CEN 5035 – SOFTWARE ENGINEERING

## Group- 10

#### Gautham Chadalavada(GC23M), V S Madhura Gayathri Mannava(VM23P), Ruchitha Reddy Munugala(RM23S)

### Research Questions

1. How does the use of ChatGPT impact the software development process and the overall 
quality of software by analyzing the success rate of issues based on the prompts given by 
the users?

2. How does the result that ChatGPT produces for a query differ with respect to quality issues 
when compared to that of internet-based searches (Google Search)?

3. Do developers often find the number of turns required to reach a conclusion in ChatGPT 
conversations consistent or variable for different issues?

### Folder Structure
- Research Question 1
    - Dataset:20230727_195954_discussion_sharings.json
    - Code for analysis and visualisation: rq1.ipynb

- Research Question 3
    - Dataset: 20230727_195816_hn_sharings.json
    - Code for analysis and visualisation: rq3.ipynb

### Working
#### Research Question 1:
For this question, to analyse the success rate, we use the dataset 20230727_195954_discussion_sharings.json from Snapshot1 of DevGPT dataset. In this dataset we are using the closed column and the upvote column to analyze the success rate. With the help of the closed column we calculated the Closure rate of each issue. With the Created Time and UpdatedTime, we calculated the mean and median seconds for the closing the issues. Then with the help of the scipy library, we calculated the t-stat value and the p-value. Then we performed the data visualisation using the pareto graph using the mathplotlib and seborn libraries.

#### Research Question 3:
For this question, to analyze the consistency of number of turns required to reach conclusion, we use the dataset 20230727_195816_hn_sharings.json from Snapshot1 of DevGPT dataset. In this dataset we are extracting data from ChatgptSharing array and getting new dataframe tokenAnswers. From this, we are creating three new dataframes: topics, number of turns and complexity. We calculated mean and mode of number of turns which is usually taken by the user. Then we performed the data visualization using scatterplot, matplotlib and seaborn libraries.

