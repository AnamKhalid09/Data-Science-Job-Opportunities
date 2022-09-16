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

4. Inside the folder you just created, add new file called `data_science.ipynb`. These will be the main scripts to run for each analysis.

5. Push the above changes to GitHub.

### Adding a .gitignore File

We don't want the `api_keys.py` file containing the API key to be exposed to the public on GitHub; this would mean anyone could copy and use our API key, possibly incurring charges.

When we type `git status` in the command line, we can see all the untracked files that we have created so far.

If we only wanted to add the `data_science.ipynb` file to GitHub, we could type `git add `data_science.ipynb``. However, every time we want to add a new file or update current files to the repository, we would have to add each file individually, which is time-consuming and cumbersome. Instead, we can add the files that we don't want to track to the `.gitignore` file.

Before we add our files to GitHub, let's add `api_keys.py` to the `.gitignore` file. Use the following instructions:

1. Open your `project-one` GitHub folder in VS Code/Anaconda.

2. Open the `.gitignore` file, and on the first line, type the following code:

```python
# Adding config.py file.
api_keys.py
```

3. While the `.gitignore` file is open, add the `API_practice.ipynb` and `random_numbers.ipynb` files and save the file.

4. In the command line, type `git status` and press Enter. The output should indicate that the `.gitignore` file has been modified and the ``data_science.ipynb`` file is untracked.

5. Use `git add`, `git commit`, and `git push` to commit the modifications to `.gitignore` and the ``data_science.ipynb`` file to GitHub.

On GitHub, the only new file you should find is the `WeatherPy.ipynb` file.

## Part 1: WeatherPy

In this section, you'll create a Python script to visualise the weather of 500+ cities of varying distance from the equator. To do so, you'll use a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and your problem-solving skills to create a representative model of weather across cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

- Temperature (C) vs. Latitude

After each plot, add a sentence or two explaining what the code is analysing.

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature (C) vs. Latitude

After each pair of plots, explain what the linear regression is modelling. For example, describe any relationships that you notice and any other findings you may have.

Your final notebook must:

- Randomly select **at least** 500 unique (non-repeated) cities based on latitude and longitude.
- Perform a weather check on each of the cities using a series of successive API calls.
- Include a print log of each city as it's being processed, with the city number and city name.
- Save a CSV of all retrieved data and a PNG image for each scatter plot.

### Part 2: VacationPy

Now, let's use your skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.

- **Note:** Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out [Google Maps Platform Billing](https://developers.google.com/maps/billing/gmp-billing#monitor-and-restrict-consumption) and [Manage your cost of use](https://developers.google.com/maps/documentation/javascript/usage-and-billing#set-caps) for more information.

- **Note:** If you are having trouble displaying the maps, run `jupyter nbextension enable --py gmaps` in your environment and then retry.

To complete this part of the assignment, you will need to do the following:

- Create a heat map that displays the humidity for every city from Part 1, as in the following image:

  ![heatmap](Images/heatmap.png)

- Narrow down the DataFrame to find your ideal weather condition. For example:

  - Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

  - **Note:** Feel free to adjust your specifications, but make sure to limit the number of rows returned by your API requests to a reasonable number.

- Use Google Places API to find the first hotel for each city located within 5,000 metres of your coordinates.

- Plot the hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**, as in the following image:

  ![hotel map](Images/hotel_map.png)

As final considerations:

- You must complete your analysis using a Jupyter notebook.
- You must use the Matplotlib or Pandas plotting libraries.
- Your plots must include labelling aspects like plot title (with date of analysis) and axis labels.
- For max intensity in the heatmap, try setting it to the highest humidity found in the dataset.

## Hints and Considerations

- If you'd like a refresher on the geographic coordinate system, [this site](http://desktop.arcgis.com/en/arcmap/10.3/guide-books/map-projections/about-geographic-coordinate-systems.htm) has great information.

- A starter code for citipy has been provided. However, if you're craving an extra challenge, push yourself to learn how it works: [citipy Python library](https://pypi.python.org/pypi/citipy). Before you try to incorporate the library in your analysis, start with simple test cases outside your main script to confirm that you are using it correctly. Often, when introduced to a new library, students will spend hours trying to figure out errors in their code&mdash;a simple test case can save you a lot of time and frustration.


**References: https://medium.datadriveninvestor.com/is-data-science-ranked-as-the-sexiest-job-for-2023-and-beyond-cf66d8ba5585
