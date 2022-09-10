# Data-Scraping-from-PDF-Files
This project has been developed for data scraping from monthly added PDF reports on the Mortgage Finance Forecast Archives website (https://www.mba.org/news-and-research/forecasts-and-commentary/mortgage-finance-forecast-archives). The data scraping framework developed in this project converts the tabular data in PDF files to ".csv" format. The developed data scraping framework integrates two different tasks such as web scraping and data extraction. The code uses three different function named as extract_table_columns_name, extract_pdf_data, and get_pdf_files. The get_pdf_files function downloads the pdf files from the archive, and then extracts tabular data and attribute names using extract_pdf_data and extract_table_columns_name functions. The entire structure of the data scraping framework checks out the archive manually for newly added reports and works as a fully automated manner. Besides, the regex expressions in the framework are also compatible with pattern formats that vary in different table structures.  In this project, two different packages used for data extraction from PDF files: pdfplumber and tika-python. At the stage of web scraping, the url links of the pdf files are parsed using lxml feature of the BeautifulSoup package.  When the code is run for the first time, it creates two files named as archievefiles, archievecsvfiles and it also creates a ".csv" file named as archievelinks in cwd. When the code is run for the second time, it only downloads the pdf files in the newly added url links to the archive and performs other operations. 

Feel free to contact me for support.
