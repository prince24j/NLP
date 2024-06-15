# Text_Analysis

```markdown
# Interview Response Text Analysis

This repository contains a Python script that performs sentiment analysis and key phrase extraction on transcribed interview responses. The script uses the TextBlob and spaCy libraries to analyze the text and provide an overall quality assessment for each response.

## Objective

Develop a script or application that:
- Analyzes the sentiment of transcribed interview responses using TextBlob.
- Extracts key phrases from each response using spaCy.
- Provides a simple overall quality assessment based on sentiment and key phrases.

## Requirements

- Python 3.6 or higher
- TextBlob
- spaCy
- A sample dataset of transcribed interview responses in a text file

## Installation

1. Clone this repository:
    ```sh
    git clone https://github.com/prince24j/interview-response-analysis.git
    cd interview-response-analysis
    ```

2. Create and activate a virtual environment (optional but recommended):
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required libraries:
    ```sh
    pip install textblob spacy
    python -m textblob.download_corpora
    python -m spacy download en_core_web_sm
    ```

## Usage

1. Prepare a text file named `transcribed_responses.txt` with the transcribed interview responses. Each response should be separated by a double newline (`\n\n`).

2. Run the script:
    ```sh
    python analyze_responses.py
    ```

3. The script will output the sentiment, key phrases, and overall quality for each response.

## Example

Sample content of `transcribed_responses.txt`:

```
I have led multiple projects to success by effectively managing teams and ensuring timely delivery. My experience in project management has taught me the importance of communication and collaboration.

During my last role, we faced significant challenges due to tight deadlines. However, I worked closely with the team to overcome these obstacles and deliver a quality product. We received positive feedback from the client.

I enjoy working on software development projects, particularly using agile methodology. My skills include coding, debugging, and testing, and I am always eager to learn new technologies.

There were some difficulties in meeting deadlines in my previous job. The client feedback was not very encouraging, and we had to make numerous revisions.

In my internship, I focused on developing my data analysis skills. I used Python and SQL extensively to analyze large datasets and generate insights. This experience was invaluable in honing my technical abilities.

My role as a marketing manager involved creating strategies to increase brand awareness and engagement. I led a team that executed successful campaigns, resulting in a 20% increase in sales.

I have a strong background in customer service. In my last position, I managed a support team and implemented a new ticketing system that improved response times by 30%.

As a graphic designer, I have worked on various projects including branding, advertising, and web design. My creativity and attention to detail have helped clients achieve their marketing goals.

My previous job in sales required excellent communication and negotiation skills. I consistently met or exceeded my sales targets and built strong relationships with clients.

In my recent role, I was responsible for financial analysis and reporting. I developed models to forecast revenue and expenses, which helped the company make informed decisions.
```

## Script Explanation

The script performs the following steps:

1. **Read the transcribed responses**: Loads the text data from the file.
2. **Analyze sentiment**: Uses TextBlob to determine if the sentiment is positive, negative, or neutral.
3. **Extract key phrases**: Uses spaCy to extract key phrases from the responses.
4. **Assess quality**: Combines sentiment and key phrases to provide an overall quality assessment.
5. **Output the results**: Prints the sentiment, key phrases, and overall quality for each response.

