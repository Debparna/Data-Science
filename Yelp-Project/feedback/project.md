# Project Feedback

The SF Open Data Portal actually has specific boundaries for San Francisco
neighborhoods. These are based on official boundaries set by the city as well
as unofficial boundaries set by local real estate agents.

Relatively clear introduction.

Code should not be in the main body of the report! This was mentioned in
lecture and also on Piazza.

Use shapes in addition to color to make sure plots are colorblind-accessible,
as described in the graphics checklist.

Units missing from price vs ratings plot. Is price in USD or in Yelp dollar
signs or something else?

By limiting to top 50 restuarants, you may have invalidated your analysis of
price versus rating. Since the mean ratings you have only span about 0.5 star,
any larger price versus rating trend is likely lost.

Parts of report seem redundant. For example, repeated discussion of how you
used the Yelp Fusion API. It would be clearer and cut down on redundant
information if common data sources were discussed in one place.

Looking at bigrams or trigrams might have solved the contextual problems you
ran into with natural language processing. In general, it seems like you did
not find any clear insights from the NLP analysis you did. It's also likely
that using top 50 reviews biased the outcome.

Do bar plots show health scores or something else? No title or labels.

Rather than examining each data source in isolation, the project would have
been stronger overall if you combined them. For instance, do health inspection
results correlate with the data you found from iwaspoisoned? Do they correlate
with Yelp ratings?

Your reasoning about how to account for population is not correct. If one area
has more reports than another because it is relatively more populous, that area
will also have a relatively higher total percentage of reports. Using
percentage of reports does not solve the problem of population difference
(notice that in order to compute the percentage, we do not need population
statistics!).

You used a bar plot, not a histogram to analyze the food poisoning percentages.
While they look similar, they serve different purposes and display different
kinds of data.

---

R1. Relatively well-organized. Results supported by evidence. Some incorrect
uses of statistics.

R2. Little or no introspection about the limitations of results: no discussion
of potential confounding variables or uncertainty.

F1. Several plots missing titles/labels/units.

F2. No major problems

C1. Code is documented and organized.

C2. No major problems

Project includes data collection, cleaning, and exploration.

See Canvas for individual grades.
