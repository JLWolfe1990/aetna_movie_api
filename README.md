# Movie API Code Test

## Pre-requisites

```
gem install bundler
bundle exec rails db:create
```

## Task
Your task is to create an API. It should implement a user stories provided below. While traditionally we have suggested using whatever language and framework you're most comfortable in, as the work we're hiring for is Rails & greenfield, please prioritize using Rails for this challenge.  Google and the interwebs are at your disposal.

Please choose ony one user story, your choice, and implement it; however, prioritize what's in Considerations, below, should you run tight on time and with an eye to what you might want to see running in a production service. Timebox to 3 hours for your own benefit.

We will pair on the code in-person, so please bring in your code with you and be prepared to run locally. Pairing is just to review the code together and extend whatever API endpoint was worked on previously.

**CSV Data**
CSV seed data is located in the `movies.csv` and the `ratings.csv` files.

## Considerations
When developing your solution, please consider the following:

* Structure of your endpoints - Can you easily extend the API to support new endpoints as feature requests come in?
* Quality of your code - Does your code demonstrate the use of design patterns?
* Testability - Is your code testable?
* Can your solution be easily configured and deployed?  Consider guidelines from [12 Factor App](http://12factor.net/) (please do not actually need to deploy this)

## Tips

* This is a test of your abilities and not how fast you can crank through random stories.  As such, it is more important to produce well structured code that meets the criteria in the user stories rather than getting all stories done.
* If you get stuck, please ask someone.  We want to know how you work both as an individual and as part of a team.  You will not lose points for asking for help on something that is unclear or where you are stuck.

## User Stories

#### List All Movies
AC:

* An endpoint exists that lists all movies
* List is paginated: 50 movies per page, the page can be altered with the `page` query params
* Columns should include: imdb id, title, genres, release date, budget
* Budget is displayed in dollars

#### Movie Details
AC:

* An endpoint exists that lists the movie details for a particular movie
* Details should include: imdb id, title, description, release date, budget, runtime, average rating, genres, original language, production companies
* Budget should be displayed in dollars
* Ratings are pulled from the rating database

#### Movies By Year
AC:

* An endpoint exists that will list all movies from a particular year
* List is paginated: 50 movies per page, the page can be altered with the `page` query params
* List is sorted by date in chronological order
* Sort order can be descending
* Columns include: imdb id, title, genres, release date, budget

#### Movies By Genre
AC:

* An endpoint exists that will list all movies by a genre
* List is paginated: 50 movies per page, the page can be altered with the `page` query params
* Columns include: imdb id, title, genres, release date, budget
