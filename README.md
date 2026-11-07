<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/brand/svg/ir-system-logo-on-dark.svg">
    <img src="docs/brand/svg/ir-system-logo-on-light.svg" alt="Information Retrieval System" width="320">
  </picture>
</p>

<h1 align="center">Crawl Turkish COVID‑19 pages.<br>Search them with TF‑IDF.</h1>

<p align="center">
  Coursework from 2021: a crawler, an inverted index and TF-IDF retrieval.<br>
  <b>Python with Zemberek stemming for Turkish through JPype.</b>
</p>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="NLP: Zemberek" src="https://img.shields.io/badge/NLP-Zemberek-2E4A7D?style=flat-square">
  <img alt="Up to 2,500 pages per crawl" src="https://img.shields.io/badge/pages%20per%20crawl-up%20to%202%2C500-2F6B4F?style=flat-square">
  <img alt="Coursework, 2021" src="https://img.shields.io/badge/project-coursework%202021-2E4A7D?style=flat-square">
  <a href="https://github.com/mertkayacs/InformatiionRetrievalSystem"><img alt="GitHub stars" src="https://img.shields.io/github/stars/mertkayacs/InformatiionRetrievalSystem?style=flat-square&logo=github&color=8A6D3B"></a>
</p>

<p align="center">
  <a href="#quick-start"><img alt="Quick start" src="https://img.shields.io/badge/Quick%20start-2E4A7D?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48cGF0aCBkPSJNMTIgMTV2NXMzLjAzLS41NSA0LTJjMS4wOC0xLjYyIDAtNSAwLTUiLz48cGF0aCBkPSJNNC41IDE2LjVjLTEuNSAxLjI2LTIgNS0yIDVzMy43NC0uNSA1LTJjLjcxLS44NC43LTIuMTMtLjA5LTIuOTFhMi4xOCAyLjE4IDAgMCAwLTIuOTEtLjA5Ii8%2BPHBhdGggZD0iTTkgMTJhMjIgMjIgMCAwIDEgMi0zLjk1QTEyLjg4IDEyLjg4IDAgMCAxIDIyIDJjMCAyLjcyLS43OCA3LjUtNiAxMWEyMi40IDIyLjQgMCAwIDEtNCAyeiIvPjxwYXRoIGQ9Ik05IDEySDRzLjU1LTMuMDMgMi00YzEuNjItMS4wOCA1IC4wNSA1IC4wNSIvPjwvZz48L3N2Zz4%3D&logoColor=white"></a>
  <a href="crawler.py"><img alt="Crawler" src="https://img.shields.io/badge/Crawler-1E2A38?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIvPjxwYXRoIGQ9Ik0xMiAyYTE0LjUgMTQuNSAwIDAgMCAwIDIwYTE0LjUgMTQuNSAwIDAgMCAwLTIwTTIgMTJoMjAiLz48L2c%2BPC9zdmc%2B&logoColor=white"></a>
  <a href="pageRetrieval.py"><img alt="Retrieval" src="https://img.shields.io/badge/Retrieval-1E2A38?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48ZyBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIyIj48cGF0aCBkPSJtMjEgMjEtNC4zNC00LjM0Ii8%2BPGNpcmNsZSBjeD0iMTEiIGN5PSIxMSIgcj0iOCIvPjwvZz48L3N2Zz4%3D&logoColor=white"></a>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/hero-dark.webp">
    <img src="docs/assets/readme/hero-light.webp" alt="Code of the TF-IDF scoring step in pageRetrieval.py, with the page score loop" width="960">
  </picture>
</p>

Information Retrieval System is a small search engine for Turkish COVID-19 web content, written as coursework in 2021. It crawls pages, builds an inverted index with Turkish stemming and ranks matches for a query typed at the console. The whole program is three Python scripts plus the Zemberek library jar.

---

## Why Information Retrieval System

The three stages mirror the classic information retrieval pipeline.

