# sattvaj-main

# Amazon Product Scraper

This project is a Python script designed to scrape product details from Amazon, including product names, brands, and images. The scraped data is then saved into an Excel file with images embedded. This script utilizes Selenium for web scraping, BeautifulSoup for parsing HTML, and OpenPyXL for Excel file manipulation.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features
- Scrape product details including name and brand from Amazon.
- Download and save product images.
- Save product details and images into an Excel file.
- Uses Selenium for automated browsing.
- Uses BeautifulSoup for HTML parsing.
- Uses OpenPyXL for Excel file creation.

## Prerequisites
- Python 3.x
- Google Chrome browser
- ChromeDriver for Selenium

## Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/your-username/amazon-product-scraper.git
    cd amazon-product-scraper
    ```

2. **Set up a virtual environment (optional but recommended)**
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows use `venv\Scripts\activate`
    ```

3. **Install required packages**
    ```bash
    pip install -r requirements.txt
    ```

4. **Download ChromeDriver**
    - Download the ChromeDriver that matches your Chrome browser version from [here](https://sites.google.com/a/chromium.org/chromedriver/downloads).
    - Extract the downloaded file and place it in a directory included in your system's PATH, or specify the path to `webdriver.Chrome()` in the script.

## Usage

1. **Modify the script to set the search key**
    - Open `index.py` and set your desired search key in the `main` section:
      ```python
      search_key = "Peanut Butter"
      ```

2. **Run the script**
    ```bash
    python index.py
    ```

3. **Check the output**
    - The script will create a directory called `images` where all the downloaded images will be stored.
    - An Excel file named `product_details.xlsx` will be created with the product details and images.

## Project Structure

amazon-product-scraper/
│
├── images/ # Directory to store downloaded images
├── index.py # Main script to run the scraper
├── requirements.txt # Required Python packages
├── README.md # Readme file
└── .gitignore # Gitignore file


## Contributing
Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [Selenium](https://www.selenium.dev/)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [OpenPyXL](https://openpyxl.readthedocs.io/en/stable/)
