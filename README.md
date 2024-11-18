AI Information Extractor
Overview
The AI Information Extractor is a powerful tool for automating web data retrieval and extraction using custom queries. This project enables users to easily gather specific public information on various entities, streamlining tasks such as retrieving company contact details, product information, and more. The system allows users to upload a list of entities in CSV format, specify a custom query template, and receive organized results extracted from web search results—all within a simple, user-friendly dashboard.

This project demonstrates proficiency in Python, Streamlit, data processing, and API integrations. It is designed to be extensible, with options to connect additional APIs or services as needed.

Key Features
.User-Friendly Dashboard: Built with Streamlit, the dashboard provides a straightforward interface for uploading data, entering queries, and       extracting information.
.Customizable Query Input: Users define a query template with placeholders, enabling flexible searches for specific types of information.
.Automated Web Search and Extraction: The tool performs web searches for each entity and processes search results to extract relevant information.
.Downloadable Results: After extraction, results can be downloaded as a CSV file for further analysis or reporting.

Technologies Used
.Frontend/UI: Streamlit for an interactive web interface
.Backend: Python for data handling and logic
.Data Processing: pandas for CSV operations
.Optional API Integrations: Supports adding web search and language model APIs (e.g., Groq, OpenAI’s GPT API)

Setup Instructions
.Prerequisites
.Python: Version 3.7 or later
.Required Libraries: Install with pip install streamlit pandas

Installation
1.Clone the Repository:
Copy code
git clone https://github.com/manasa22wh1a1261/AI-Information-Extractor.git
2.Navigate to the Project Directory:
Copy code
cd AI_Info_Extractor
3.Install Dependencies:
Copy code
pip install -r requirements.txt

Usage Instructions
Running the Application
1.Start the Streamlit App:

Copy code
streamlit run app.py
This command will open the app in your browser.

2.Using the Dashboard:

Upload a CSV File: Click to upload a CSV file containing entity names (e.g., company names).
Preview Data: The dashboard shows a preview of the uploaded data.
Primary Column Selection: Select the column with entity names, e.g., “company.”
Enter Custom Query: Define a query such as "Get the email address of {company}"—the {company} placeholder will be replaced by each entity in the list.
Start Extraction: Click Start Extraction to initiate the web search and information extraction process.
View and Download Results: Results are displayed in a table and can be downloaded as a CSV file by clicking Download Results as CSV.

Example Use Case
Consider a scenario where you need to collect contact information for a list of companies:

.Upload a CSV file with a column of company names.
.Enter a query like “Get the email address of {company}.”
.Click Start Extraction, and the tool retrieves relevant data for each company.
.Download the compiled contact information as a CSV file for easy reference.

Limitations and Future Improvements
Current Limitations
.Limited to Publicly Available Data: This tool is designed to retrieve publicly accessible information only.
.API Limitations: Performance may be constrained by web search API rate limits and language model costs or restrictions.
Potential Future Enhancements
.Multi-Source Support: Integrate additional data sources for richer information extraction.
.Enhanced Error Handling: Implement detailed error handling to inform users of any retrieval issues or missing data.
.Batch Processing: Add options for processing large datasets in batches to improve scalability.
