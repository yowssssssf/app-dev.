# app-dev.
# set the API key
omdb.set_default('apikey', '<your_api_key>')

# search for a movie by title
search_results = omdb.search('The Shawshank Redemption')

# get the ID of the first search result
movie_id = search_results[0].imdb_id

# get the full movie details by ID
movie_details = omdb.get(imdbid=movie_id)

# print the movie title and plot
print(movie_details.title)
print(movie_details.plot)
