# Homework 2.2

Using the video.movieDetails collection, which of the queries below would produce output documents that resemble the following. Check all that apply.

NOTE: We are not asking you to consider specifically which documents would be output from the queries below, but rather what fields the output documents would contain.

    { "title" : "P.S. I Love You" }
    { "title" : "Love Actually" }
    { "title" : "Shakespeare in Love" }

Check all that apply:

- db.movieDetails.find({}, {title: 1, _id: 0})
- db.movieDetails.find({}, {title: 1})
- db.movieDetails.find({title: ""}, {title: 1})
- db.movieDetails.find({}, {title})
- db.movieDetails.find({year: 1964}, {title: 1, _id: 0})
- db.movieDetails.find({title: "Muppets from Space"}, {title: 1})

## Answer

These are the only ones that output just the title field:

- db.movieDetails.find({}, {title: 1, _id: 0})
- db.movieDetails.find({year: 1964}, {title: 1, _id: 0})