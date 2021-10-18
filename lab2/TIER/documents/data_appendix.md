# billboard_clean.csv
File containing cleaned data from billboard.csv

## year
  - year in which the ranking took place [5307 non-null | 0 null | type=int64]
## artist
  - artist name (if contains name and surname created as "name surname") [5307 non-null | 0 null | type=str]
## track
  - song name [5307 non-null | 0 null | type=str]
## time
  - song duration [5307 non-null | 0 null | type=str]
## genre
  - music genre [5307 non-null | 0 null | type=str]
## week
  - week from in which track scored a place on billboard ranking (since entering the list) [5307 non-null | 0 null | type=int64]
  - melted from columns "x1st.week", "x2nd.week", ... , "x76th.week"
## rank
  - what place the track scored (1-100) [5307 non-null | 0 null | type=int64]
## date
  - date when track scored the rank [5307 non-null | 0 null | type=datetime64]
  - created by calculating calculating "week"s since "date.entered"


# billboard_dates.csv
Side file containing dumped columns from billboard.csv

## track
  - song name
## date.entered
  - date in which song first appeared on ranking
  - data used in cleaning process to calculate "date"
## date.peaked
  - date of ranking in which song scored the best
  - unnecessary and repeated data