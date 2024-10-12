# Amazon Reviews Scraper

This project is a Python-based web scraper designed to extract customer reviews from Amazon's Trustpilot review page. It collects information such as reviewer name, country, profile link, review date, review title, review text, and date of experience. The scraper handles multiple pages and applies rate limiting to avoid overloading the server.

## Features
- **Multi-page Scraping:** The script scrapes reviews from multiple pages on Trustpilot for Amazon.
- **Review Details:** Extracts detailed review information, including the reviewer's profile, country, review count, date, and text.
- **Rate Limiting:** Automatically delays after scraping every 10 pages (2 seconds) and every 100 pages (5 minutes) to prevent overloading the server.

## Requirements

The project requires the following Python libraries:

- **requests:** For sending HTTP requests to the webpage.
- **beautifulsoup4:** For parsing the HTML content of the webpage.
- **pandas:** For storing the scraped data in a structured DataFrame.


## You can install the required libraries using:

```bash
pip install requests beautifulsoup4 pandas
```

or 
```bash
pip install -r requirements.txt
```

# How to Use
Clone the repository:

```bash
git clone https://github.com/your-username/amazon-reviews-scraper.git
```
```bash
cd amazon-reviews-scraper
```


**Run the scraper:**
You can customize the number of pages to scrape by modifying the start_page and end_page variables in the script. For example, to scrape the first 5 pages of reviews:

```bash
start_page = 1
end_page = 5
Amazon_reviews = scrape_pages(start_page, end_page)
```

**Save the reviews:**

The scraped data is stored in a pandas DataFrame. You can save it as a CSV file for further analysis.

## Output Format
The scraper returns the following information for each review:

- **Reviewer Name:** The name of the reviewer.
- **Profile Link:** Link to the reviewer's profile on Trustpilot.
- **Country:** The reviewer's country of origin.
- **Review Count:** Number of reviews written by the reviewer.
- **Review Date:** The date the review was posted.
- **Review Title:** Title of the review.
- **Review Text:** The body of the review.
- **Date of Experience:** The date when the reviewer experienced the product/service.

## Rate Limiting
To avoid overloading the Trustpilot website, the script includes automatic delays:

- **2 seconds** after scraping every 10 pages.
- **5 minutes** after scraping every 100 pages.

These delays help reduce the risk of being blocked by the server.

## Contributing
We welcome any contributions! Here are some ways you can contribute:

- **Report bugs:** If you find any issues, please report them in the Issues tab.
- **Suggest features:** Have ideas for new features? Let us know!
- **Improve documentation:** If you see areas where documentation can be improved, feel free to submit a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.


##Contact
If you have any questions or need further clarification, feel free to reach out via dongrei481@gmail.com.