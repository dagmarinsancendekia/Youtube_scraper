# TODO List for Testing Shopee Scraper

## Setup Testing
- [ ] Install Python dependencies: selenium, beautifulsoup4, pandas, openpyxl
- [ ] Ensure Chrome browser is installed and up-to-date
- [ ] Verify ChromeDriver compatibility

## Functional Testing
- [ ] Run scraper with keyword "laptop" and 1 page
- [ ] Check if browser opens Shopee search page correctly
- [ ] Verify search results are loaded
- [ ] Confirm data extraction: check if products are found and parsed
- [ ] Validate extracted data fields (nama, harga, terjual, rating) are not empty/N/A

## Output Testing
- [ ] Check if shopee_data.xlsx file is created
- [ ] Open Excel file and verify column headers: Nama Produk, Harga, Terjual, Rating
- [ ] Ensure data rows are populated correctly
- [ ] Check column formatting and widths
- [ ] Test with multiple pages (e.g., 2 pages) and verify data accumulation

## Edge Case Testing
- [ ] Test with invalid search keyword (e.g., random string with no results)
- [ ] Test with 0 pages or negative pages
- [ ] Test network disconnection scenario
- [ ] Test with very long search keywords
- [ ] Verify error handling when page fails to load

## Performance Testing
- [ ] Test scraping speed for 1 page vs multiple pages
- [ ] Ensure headless mode works without GUI issues
- [ ] Check memory usage during scraping
- [ ] Test stability with large number of products

## Validation Testing
- [ ] Manually verify a few extracted data points against actual Shopee website
- [ ] Check data types (strings, numbers) in DataFrame
- [ ] Ensure no duplicate entries in output
- [ ] Validate price formatting and sold count parsing
