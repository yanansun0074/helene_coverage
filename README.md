# Hurricane Helene Local News Coverage Research

This is a Github repository for the local news coverage analysis on Hurricane Helene in North Carolina by CISLM.

News article data was collected from <a href='https://www.newsbank.com/'>NewsBank</a>

Latest baseline data in: 
'helene_all_articles_cleaned.csv'

Filtered by newspapers in western NC areas from 9/23/2024 to 10/23/2024 --> 1714 articles

| Column Name | Description |
| -------- | ------- |
| header | header scraped from newsbank pdf |
| article | texts of the article |
| title | title of the article |
| date | publication date(format: Month day, year)|
| newspaper | publisher |
| author | author names |
| County | where the newspaper is |
| Outlet | publisher (from the NC News Census data) |
| article_text | texts after basic cleaning |

**Notebooks**:
- <ins>news_collection.ipynb</ins>: Extract texts from pdfs in *news_bank_pdf* and *helene_articles_readable*. Filter with data in *wnc_county_newsrooms*.

    * Output: *helene_all_articles.csv*
- <ins>news_analysis.ipynb</ins>: Clean and analyze data from *helene_all_articles.csv*
    * Output: *helene_all_articles_cleaned.csv*, *helene_articles_originality_final.csv*, *BERTopic_lables_final.csv*, 

- <ins>visualization</ins>: Create visualizations with data from *graphics_data*
    * Output: *graphics_output*


**Tools used**:
- <a href = 'https://github.com/jsvine/pdfplumber'>PdfPlumber</a>: extract texts from pdf
- <a href = 'https://notebooklm.google.com/'>NotebookLM</a>: extrct texts from newspaper layout
- Adobe Illustrator, <a href = 'https://app.flourish.studio/projects'>flourish</a>: for visualization

