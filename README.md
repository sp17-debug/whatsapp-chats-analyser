# whatsapp-chats-analyser
# WhatsApp Chat Analyzer

Overview

The WhatsApp Chat Analyzer is a Streamlit application designed to analyze and visualize WhatsApp chat data. By processing exported chat files, users can gain insights into message statistics, activity patterns, and more.

Features

Upload WhatsApp Chat Files: Easily upload exported chat files for analysis.
User Statistics: View overall chat statistics such as total messages, words, media shared, and links.
Timeline Visualization: Analyze chat activity over time with monthly and daily timelines.
Activity Maps: Discover the busiest days and months with bar charts, and visualize weekly activity with a heatmap.
User Comparison: Identify the most active users in group chats when viewing overall data.
Word Cloud: Generate a visual representation of the most commonly used words in the chat.
Emoji Analysis: View a breakdown of emojis used in chats, including a pie chart representation.

Requirements

To run the application, ensure you have the following Python packages installed:

- `streamlit`
- `matplotlib`
- `seaborn`
- `pandas`
- `wordcloud` (for word cloud generation)

You can install the required packages using pip:

```bash
pip install streamlit matplotlib seaborn pandas wordcloud
```

## Usage

1. Clone this repository or download the source code.
2. Ensure you have the necessary packages installed as mentioned above.
3. Navigate to the project directory in your terminal.
4. Run the Streamlit application:

   ```bash
   streamlit run app.py
   ```

5. Open the provided URL in your web browser.
6. Upload a WhatsApp chat file (in `.txt` format).
7. Select the user for whom you want to analyze the data and click on "Show Analysis".

## How It Works

The application uses several helper functions defined in the `preprocessor` and `helper` modules to process and analyze the data. Here's a brief overview of the main functions:

preprocess(data): Cleans and formats the raw chat data for analysis.
fetch_stats(selected_user, df): Computes basic statistics for the selected user.
monthly_timeline(selected_user, df): Generates a timeline of messages sent monthly.
daily_timeline(selected_user, df): Generates a timeline of messages sent daily.
week_activity_map(selected_user, df): Analyzes activity to find the busiest day of the week.
month_activity_map(selected_user, df): Analyzes activity to find the busiest month.
activity_heatmap(selected_user, df): Creates a heatmap to visualize user activity patterns.
most_busy_users(df): Identifies the most active users in group chats.
create_wordcloud(selected_user, df): Generates a word cloud based on message content.
most_common_words(selected_user, df): Finds the most commonly used words in the chat.
emoji_helper(selected_user, df): Analyzes and counts emoji usage.

Contributing

Contributions are welcome! If you'd like to contribute to the project, please fork the repository and submit a pull request.

License

This project is open-source and available under the [MIT License](LICENSE). 

Acknowledgments
Streamlit for providing an easy-to-use framework for building web applications.
CampusX
The contributors to the libraries used in this project.


