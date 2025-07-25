# ArXNews: A Benchmarking Arabic News Headlines Dataset from Twitter/X

**ArXNews** is a large-scale dataset of over **5.29 million Arabic news headlines** posted by **72 verified Arabic news sources** on **Twitter/X** between **2008 and 2020**. Each headline is enriched with annotations for **topic**, **sentiment**, **emotion**, and **user engagement**, along with linguistic metadata supporting psycholinguistic and computational research.

This repository provides **open access** to the processed dataset files, organized by **yearly quarters** under the `Data/` directory.

---

## 📂 Repository Structure

ArXNews/
│
├── Data/
│ ├── ArXNews_2008-1.csv
│ ├── ArXNews_2008-2.csv
│ ├── ...
│ └── ArXNews_2020-4.csv
│
├── scripts/
│ └── processing_and_annotation_tools/
│
├── README.md
└── LICENSE (CC-BY 4.0)


---

## 📊 Dataset Format

Each CSV file contains the following columns:

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `tweet_id`          | Unique identifier of the tweet (Twitter/X ID)                               |
| `headline`          | Arabic news headline text (cleaned and normalized)                          |
| `tokens`            | Space-separated tokenized headline                                           |
| `lemmas`            | Space-separated lemmas for each token                                        |
| `pos_tags`          | Universal Part-of-Speech tags corresponding to each token                   |
| `morph_features`    | Morphological features (e.g., gender, number, case) per token                |
| `dep_parse`         | Dependency tree in CoNLL-U or JSON format                                    |
| `sentiment`         | Sentiment label: `positive`, `neutral`, or `negative`                        |
| `emotion`           | Emotion label: `joy`, `anger`, `sadness`, `fear`, `surprise`, or `disgust`  |
| `source`            | Name of the Twitter news account                                             |
| `country`           | Country of the news source                                                   |
| `year`              | Year of publication                                                          |
| `quarter`           | Quarter of publication (`Q1`, `Q2`, `Q3`, or `Q4`)                           |
| `likes`             | Number of likes received on the tweet                                        |
| `retweets`          | Number of retweets                                                           |
| `replies`           | Number of replies                                                            |

---

## 🔍 Use Cases

ArXNews can be used for:

- Psycholinguistic analysis of news framing and emotional salience
- NLP research in Arabic sentiment and emotion classification
- Syntactic complexity and dependency structure modeling
- Temporal and cross-source studies of media discourse
- Audience engagement analysis in online journalism

---

## 📜 License

This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.  
You are free to share, adapt, and build upon this dataset for any purpose, with appropriate credit.

---

## 📌 Citation

If you use this dataset in your work, please cite:

@dataset{arxnews2025,
title = {ArXNews: A Benchmarking Arabic News Headlines Dataset from Twitter/X},
author = {Author One and Author Two and Author Three},
year = {2025},
url = {https://github.com/yemen2016/ArXNews},
publisher = {Umm Al-Qura University, Saudi Arabia},
note = {CC-BY 4.0}
}
