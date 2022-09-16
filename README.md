# Project-1

# Project-Title: Data Science employment opportunities in Australia

![image](https://user-images.githubusercontent.com/109832565/190567544-cf01d579-eb63-4f88-a4e2-c3a6665e6c0c.png)


## Background

**According to an IBM report, data science jobs will show a growth of 30%. As per the US Bureau of Labor Statistics, about 11 million jobs would be created by the year 2026. The US Bureau of Labor Statistics further predicts a stupendous growth in the data science field between now and 2029, with professionals being paid quite well. According to a websource, Data scientist is ranked #3 in best technology jobs on the global charts!(See References)

Now the question is, Do we have data that supports this narration? If yes, how is the field doing in Australia? Are data scientists being paid well in Australia? What job titles are at the top in terms of salary? How about the distribution of opportunities among different states? Does being in Metro or Regional affects the job opportunities? What skills are the pre-requisites? 

### Before You Begin

1. Create a new repository for this project and name it as **project-one**. 
   **Do not add this to an existing repository**.

2. Clone the new repository to your computer.

3. Inside your local Git repository, create a directory. Use a folder name such as: **Data-Science**.

4. Inside the folder you just created, add new file called `data_science.ipynb`. These will be the main script to run for each analysis.

6. Create another folder called **Resources** and put your csv file in it.

7. Add a .gitignore file as a good practice in case you want to keep any confidential files in it like your API keys. .gitignore file will keep all the files hidden from being published publicly even if your repository is public. For API keys, open your .gitignore file and in the first line type the following:

```python
# Adding config.py file.
api_keys.py
```

8.Add a README.md file to share your approach towards project.

9. Push the above changes to GitHub.

## Data-Science

In this folder, you'll create a Python script to visualise the 

The first requirement is to create a series of scatter plots to showcase the following relationships:

- Temperature (C) vs. Latitude

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Your final notebook must:

- Randomly select **at least** 500 unique (non-repeated) cities based on latitude and longitude.
- Perform a weather check on each of the cities using a series of successive API calls.
- Include a print log of each city as it's being processed, with the city number and city name.
- Save a CSV of all retrieved data and a PNG image for each scatter plot.

- **Note:** If you are having trouble displaying the maps, run `jupyter nbextension enable --py gmaps` in your environment and then retry.

## Considerations
##References:
https://medium.datadriveninvestor.com/is-data-science-ranked-as-the-sexiest-job-for-2023-and-beyond-cf66d8ba5585
