# MAL_Project
Machine learning projikt :)))

# Noter
- er Status og Airing altid ens ? (skal testes)
- Engelsk titel
- Kunstner / producer
- Meget preprocessing

- Shape = 37900 x 31

- HUSK AT VI PREDICTER **FREMTIDIGE** ANIMES **RATING** :)
.
# Exploration noter
- AnimeId: *delete*
- Title: transform to **TitleLength** & set title as **Index** (Change the 1 duplicate title to something else)
- Title_japanese: *delete*
- Title_synonyms: -> **AmountOfSynonyms**
- Image_url: *delete*
- Type: **OneHotEncode**, keep in mind when doing feature_importance later
- Source: **OneHotEncode**, afterwards remove _unknown_
- Episodes: :)
- Status: 1st delete all *Not yet aired* rows - 2nd *delete* feature
- Airing: *delete*
.
  **All belove** used for finding **release_season**
- Aired_string
- Aired
- Premiered
  .
- Duration: *Might need to handle outliers* -> **Min_duration**
- Rating: **OneHotEncode**
- Score: **THIS IS OUR TARGET**
- Scored_by: *delete* could be another target
- Rank: *delete* could be another target
- Popularity: *delete* could be another target
- Members: *delete* could be another target
- Favorites: *delete* could be another target
- Background: *delete* to many NaN
- Broadcast: *delete* to many NaN
- Related: *delete* could be interesting for later work (not for this project)
.
**Below** concatted to **Is_liscensed**, because of many NaN
- Liscensor: 
- Title_english:
.
*x* should be maximised try (10)
- Studio: Use the biggest studios aka studios with *x*(minimum 3) or more entrees. **OneHotEncoding** rest is just false
- Genre: **OneHotEncoding**
.
- OpeningTheme: Use the biggest artists aka artists with *x*(minimum 5)
- EndingTheme: Use the biggest artists aka artists with *x*(minimum 5)
