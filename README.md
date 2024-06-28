# Reddit Realtime Analysis Sparkstreaming Hackathon 🤖

#### Using Reddit topics (subreddits such as AskReddit, AskMen AskWomen) providing some insights and metrics in Real-Time.  
#### There are no stupid question?

## Overview

This project sets up a real-time data pipeline to pull questions and comments from Reddit, process them using Apache Spark, and display various metrics on a Streamlit dashboard. It consists of a producer that fetches data from Reddit, a consumer that processes this data using Spark Streaming, and a Streamlit application to visualize the results.

## Features

- **Real-time Data Ingestion:** Continuously pulls questions and comments from Reddit.
- **Data Processing:** Uses Apache Spark Streaming for processing the data.
- **Metrics Visualization:** Displays various metrics in real-time using Streamlit.

## Architecture

- **Producer:** A script that connects to the Reddit API, fetches questions and comments, and pushes them to a messaging system (like Kafka).
- **Consumer:** A Spark Streaming application that consumes data from the messaging system, processes it, and stores the results.
- **Streamlit Dashboard:** A web application that reads the processed data and displays various metrics in real-time.

## Setup and Installation

**Prerequisites**
- Python 3.11 or higher
- Apache Spark 3.5 or higher
- Streamlit 1.35
- Reddit API credentials
- PRAW
- NLTK

## How to Run in Windows
- Build the docker image and run the container
- Configure your Reddit API credentials as a creds.sh file
- Run the Producer notebook cells (see data stream)
- Run the Consumer notebook cells
- In the command prompt run "streamlit run streamlit_app.py"
- Ensure the streamlit_app.py file is in the same directory as the Consumer

## Credits:
 - Olga Beliai: https://github.com/Gliese8
 - Juan Neuenschwander: https://github.com/JuanNeuenschwandesBTS
- Karen Hourican