|  |  |
|---|---|
| <img src="docs/assets/readme/icons/globe.svg" width="18" height="18" alt=""> **Crawl** | crawler.py runs one crawl from each of four Turkish COVID-19 pages. Each crawl stops at 2,500 pages and appends them to webPages.json. |
| <img src="docs/assets/readme/icons/list-filter.svg" width="18" height="18" alt=""> **Index** | indexer.py strips punctuation, stems words with Zemberek and writes term frequencies per page to invertedList.json. |
| <img src="docs/assets/readme/icons/search.svg" width="18" height="18" alt=""> **Rank** | pageRetrieval.py scores pages with TF-IDF, using (1 + log10 tf) times log10(N / df), and prints the matching URLs. |

## A quick tour

<table>
  <tr>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/download-dark.webp">
        <img src="docs/assets/readme/tour/download-light.webp" alt="Code card of the crawler download_url method">
      </picture>
      <h3>Download a page</h3>
      A page is fetched, its title and text are kept, and it counts toward the cap.
    </td>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/loop-dark.webp">
        <img src="docs/assets/readme/tour/loop-light.webp" alt="Code card of the crawler run loop">
      </picture>
      <h3>Crawl loop</h3>
      URLs are visited until the queue is empty or 2,500 pages are stored.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/index-dark.webp">
        <img src="docs/assets/readme/tour/index-light.webp" alt="Code card of the inverted index loop in indexer.py">
      </picture>
      <h3>Inverted index</h3>
      Each word is stemmed with Zemberek and counted per page.
    </td>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/assets/readme/tour/save-dark.webp">
        <img src="docs/assets/readme/tour/save-light.webp" alt="Code card of the end of indexer.py that writes invertedList.json">
      </picture>
      <h3>Save the index</h3>
      The inverted index is written to invertedList.json and the Zemberek JVM is shut down.
    </td>
  </tr>
</table>

<p align="center"><sub>Code cards show the files as they are in the repository.</sub></p>

## Features

- Requests and BeautifulSoup crawler with a cap of 2,500 pages per crawl.
- Turkish stemming through the Zemberek jar, called from Python with JPype.
- JSON files for storage, with no database.
- Console menu in Turkish for queries.

## Quick start

```sh
pip install jpype1 beautifulsoup4 requests
```

The JVM path is fixed in `indexer.py` and `pageRetrieval.py` (the `jpype.startJVM` call near the top of each). Point both at the JVM library on your machine and at the `zemberek-tum-2.0.jar` file in this repository. Then run the stages in order:

```sh
echo "[]" > webPages.json
python crawler.py
python indexer.py
python pageRetrieval.py
```

The crawler reads `webPages.json` at the end of each crawl, so create it first as shown.

### Requirements

- Python 3 and a JDK.
- The packages above.

## FAQ

<details>
<summary><b>Why does it need Java?</b></summary>

Zemberek, the Turkish morphological analyser, is a Java library. The scripts call it from Python through JPype.
</details>

<details>
<summary><b>How are results ranked?</b></summary>

By TF-IDF over the inverted index of stemmed words.
</details>

<details>
<summary><b>Why is the repository called InformatiionRetrievalSystem?</b></summary>

The name is the original coursework name and keeps its typo. The project is the Information Retrieval System.
</details>

<details>
<summary><b>Does the crawler still work?</b></summary>

The seeds are four pages from 2021, and some may have moved. The crawler has not been re-run for this README.
</details>

If Information Retrieval System is useful to you, a ⭐ helps other people find it.

Photos behind the screenshots are credited in [docs/assets/readme/CREDITS.md](docs/assets/readme/CREDITS.md).

[![views](https://hits.sh/github.com/mertkayacs/InformatiionRetrievalSystem.svg?view=today-total&style=flat-square&label=views&color=2E4A7D&labelColor=1E2A38)](https://github.com/mertkayacs/InformatiionRetrievalSystem)
