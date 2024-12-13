# Web Scraper

## Introduction
This Python script automates the extraction of data from a given webpage. It retrieves information such as headings, paragraphs, tables, product details, and multimedia links, saving them into structured CSV and JSON formats for further analysis.

## Approach
1. **HTML Parsing**: BeautifulSoup is used to parse HTML content retrieved via HTTP with the `requests` library.
2. **Data Extraction**: CSS selectors , class-based and tag-based searching identify and extract specific elements.
3. **File Writing**:
   - CSV files store tabular data like headings and table contents.
   - JSON files store hierarchical data such as product details and multimedia links.
4. **Special Cases**:
   - Handled hidden elements (e.g., `style="display: none;"`) to extract hidden prices.
   - Managed inline styles and class-based selectors for complex data structures.

## Tools Used
- **Libraries**: `requests`, `beautifulsoup4`, `csv`, `json`
- **Development Tools**: Python IDE or text editor for scripting.

## Output Files
- `Extract_Text_Data.csv`: Contains text data from headings, paragraphs, and lists.
- `Product_Information.json`: Stores detailed product/book information.
- `Links_and_Multimedia.json`: Captures hyperlinks and multimedia links.

## Challenges
- Parsing hidden elements required careful CSS selector handling.
- Ensured consistent formatting in CSV and JSON files despite varying input structures.
