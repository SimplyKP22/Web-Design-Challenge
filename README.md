# Web-Design-Challenge

## Overview:
	HTML (HyperText Markup Language) and CSS (Cascading Style Sheets) allow us to display information to a user in a more easily digestible and visually appealing way. Since users are familiar with HTML because websites are built using this language, the user interface can be much easier to use. In this exercise, we will utilize HTML and CSS to feature data put together from a previous Python API exercise, where we gathered and analyzed weather-related data about cities based on their latitude. We will also be showcasing some of the functionality of Bootstrap, which is a web-based application that allows us to make our webpage more dynamic and easier to use. 
	We begin by creating our primary HTML foundation site, along with the resource files that will house the visualizations of our data analysis. This initial index.html site will act as the landing page for our website. Since all of our pages will feature the same theme and similar functionality as the landing page, this is where we will spend the time developing the navigation bar and making sure our links within that bar are located in the right place. We will also create the template that will be used for the pages that will feature our data visualizations. To do this, we will utilize the bootstrap functionality to make the navigation bar, along with containers on the landing page that will contain the visualizations, headers, and main description for the landing page and the exercise.
	Once we are happy with the setup of the landing page, we can then create the remaining plot pages by simply duplicating the landing page and making adjustments to our headers and the file references for the visualizations relevant to that page. For example, we would want to make sure that we display the temperature graph for the temperature plot page and not the humidity page. We can begin constructing the remaining pages for the relevant plots when we are done with the landing page. 
	Upon completing the setup for the pages for each plot, we also want to develop the comparison and data pages. These pages will follow a very similar structure that we used for the plot pages, except we will need to utilize the grid functionality from Bootstrap for the comparison page and the table functionality for the data page to make sure the data is displayed appropriately. To develop the table for the data page, we will first look at the CSV file containing our city data and convert it to an HTML format. To do this, we import the data into a jupyter notebook and utilize the pandas library to convert the file into a dataframe. We can then use the to_html method to a version of the data that can be placed on our HTML data page. Once this is done, we will notice that the page will display our table data. 
	Using HTML and CSS, we can easily display our data and analysis in a visually appealing way and easily referenced by the user. We can also allow the information to be much easier to share with various users by hosting the pages on a website. 

### Website Requirements


The website must consist of seven pages in total, including:

* A ontaining the following elements:

  * An explanation of the project

  * Links to each visualizations page. There should be a sidebar containing preview images of each plot. Clicking an image should take the user to that visualization.

* Four visualization pages, stored in the `visualizations` folder, each with the following elements:

  * A descriptive title and heading tag.

  * The plot or visualization for the selected comparison (latitude vs: max temperature, humidity, cloudiness, or wind speed). The images displayed on these pages should be stored in the `assets/images` folder.

  * A paragraph describing the plot and its significance.

* A Comparisons page that does the following:

  * Contains all of the visualizations on the same page so they can easily be compared with each other.

  * Uses a Bootstrap grid for the visualizations.

    * The grid must be two visualizations across medium and large screens, and it must be one visualization across on extra-small or small screens.

* A Data page that displays a responsive table containing the data used in the visualizations.

  * The table must be a Bootstrap table component. Refer to the Bootstrap documentation for how to use responsive tables. 

  * The data must come from exporting the `.csv` file as HTML or by converting it to HTML. Try using a tool that you already know: Pandas. Pandas has a method, appropriately called `to_html`, that allows you to generate an HTML table from a Pandas DataFrame. 

At the top of every page, the website must have a navigation menu with the following elements:

* It should have the name of the site on the left of the navigation bar, allowing users to return to the landing page from any page.

* It should contain a dropdown menu on the right of the navigation bar, named "Plots," to provide links to each individual visualization page.

* It should provide two more text links on the right: "Comparisons," which links to the comparisons page, and "Data," which links to the data page.

