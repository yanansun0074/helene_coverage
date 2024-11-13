# Hurricane Helene Local News Coverage Research

This is a repository for local news coverage analysis on Hurricane Helene in North Carolina, by CISLM.

News article data collected from <a href='https://www.newsbank.com/'>NewsBank</a>

Latest data in: 
'helene_articles_20241113.csv'

Filtered by newspapers in disaster areas from 9/23/2024 to 10/23/2024 --> 1911 articles

| Column Name | Meaning |
| -------- | ------- |
| header | header scraped from newsbank pdf |
| article | texts of the article |
| title | title of the article |
| date | publication date(format: Month day, year)|
| newspaper | publisher |
| author | author names |
| word_count | number of words |

'articles_20241108.csv'

Same data structure




**Todo**:

- 231 articles are picture copies of the hard prints, which make text extraction difficult.

**Tools used**:
- <a href = 'https://github.com/jsvine/pdfplumber'>PdfPlumber</a>: extract texts from pdf
- <a href = 'https://github.com/tesseract-ocr/tesseract'>Tesseract</a>: OCR engine to extract text from images
- <a href = 'https://layout-parser.github.io/'>Layoutparser</a>: decompose complicated layouts
