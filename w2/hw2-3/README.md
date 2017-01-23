# Homework 2.3

Using the video.movieDetails collection, how many movies list "Sweden" second in the the list of countries.

NOTE: There is a dump of the video database included in the handouts for the "Creating Documents" lesson. Use that data set to answer this question.

Choose the best answer:
- 5
- 6
- 7
- 8
- 9
- 10
- 11
- 12
- 13
- 14

## Answer

The answer is 6 as we can see with the following query:

    db.movieDetails.find({"countries.1": "Sweden"}).count()
