# SloozeProject
**Creating Data Crawler Data Extraction**
1. Here I have used Web Scrapper Chrome extension
2. Download the extension and open the site where we need to crawl( I have used Flipkart)
3. I have extracted data from Moblie Phones page
4. Scrapping : Browser Menu > More Tools > Developer Tools
5. Navigate to Web Scrapper Tab
6. Create a new sitemap > Add the url from the page > Create Sitemap
7. Inside the site map add selectors required to collect data > Add New Selector > Give a name > Give required Type > From selector click "Select" and select the div from which data has to be extracted > Continue adding all required selectors
8. Go back to the site map root and add required page links if needed to extract data from all pages > In the initial link add parent as this created "page link" too including "root"
9. From Site map dropdown > Select Scrape > Give both time as 7000ms and above to avoid being blocked from scraping(As site can identify that we are scraping if Request Interval is 3000ms and below
10. Wait till scraping finishes and extract data as csv.(FlipkartPhones.csv)

**Transformation and Loading**
1. Create a databricks commmuntiy account
2. Login in > Create a Workspace > Create a note book > On top right create a Cluster of required core for use
3. Upload the Data csv to databricks : Click on Catalog from left menu > DBFS > Upload.
4. Read the data using the required code > Perform the reuired Analysis and Transformations
5. **EDA** is done in the databricks file that is uplaoded(Flipkart_Phones.ipynb).
