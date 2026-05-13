# 🕷️Search-Engine-Project

A multi-threaded search engine that crawls, indexes, ranks, and retrieves relevant webpages efficiently.

---

## Components

### Crawler
- Reads seed URLs or previous crawl links.
- Parses and normalizes links, skipping duplicates.
- Respects `robots.txt`.
- Multi-threaded for faster crawling.

### Indexer
- Computes term frequency (TF) and document frequency (DF).
- Stores tags for words, removes stop words.

### Ranker
- **Offline:** PageRank and TF-IDF scores computed and stored.
- **Online:** Combines TF-IDF and PageRank with tag weights to rank pages.
- Extracts the most relevant paragraph from each page.

### Query Processor
- Stems query words using Porter Stemmer.
- Retrieves matching webpages and maps tags and URLs.

### Servlet
- Handles partial queries and stores them in the database.
- Generates HTML results with highlighted keywords and pagination.

---

## Features
- Multi-threaded crawling.
- Page indexing
- TF-IDF + PageRank for ranking.
- Tag-weighted scoring.
- Stemmed query processing.
- Highlighted results with pagination.

---

## Technologies
- Java, Servlets
- Multi-threading
- Data structures (HashMaps, files, database)
- HTML for displaying results

