# Homework 2.5

As a follow up to the previous question, how many documents in the video.movieDetails collection list both "Comedy" and "Crime" as genres regardless of how many other genres are listed?

NOTE: There is a dump of the video database included in the handouts for the "Creating Documents" lesson. Use that data set to answer this question.

Choose the best answer:

- 13
- 29
- 44
- 56
- 82
- 109
- 248
- 476
- 500
- 514
- 874

## Answer

The answer is 56 as we can see in the following query:

    db.movieDetails.find({genres: {$all: ["Comedy", "Crime"]}}).count()
