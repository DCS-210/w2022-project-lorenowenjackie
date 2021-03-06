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
productivity, respiratory ailments, environmental degradation, and even
deteriorate the ecosystem of different species which in turn can affect
how we live our lives. Over the last century, the average surface
temperature of the Earth has increased by about 1.0 degree Fahrenheit.
One of the main drivers of global warming is energy consumption, and
more specifically fossil fuel combustion. Our group is interested in
studying the different types of energy consumption in different
countries around the world to see who is still heavily dependent on
fossil fuels versus who is making progress towards renewables. Which
countries are consuming the most energy? What do these trends look like
over time in comparison to fossil fuel usage? Who is emitted the most
carbon? Can we predict these trends into the future? After finding an
ideal data set, we decided to narrow our search, understanding how
fossil fuels and renewable energies change overtime for different
countries, focusing on the energy consumption as well as the energy
consumption per capita.

It appears that the USA and China are by far the largest consumers of
energy, and in particular fossil fuels, so we wanted to look at energy
consumption trends for these countries and potentially make future
predictions.

## Methodology

The dataset we have chosen is World Energy Consumption, a dataset
consisting of key metrics of energy usage (primary energy, per capita,
growth rates, energy mix, electricity mix, and other metrics) from
Kaggle. This data set is part of Our World in Data, which seeks to
collect data and research the world???s largest problems. Initially, the
data set contained 122 columns of variables, and over 17,000
observations for each country from 1900 to the present. There were many
observations which had ???NA??? as their entry.

Because there were over 100 columns and over 17,000 observations, we
wanted to focus our findings on a few specific countries as well as a
few specific variables. During the cleaning process, we focused on
creating a data frame that included country, year, and energy
consumption from wind, solar, other renewables, nuclear, and fossil
fuels.

In order to understand who the largest consumers of energy are, we began
by making a simple faceted barchart for countries of interest, breaking
down their total energy consumption into contributing energy sources.
This allowed us to understand not only who was consuming the most
energy, but also which countries had minimal consumption and therefore
had an easier time increasing their renewable energy shares of their
total consumption. We also made a smaller subset of this facet, looking
at only the US and China in further detail using an area chart.

After determining that the USA and China are by far the largest consumers of fossil fuels, we decided to perform a linear regression in order to model their past consumption and attempt to make future predictions based off of this model.  Based on the R^2 values, we will evaluate whether or not the linear regression model is appropriate to predict these trends. 

To understand our next question of who is making the most progress in
renewables, we decided to make two leaflet plots which visualized the
share of renewable energy in 1990 then 2018. Countries with the lowest
share of renewable energy (out of 100) were colored in darker red hues
to indicate reliance upon fossil fuels, while countries leading the
charge with renewable energy were colored in green. Although no country
had over 50% renewable shares, we were able to determine that the Nordic
countries led the world in renewable shares. But, as we saw with our bar
chart, these countries also do not consume very much energy. Also from
this plot we were able to see how many countries did not have data,
which we will discuss later.

Another question we had was to see which countries were emitting the
most carbon. To begin the discussion around this question, we made an
animated plot of fossil fuel consumption from 1990 to the present for
the US and China, just to provide an idea of how much this has changed
for each country. To move to a global scale, we made a leaflet of carbon
emissions from electricity for countries. However, many countries do not
report their emissions, which was a limitation of this visualization and
our figure.

Finally, to answer our question of who is leading the renewable energy
effort, we made four plots to break this into solar and wind energy, for
both total consumption and per capita. Total consumption allowed us to
understand who is actually producing the most renewable energy, while
per capita allowed us to understand which countries, no matter the size,
led the world. For these we made smooth line graphs from 2000-present.

## Findings + Discussion

Our linear regression models for the USA and China have r^2 values of
0.141 and 0.946, respectively. This is surprising because upon visual
inspection of the plot with both predicted and actual data, the USA
regression line closely follows the data, which appears to be just as if
not more linear than the China data. In 1990, the USA consumed about
twice as much fossil fuel as China. In 2018, the USA consumed about ???
the amount of fossil fuel as china. China???s fossil fuel consumption is
predicted to increase steadily over the next 8 years and by 2030 China
is predicted to consume about twice as much fossil fuel as the USA.
Perhaps China will consider utilizing a higher proportion of renewable
sources as their energy demands continue to grow. Some of the important
points to note is that when looking at the fossil fuel comparison
visualization between China and the USA, we noticed that there was a
sharp increase in slope for China after 2003. On the other hand, there
was a gradual decrease in consumption for the US after 2010. It was also
interesting to find that beginning with 1990, the US doubled China???s
fossil fuel consumption, but as time went by, China consumed more fossil
fuel than the US.

Our figures show that China and the United States consume the most
energy, but have made little overall progress to diversify their energy
consumption in comparison to countries like Germany. With that, our
visualizations show that smaller countries with less energy usage lead
the charge in renewables, possibly because they do not have to generate
as much total energy to support their smaller populations. It was
unexpected to see Brazil leading in renewables, but we learned that this
is not necessarily totally clean renewables like solar and wind, but
does involve biofuel sources mixed with fossil fuels. In terms of wind
consumption per capita and solar consumption per capita, it is
interesting to see that Sweden and Germany, and Australia and Japan,
were leading in their respective energy consumption. As mentioned
previously, these countries rely on foreign export for fossil fuels,
thus they have been trying to be more sustainable by putting more effort
in using their own renewable energy.

Our bar chart shows that in general, renewable sources contribute evenly
to energy consumption in the US and China. Additionally, our figures
show an interesting relationship between leaders in solar and wind which
depends on whether we look at per capita, or overall generation. We see
that usually, larger countries produce more total renewable energy, but
this makes up a much smaller percentage of their total energy
consumption. If we look at per capita, we see that smaller countries are
in fact leaders in renewable energy generation/consumption.

It is important to note that the limitations of the data is that there
were a lot of missing values for Subsaharan Africa. It is unclear why
this is the case our dataset had missing values and it may be due to the
bias of the creator. If more information was collected for Subsaharan
Africa, our findings and research would definitely be more accurate. It
is also important to note that the US model might not be a good fit
because other factors such as the constant change in the market can
impact the accuracy of our US prediction model.

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

World Energy Consumption:
url(<https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption>)

???This dataset is a collection of key metrics maintained by Our World in
Data. It is updated regularly and includes data on energy consumption
(primary energy, per capita, and growth rates), energy mix, electricity
mix and other relevant metrics.???

## References

Poudel, P, *World Energy Consumption: Consumption of energy by different
countries,* electronic dataset, viewed 28 February 2022,
<https://www.kaggle.com/pralabhpoudel/world-energy-consumption>
