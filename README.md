# Web scraping Amazons Bestseller Books webpage
Web scraping of amazon's bestseller books web page using `request` and `BeautifulSoup` python libraries

Check out the Jupyter notebook here: https://jovian.com/ahlenoorkhan/project1-web-scraping-bestseller-books-on-amazon

Web scraping, web harvesting, or web data extraction is an automatic method to obtain large amounts of data from websites. Most of this data is unstructured data in an HTML format which is then converted into structured data in a spreadsheet or a database so that it can be used in various applications. There are many different ways to perform web scraping to obtain data from websites. These include using online services, particular API’s or even creating your code for web scraping from scratch. Many large websites, like Google, Twitter, Facebook, StackOverflow, etc. have API’s that allow you to access their data in a structured format. This is the best option, but there are other sites that don’t allow users to access large amounts of data in a structured form or they are simply not that technologically advanced. In that situation, it’s best to use Web Scraping to scrape the website for data.

The pages https://www.amazon.in/gp/bestsellers/books/ref=zg_bs_pg_2?ie=UTF8&pg=1 and https://www.amazon.in/gp/bestsellers/books/ref=zg_bs_pg_2?ie=UTF8&pg=2 provides the top 100 bestseller books on Amazon. The list is updated hourly based on the sales of the books. In this project we'll retrieve information from these pages using web scraping.

We'll use the Python libraries such as Requets and Beautiful Soup to scrape data from these pages.

Here is the outline of the steps we'll be follow:

Download the web page using requests
Parse the HTML source code using beautiful soup
Extract books title, author name, star rating, total ratings, price and URLs from page
Compile the extracted information into Python lists and dictionaries
Extract and combine data from both pages
Save the extracted information to a CSV file.
By the end of the project we'll create a CSV file in the following format:

Book Title, Author, Star Rating, Total Ratings, Price and URL
The Psychology of Money, Morgan Housel, 4.6 out of 5 stars, 43,757, ₹240.00, https://amazon.in/Psychology-Money-Morgan-Housel/dp/9390166268/ref=zg_bs_books_sccl_2/000-0000000-0000000?pd_rd_i=9390166268&psc=1
Word Power Made Easy, Norman Lewis, 4.4 out of 5 stars, 41,780, ₹115.00, https://amazon.in/Word-Power-Made-Norman-Lewis/dp/0143424688/ref=zg_bs_books_sccl_8/000-0000000-0000000?pd_rd_i=0143424688&psc=1
...
