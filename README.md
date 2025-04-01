# mongodbHW

#Query 1 - Queries through the sample_mfix database to find all movies that have a runtime longer than 200 minutes AND released in 1983. This query displays of each movie:
  - Runtime
  - Title
  - Year released<br>

<b>Query Ran:</b> db.movies.find (truntime: ($gt:200}, year: 1983], (_id: 0, runtime: 1, title: 1, year: 1}) .sort ({ runtime: 1})
<img width="1299" alt="Screen Shot 2025-04-01 at 5 13 04 PM" src="https://github.com/user-attachments/assets/9ffcd77c-e964-46e1-be62-990649eff242" />

#Query 2 - Queries through the sample_mfix database to find all movies that were released after 2014 AND have an IMDB rating greater than 9. This query displays of each movie:
  - Title
  - Year released
  - IMDB rating<br>
  
<b>Query Ran:</b> db. movies. find ({year: [$gt:2014},"imdb.rating": {$gt:9}}, (_id: 0, title: 1, year: 1,"imdb.rating":1}).sort ({"imdb.rating": -1})
<img width="1286" alt="Screen Shot 2025-04-01 at 5 27 37 PM" src="https://github.com/user-attachments/assets/e3981992-6395-4c92-b4bf-77b9aeacecbf" />

Quick view of the "movies" dataset on MongoDB Compass interface
<img width="1503" alt="Screen Shot 2025-04-01 at 5 43 46 PM" src="https://github.com/user-attachments/assets/3d213a82-9d22-4df6-b88b-27b96dac4f66" />
