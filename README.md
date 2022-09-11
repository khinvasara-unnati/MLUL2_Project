# Book Recommendation Engine using Collaborative Filtering

## EXECUTIVE SUMMARY

•	**Stakeholder & Business Problem** – Implementing a Book Recommendation System for Crossword Bookstore’s recently launched website to drive revenue & satisfy customer experience <br /> <br />
•	**Business Solution** - Using Crosswords’ User Rating History to build a recommendation engine based on collaborative filtering <br /> <br />
•	**Success Criterias** – Metrics such as incremental revenue, clicks on recommendation pane, decrease in page bounces, change in books sold per user, etc. in an AB Testing environment <br /> <br />
•	**Data Description** – 2 related Datasets taken from stakeholder’s historical data – <br />
  o Books Dataset – 271k rows in total with features like Title, Author, ISBN Code & Publication Year <br />
  o	Ratings Dataset – 1.14m rows from 105k users with features UserID, ISBN Code, Book Ratings <br /><br />
•	**Data Preparations** – Both Datasets have been merged based on common key ISBN Code and pivot is created on the basis of Top Users & Top Books criteria for quality recommendation dataset <br /><br />
•	**Methodology** – Usage of item-to-item collaborative filtering using cosine similarity as a metric <br /><br />
•	**Interpretation** – Highest cosine metric for the input book-name would be sorted and filtered in descending order, out of which Top-5 Books (with highest cosine metric) would be recommended <br /><br />
•	**Recommendations for improvements** <br />
o	Adding more dimensions to the data to increase accuracy of recommendation (like genre, age, etc)<br />
(Secondary Model taking Publication Year as additional input has been made as sample)<br />
o	Adopt Hybrid Filtering approach using collaborative as well as content-based filtering <br />
o	Match Recommendations from Model to available inventory & stock in hand <br />
o	Enhance business offerings by providing options for bundles or “Book of the Month” category<br />
