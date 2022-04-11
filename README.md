How Has Energy Consumption Changed in Past History
================
by Loren, Jackie, Owen

## Introduction

According to the NOAA, global CO2 levels were at 313 parts per million
(ppm) in 1959. Just 6 decades later, they have reached 417 ppm, as of
October 2021. Most of the greenhouse gas emission into the atmosphere
each year is driven by fossil fuel combustion. Although the world has
made efforts to shift to renewable energy sources like wind, hydropower,
and solar, drastic changes need to be made in order for humanity to
avoid the worst of climate change.

Global warming can lead to infectious diseases, changes in agricultural
productivity, respiratory ailments, environment degredation, and even
deteriorate the ecosystem of different species which in turn can affect
how we live our lives. Over the last century, the average surface
temperature of the Earth has increased by about 1.0 degree Fahrenheit.
One of the main drivers of global warming is energy consumption, and
more specifically fossil fuel combustion. Our group is interested in
studying the different types of energy consumption in different
countries around the world to see who is still heavily dependent on
fossil fuels versus who is making progress towards renewables. What do
these trends look like over time in comparison to fossil fuel usage?
After finding an ideal data set, we decided to narrow our search,
understanding how fossil fuels and renewable energies change overtime
for different countries, focusing on the energy consumption as well as
the energy consumption per capita.

The dataset we have chosen is World Energy Consumption, a dataset
consisting of key metrics of energy usage (primary energy, per capita,
growth rates, energy mix, electricity mix, and other metrics) from
Kaggle. This data set is part of Our World in Data, which seeks to
collect data and research the world’s largest problems. Initially, the
data set contained 122 columns of variables, and over 17,000
observations for each country from 1900 to the present. There were many
observations which had “NA” as their entry.

Because there were over 100 columns and over 17,000 observations, we
wanted to focus our findings on a few specific countries as well as a
few specific variables. During the cleaning process, we focused on
creating a data frame that included country, year, and energy
consumption from wind, solar, other renewables, nuclear, and fossil
fuels. After creating this data frame, we noticed that we still had a
lot of information and decided that it was best to look at how energy
consumption has changed in the past two-three decades for a few
developed and industrialized countries.

## Methodology

While looking at our research topic we began by making a simple
comparison graph, looking at the development of solar energy in the past
20 years for a set of a few developed countries of interest. After
seeing a few unexpected trends, we decided to make leaflet plots as well
as a comparison graph that focused on looking at the fossil fuel
consumption for China and the United States. Our leaflet focused on
renewable energy consumption for 1900 and 2018 (the most recent
comprehensive global data in our dataset). After making this
visualization, our group was interested in looking at how a variety of
energy sources would differ for a list of countries. Generating these
visualizations, we noticed that because we had a list of a lot of
different countries, it was hard to identify which line matched with
which country based on our key. As a result, we added an additional
feature to our visualization, giving the information of country and
value when highlighting a specific data point in the graph. The same
ideas were also implemented in our leaflet of the world, showing the
renewable energy share between countries across the world in 1990 and
2018. We also decided to create a faceted bar graph of the different
types of energy consumption each country has used in the past 20 years.
Through these visualizations we observed that because of the two leading
countries in energy consumption, we created a visualization that focused
on the two countries (China and the United States). After understanding
the story the data could tell us, we decided to create a prediction
model to help predict energy consumption for the leading countries in
future years because China and the United States are definitely the most
influential countries in terms of affecting the environment and the
world.

## Findings + Discussion

Our linear regression models for the USA and China have r^2 values of
0.141 and 0.946, respectively. This is surprising because upon visual
inspection of the plot with both predicted and actual data, the USA
regression line closely follows the data, which appears to be just as if
not more linear than the China data. In 1990, the USA consumed about
twice as much fossil fuel as China. In 2018, the USA consumed about ⅔
the amount of fossil fuel as china. By 2030, China is predicted to
consume about twice as much fossil fuel as the USA. Perhaps China will
consider utilizing a higher proportion of renewable sources as their
energy demands continue to grow. Our figures show that China and the
United States consume the most energy, but have made little overall
progress to diversify their energy consumption in comparison to
countries like Finland. With that, our visualizations show that smaller
countries with less energy usage lead the charge in renewables, possibly
because they do not have to generate as much total energy to support
their smaller populations. Our bar chart shows that in general,
renewable sources contribute evenly to energy consumption in the US and
China. Additionally, our figures show an interesting relationship
between leaders in solar, wind, and nuclear which depends on whether we
look at per capita, or overall generation. We see that usually, larger
countries produce more total renewable energy, but this makes up a much
smaller percentage of their total energy consumption. If we look at per
capita, we see that smaller countries are in fact leaders in renewable
energy generation/consumption.

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

World Energy Consumption:
url(<https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption>)

“This dataset is a collection of key metrics maintained by Our World in
Data. It is updated regularly and includes data on energy consumption
(primary energy, per capita, and growth rates), energy mix, electricity
mix and other relevant metrics.”

## References

Poudel, P, *World Energy Consumption: Consumption of energy by different
countries,* electronic dataset, viewed 28 February 2022,
<https://www.kaggle.com/pralabhpoudel/world-energy-consumption>
