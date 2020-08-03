# Multivariate_Final_Report

## Introduction: The COVID-19 Pandemic

As SARS-CoV-2, more commonly referred to as COVID-19, proliferated to grip all
corners of the country, governors scrambled to implement stay-at-home orders and quarantine
directives as positive test cases skyrocketed. As of April 21, 2020, there are 824,698 confirmed
cases in the United States and 45,297 deaths as a result of the virus (Centers for Disease Control
and Protection 2020). Due to the rapid spread of the virus, hospitals all across the nation have
seen the number of patients increase exponentially; in particular, hospitals in densely-populated
urban areas such as Los Angeles and New York City are seeing their hospitals flood with sick
patients, with the end of the pandemic nowhere near in sight.

As a result, many health experts and scientists pushed measures to stop the rampant
spread of the disease; some of these include constant sterilization through hand soap or hand
sanitizer and “social distancing,” where people are encouraged to maintain six feet worth of
distance between others in public. This is largely an effort to “flatten the curve” or reduce the
peak number of infections so that the healthcare industry will not be overwhelmed.

![Flattening the Curve Graphic, Source: NPR](graph1.png)


Even with these efforts, however, health care systems across the country are struggling to
meet the needs of all their patients; intensive care unit beds are going scarce, doctors are
desperately needed, and the growth of the virus is steadily continuing. As a result, I chose to look
at the abilities of each of the 50 states, Puerto Rico, and Washington D.C. to handle the load of
COVID-19 in the near future.

## Design and Primary Questions:

Specifically, I am interested in looking at the amount of current cases each state and
territory has, along with other facts revolving around available Intensive Care Unit beds and
projected growth of the virus in order to look at the measures each state would theoretically have
to undergo to handle the amount of patients. Through this paper, I plan to delve into the
following research topics: the extent to which markers such as available Intensive Care Unit beds
and Projected Hospitalized Individuals offer redundant information, and how this can be
conveyed more effectively using Principal Components Analysis; the amount of variation in
ability to handle the projected growth of the coronavirus pandemic across states and territories in
the United States through Cluster Analysis; and the presence of underlying factors that explain
the markers of the hospital data through Factor Analysis.

## Data:
My dataset, which I borrowed from globalepidemic.org, focuses on the hospital capacity
per state and territory in the United State during the COVID-19 pandemic (Jha). This dataset is
based on a predictive model of 306 U.S. Hospital markets across all 50 states and additional
territories. This particular model was developed by an experienced group of health system
researchers at Harvard Global Health Institute and the Harvard T.H. Chan School of Public
Health.

Although the dataset contains more than 30 variables, I chose to focus on seven particular
variables: Total Intensive Care Unit Beds, Projected Infected Individuals, Projected Hospitalized
Individuals, Percentage of Total ICU Beds Needed in Six Months, Percentage of Total ICU Beds
Needed in Twelve Months, and Percentage of Total ICU Beds Needed in Eighteen Months. The
Total Intensive Care Unit Beds variable indicates the count of all ICU beds within an HRR that
are set up and staffed. Total Available ICU beds is the number of unoccupied ICU beds on
average. The Projected Infected Individuals variable states the amount of individuals over the
age of 18 that are expected to get infected with COVID-19 over the course of the entire
pandemic. The Projected Hospitalized Individuals is similar in that it states the amount of
individuals over the age of 18 that are expected to get hospitalized due to COVID-19 over the
course of the entire pandemic. Lastly, the Percentage of Total ICU Beds Needed, X months
variables indicate how many ICU beds would need to be available to care for all patients
requiring hospital care within X months. All of the variables are quantitative.

![Data](graph2.png)

I used histograms and normal quantile plots to examine all seven variables. I decided to
log Total ICU Beds, Available ICU Beds, Projected Infected Individuals, and Projected
Hospitalized Individuals due to the magnitude of those variables, their means, and standard
deviations relative to the other variables. I examined the distributions for my variables again, and
these distributions were much closer to normal after examining their respective normal quantile
plots. However, univariate normal distributions do not guarantee a multivariate normal
distribution, so I also used a chi-square quantile plot test (results are displayed in Figure 1 below)

![Figure 1](graph3.png)
