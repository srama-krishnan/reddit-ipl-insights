# 🏏 IPL Reddit Sentiment Analysis

This project analyzes the sentiment of Reddit comments related to IPL teams using GPT-based models. It visualizes fan emotions for each team via smooth KDE plots, giving insights into how fans feel about their favorite franchises during the IPL season.
---

## 📂 Files Included

- `IPL (Reddit) Sentiment Analysis.ipynb` – Main notebook for cleaning, analyzing, and plotting sentiments.
- `IPL Teams Reddit Comments.csv` – Preprocessed dataset with team subreddit labels and sentiment scores.

---

## 🧠 Key Features

```
- Reddit-based IPL team sentiment scraping & analysis.
- GPT-4/4o powered sentiment scoring using OpenAI API.
- Clean KDE visualization for sentiment distribution.
- Custom labeling with full IPL team names.
```

---

## ⚙️ Setup Instructions

### 1. Install dependencies

```
pip install -r requirements.txt
```

### 2. Set your OpenAI API key

Go to https://www.reddit.com/prefs/apps and create an app, select `Script` and note the `client_id` and `client_secret`
Create a `.env` file in the project root with the following content:
```
REDDIT_CLIENT_ID=reddit-client-id
REDDIT_CLIENT_SECRET=secret_key
APIKEY=your-openai-api-key
```
---

## 📊 Output Preview

![image](https://github.com/user-attachments/assets/6ad518ee-5a58-4a43-bb41-ee8696f3ead4)

---

## 📌 IPL Teams Covered

- Chennai Super Kings
- Royal Challengers Bangalore
- Mumbai Indians
- Kolkata Knight Riders
- Rajasthan Royals
- Delhi Capitals
- Sunrisers Hyderabad
- Punjab Kings
- Gujarat Titans
- Lucknow Super Giants

---

## 📈 Sentiment Score

Each comment is assigned a continuous sentiment score ranging from -1 to 1:
-1 → Strongly Negative
0 → Neutral
+1 → Strongly Positive
These scores are generated using a GPT-based model (gpt-4o) by prompting it to evaluate sentiment intensity and context. Unlike basic classification, this model outputs nuanced scores based on emotion, tone, and intent embedded in user comments.

---

## 🧠 Example Prompt Sent to GPT

Score the reddit comment from -1 to 1, where -1 is most negative and 1 is most positive:
CSK always brings their A-game in playoffs. Dhoni’s leadership is just unmatched!
Score: `0.85`
Justification: The comment praises CSK's performance and highlights admiration for the captain, indicating strong positive sentiment.

---

## 🧑‍💻 Author

Built by S Ramakrishnan using Python, OpenAI API, Seaborn, Reddit API & Pandas.

---

## 🪪 License

MIT License – feel free to use, modify, and contribute.
