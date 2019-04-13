# Feedback

> We will then use this analysis to give the restaurant a health rating and compare to the official health inspection rating to provide an accuracy score. 

This seems to imply that your rating will be more accurate than the health
inspector rating. How can you be sure of this? Do most customers go in the
kitchen?

Why do you need sentiment analysis for this project? Sentiment analysis is
typically used to measure whether a document is positive/negative about a
topic. Is that what you're trying to do? Could you perhaps make the problem
simpler (and get a more accurate solution) by searching for keywords like
"dirty", "unsanitary", "cockroach", etc..?


> The problem that we are trying to address is that health inspections are not always up to date,

Do you have data to support this? How often to health inspections actually take
place? Have you checked?

---

Does a "negative" Yelp post necessarily mean a restaurant has health-related
problems? Do people ever post negative reviews for other reasons? How will you
tell the difference?

Does Yelp label "complaints" separately from regular reviews, and provide this
data to you? If so, why do you also need sentiment analysis? If not, how will
you identify complaints?

> 4. What is the percentage of restaurants with incorrect or outdated health ratings? This can help prove that since yelp reviews are up to date and more realistic, they can be used as a more accurate health metric for restaurants. 

Start here. Which cities can you actually get health inspection data for? You
will probably need to focus on just a few cities, since each city/county
distributes their health inspection data in a different way (if at all).

Be careful about choosing your cities, since you also need to make sure you can
get Yelp data for those cities.


## Data Sources

What is `review.json`? Don't assume the reader is already familiar with your
dataset. The name of the file is not particularly relevant here, either, but if
you want to talk about the dataset by naming a file, you need to explain what
that file is first.

-----

Again, I do not think sentiment analysis is entirely appropriate for what
you're trying to do. You can likely detect many kinds of reported health
violations in reviews through simple string matching.

There are also problems with bias in Yelp reviews. Reviewers are unlikely to
notice violations that are not immediately visible, and most reviewers don't
have access to the kitchen.

You also need to clarify how you will use reviews to decide whether a
restaurant has health problems. In particular, how many reviews have to
complain for you to decide that restaurant has a problem? And how will you test
whether your statistic is accurate if you don't have any data about the "ground
truth"?

Can you get data from websites such as <https://iwaspoisoned.com> and similar?
This data might be more relevant to what you're trying to do.

Start with health inspector data, since you can use health inspector data to
justify whether the claims you made about infrequency of inspections are
actually true.

I am concerned that your proposed project lacks credibility. I do not see a
reliable way for you to check whether your "health score" based on Yelp is
measuring noise versus an actual signal. So it may be a good idea to think
about other things you can do with Yelp data and/or health inspector data that
are more credible.
