# InformatiionRetrievalSystem

A basic search engine for Turkish COVID-19 web content. It implements a classic information retrieval pipeline in three stages: crawling web pages, building an inverted index with Turkish stemming, and querying the index from the command line.

## How to run

Requirements: Python 3, Java (a JDK), and the following Python packages:

```bash
pip install jpype1 beautifulsoup4 requests
```

The JVM path is hardcoded in `indexer.py` and `pageRetrieval.py` (`jpype.startJVM(...)` near the top of each file). Before running, edit both calls to point to the JVM library on your machine and to the `zemberek-tum-2.0.jar` file included in this repo.

Then run the three stages in order:

1. Crawl and save pages to `webPages.json`:

   ```bash
   python crawler.py
   ```

   The crawler starts from a set of Turkish COVID-19 seed pages and stores up to 2500 pages per run.

2. Build the inverted index (`invertedList.json`):

   ```bash
   python indexer.py
   ```

   This strips punctuation, stems words with Zemberek, and writes term frequencies per page.

3. Search:

   ```bash
   python pageRetrieval.py
   ```

   A Turkish console menu lets you enter a query; matching page URLs are ranked with TF-IDF scoring and printed to the console.

## Tech used

- Python 3
- requests and BeautifulSoup (crawling and HTML parsing)
- JPype (jpype1) to call Java from Python
- Zemberek NLP (`zemberek-tum-2.0.jar`) for Turkish word analysis and stemming
- JSON files for storage (`webPages.json`, `invertedList.json`)

## Status

Coursework, 2021.

## License

An educational project. You are free to use and improve it.
