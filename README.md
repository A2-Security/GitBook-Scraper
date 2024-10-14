# GitBook Scraper

This Python script scrapes documentation from a GitBook site and converts the extracted HTML content into Markdown format. It can be used to back up documentation or convert it for offline use in Markdown-based repositories or projects.
## Features

- Scrapes all accessible pages of a GitBook website.
- Converts the HTML content into Markdown format using the html2text library.
- Handles links between pages and includes them in the final Markdown document.
- Saves the final Markdown content to a file.

## Requirements

Ensure that you have the following installed:

- Python 3.x
- Required Python packages: requests, beautifulsoup4, html2text

You can install the necessary packages using:

```bash
pip install requests beautifulsoup4 html2text
```
## Usage

To use the script, follow these steps:

### Clone this repository:

```bash
git clone https://github.com/A2-Security/GitBook-Scraper
cd GitBook-Scraper
```
### Update the script:

- Replace the gitbook_url variable in the script with the GitBook URL you want to scrape.

```python
gitbook_url = 'docs-one.example.xyz'  # Example GitBook URL
```
- You can also change the output file name by modifying the output_file variable.

```python
output_file = 'documentation.md'  # Desired output file name
```

### Run the script:

- Execute the script to start scraping the GitBook:

```bash
    python gitbook_scraper.py
```
The script will:
- Fetch the main page of the GitBook.
- Extract and follow all internal links.
- Scrape the content of each page.
- Convert the content to Markdown format.
- Save the output to a Markdown file.

### Check the output:

- Once the script has finished, the Markdown file will be available in the specified output path (documentation.md by default).

## Example

For example, to scrape the documentation from a GitBook page like https://docs-one.example.xyz/, you would:

- Update the gitbook_url in the script to this URL.
- Run the script, and it will generate a file named documentation.md with the full scraped content.
