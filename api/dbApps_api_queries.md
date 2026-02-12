# API Query Building Assignment
---

## USGS Earthquake Queries

### Query 1: Earthquakes with a minimum magnitude of 6
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=6.0&limit=10
```

**Parameters used:**
- `format`: GeoJSON
- `minmagnitude`: minimum magnitude of 6
- `limit`: limits to 10

**Result:** Showed a few earthquakes, from new zealand, south sandwich islands, russia, japan, etc.

---

### Query 2: Earthquakes from my birth year
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&starttime=2008-01-01&endtime=2008-10-02&limit=10
```

**Parameters used:**
- `format`: GeoJSON
- `starttime and endtime`: limits the earthquakes from the start of 2008 to when I was born
- `limit`: limits the returned earthquakes by 10

**Result:**  many different earthquakes, with magnitudes being pretty low from the ones I collected

---

### Query 3: The most powerful earthquakes on the list
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&limit=10&orderby=magnitude
```

**Parameters used:**
- `format`: GeoJSON
- `limit`: limited the returned earthquakes to 10
- `orderby`: ordered the list from largest to smallest

**Result:** A list of the top 10 largest earthquakes in magnitude. The first being from the Philippines

---

## Open Library Queries

### Query 4: Books written by John Green
**URL:**
```
https://openlibrary.org/search.json?author=john+green&limit=10&language=eng&fields=title,author_name,first_publish_year
```

**Parameters used:**
- `parameter1`: author's name, limit on the number returned, only written in english
- `parameter2`: only getting the title, author name, and first publish year

**Result:** Found roughly 6 books written by John Green, with the rest being written by other people, assumingly because he's only written six books.


### Query 5: Books about sports/with sports in the title
**URL:**
```
https://openlibrary.org/search.json?limit=10&title=sports&fields=title,author_name,first_publish_year
```

**Parameters used:**
- `parameter1`: limiting the list to show only ones with sports in the title
- `parameter2`: only getting the fields of title, author name and first publish year

**Result:** I got multiple books back, whether they are actually about sports, I wouldn't know. The years are varied largely, with some from 1967, to 2003.

### Query 6: Books related to math
**URL:**
```
https://openlibrary.org/search.json?limit=10&q=math&fields=title,author_name,first_publish_year
```

**Parameters used:**
- `parameter1`: I set the query to math, so it tried to look for things related to math
- `parameter2`: Only returning the fields of title, author name and first publish year

**Result:** Interestingly, I feel as if the books returned a 50/50 split between related to math, and just random books. For example, I got a book titled, "Ramayana, a Holy Bible of India", written in 1823. Whether this is related to math at all, I really don't know.