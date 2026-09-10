# Customer-Support-Ticket-Analyser
Customer support teams handle numerous service tickets daily. Analysing support tickets helps identify common issues, customer sentiment, support quality, and areas for improvement. In this project, you will build a Python-based Ticket Analysis System that stores, cleans, analyses, and extracts insights from customer support tickets.
# Customer Support Ticket Analysis Using Python

## Project Overview

This project focuses on analyzing customer support ticket data using Python. The objective is to clean customer issue descriptions and generate useful insights from the ticket data.

The project covers text cleaning, keyword-based analysis, priority analysis, longest issue identification, and unique word extraction.

---

## Objectives

- Clean customer issue descriptions using Python string methods.
- Remove punctuation and unnecessary spaces.
- Convert text into lowercase.
- Replace common slang or shorthand words.
- Count tickets containing specific keywords.
- Analyze ticket priorities.
- Find the ticket with the longest issue description.
- Extract and sort unique words from all issue descriptions.

---

## Dataset

The dataset contains customer support ticket information with the following fields:

- `Ticket_No` – Unique ticket number
- `customer_name` – Name of the customer
- `issue` – Customer's issue description
- `status` – Ticket priority/status

A total of **10 customer support tickets** were analyzed.

---

## Step 1: Ticket Data

The ticket data was stored using a Python dictionary-of-lists structure.

Example:

```python
ticket_data = {
    "Ticket_No": [...],
    "customer_name": [...],
    "issue": [...],
    "status": [...]
}
Step 2: Text Cleaning

The issue descriptions were cleaned using Python string methods.

The following operations were performed:

Converted text to lowercase.
Removed punctuation such as . , ! ? -.
Converted multiple spaces into a single space.
Removed leading and trailing spaces.
Replaced slang or shorthand words such as ok with okay.

Python methods used:

.lower()
.replace()
.split()
.join()
.strip()
Step 3: Keyword-Based Issue Insights

A function was created to count tickets containing a specific word.

def count_tickets_with_word(word):
    count = 0

    for issue in cleaned_issues:
        if word.lower() in issue.lower():
            count += 1

    return count

The function was used to analyze the following keywords:

poor
good
slow
excellent

This helped identify common customer feedback patterns.

Step 4: Final Summary and Insights
1. Final Cleaned Ticket Data

The final cleaned ticket data was displayed as a dictionary of lists containing:

Ticket number
Customer name
Cleaned issue description
Priority/status
2. Priority Analysis
Priority	Number of Tickets
High	4
Medium	3
Low	3

Insight: High-priority tickets were the most common and require faster attention from the support team.

3. Longest Issue Description
Ticket Number: 2
Customer Name: Meera
Cleaned Issue: slow response very poor service
Word Count: 5

Insight: The issue indicates concerns about slow response and poor service quality.

4. Unique Words Analysis
Number of Unique Words: 31
The unique words were extracted from all cleaned issue descriptions.
The words were sorted alphabetically.

Examples include:

poor, slow, good, excellent, support, service, response, issue, and technical.

Key Insights
High-priority tickets represent the largest priority category.
Customer issues include concerns about slow response and poor service.
Positive feedback includes words such as good and excellent.
Keyword analysis helps identify common customer concerns quickly.
Unique word extraction provides an overview of the vocabulary used in customer feedback.
Text cleaning makes customer issue descriptions easier to analyze.
Conclusion

This project demonstrates how Python can be used to clean and analyze customer support ticket data. Text preprocessing, keyword analysis, priority analysis, word counting, and unique word extraction provided useful insights into customer feedback.

The analysis can help support teams identify important issues, improve response time, and enhance overall customer service quality.

Technologies Used
Python
Google Colab
Python String Methods
Lists
Dictionaries
Sets
Functions
Loops
Conditional Statements
Skills Demonstrated
Data Cleaning
Text Processing
Data Analysis
Keyword Analysis
Python Programming
Problem Solving
Basic Business Insights
