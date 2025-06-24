# Information Retrieval System for Turkish COVID-19 Content

This project contains the full codebase for a basic search engine tailored to Turkish COVID-19-related web content.

It implements a classic Information Retrieval (IR) pipeline with three stages:
- **Crawling**: Collecting web pages
- **Indexing**: Creating an inverted index
- **Retrieval**: Querying the indexed content

---

## 🔧 Requirements

Install the following Python packages:

```bash
pip install jpype1 beautifulsoup4 requests
```

Also ensure you have:

- **Java 11+** installed
- `zemberek-tum-2.0.jar` Turkish NLP JAR file

---

## ⚙️ Configuration

Update JVM paths manually in:

- `pageRetrieval.py` (lines 16–17)
- `indexer.py` (lines 13–14)

Example:

```python
jpype.startJVM(
    "C:\\Program Files\\Java\\jdk-11.0.1\\bin\\server\\jvm.dll",
    "-Djava.class.path=C:\\Users\\Ahmet\\PycharmProjects\\InformationRetrievalSystem\\zemberek-tum-2.0.jar",
    "-ea"
)
```

---

## 🚀 Running the Project

1. **Start the crawler**  
   ```bash
   python crawler.py
   ```
   - Downloads and saves web pages to `webPages.json`
   - Writes every 2500 pages (may take time)

2. **Run the indexer**  
   ```bash
   python indexer.py
   ```
   - Generates `invertedList.json` from crawled data

3. **Launch the retrieval interface**  
   ```bash
   python pageRetrieval.py
   ```
   - Search and interact with your IR system!

---

## 📄 Output Files

- `webPages.json` – Raw crawled content
- `invertedList.json` – Inverted index for search
- Search results are printed to console in `pageRetrieval.py`

---

## 🤖 Notes

- This is an **offline IR system**, requiring no internet after crawling.
- It supports **Turkish language** using [Zemberek NLP](https://github.com/ahmetaa/zemberek-nlp).

---

## 📍 License

This project is for educational purposes only. Feel free to use and improve upon it.
